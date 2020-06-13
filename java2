//<![CDATA[	
(function (_0xdc10x2) {
    _0xdc10x2.fn.theiaStickySidebar = function (_0xdc10x3) {
        var _0xdc10x4 = {
            "containerSelector": "",
            "additionalMarginTop": 0,
            "additionalMarginBottom": 0,
            "updateSidebarHeight": true,
            "minWidth": 0,
            "sidebarBehavior": "modern"
        };
        _0xdc10x3 = _0xdc10x2.extend(_0xdc10x4, _0xdc10x3);
        _0xdc10x3.additionalMarginTop = parseInt(_0xdc10x3.additionalMarginTop) || 0;
        _0xdc10x3.additionalMarginBottom = parseInt(_0xdc10x3.additionalMarginBottom) || 0;
        _0xdc10x5(_0xdc10x3, this);
        function _0xdc10x5(_0xdc10x3, _0xdc10x6) {
            var _0xdc10x7 = _0xdc10x9(_0xdc10x3, _0xdc10x6);
            if (!_0xdc10x7) {
                console.log("TST: Body width smaller than options.minWidth. Init is delayed.");
                _0xdc10x2(document).scroll(function (_0xdc10x3, _0xdc10x6) {
                    return function (_0xdc10x8) {
                        var _0xdc10x7 = _0xdc10x9(_0xdc10x3, _0xdc10x6);
                        if (_0xdc10x7) {
                            _0xdc10x2(this).unbind(_0xdc10x8)
                        }
                    }
                }(_0xdc10x3, _0xdc10x6));
                _0xdc10x2(window).resize(function (_0xdc10x3, _0xdc10x6) {
                    return function (_0xdc10x8) {
                        var _0xdc10x7 = _0xdc10x9(_0xdc10x3, _0xdc10x6);
                        if (_0xdc10x7) {
                            _0xdc10x2(this).unbind(_0xdc10x8)
                        }
                    }
                }(_0xdc10x3, _0xdc10x6))
            }
        }
        function _0xdc10x9(_0xdc10x3, _0xdc10x6) {
            if (_0xdc10x3.initialized === true) {
                return true
            };
            if (_0xdc10x2("body").width() < _0xdc10x3.minWidth) {
                return false
            };
            _0xdc10xa(_0xdc10x3, _0xdc10x6);
            return true
        }
        function _0xdc10xa(_0xdc10x3, _0xdc10x6) {
            _0xdc10x3.initialized = true;
            _0xdc10x2("head").append(_0xdc10x2("<style>.theiaStickySidebar:after {content: \"\"; display: table; clear: both;}</style>"));
            _0xdc10x6.each(function () {
                var o = {};
                o.sidebar = _0xdc10x2(this);
                o.options = _0xdc10x3 || {};
                o.container = _0xdc10x2(o.options.containerSelector);
                if (o.container.size() == 0) {
                    o.container = o.sidebar.parent()
                };
                o.sidebar.parents().css("-webkit-transform", "none");
                o.sidebar.css({
                    "position": "relative",
                    "overflow": "visible",
                    "-webkit-box-sizing": "border-box",
                    "-moz-box-sizing": "border-box",
                    "box-sizing": "border-box"
                });
                o.stickySidebar = o.sidebar.find(".theiaStickySidebar");
                if (o.stickySidebar.length == 0) {
                    o.sidebar.find("script").remove();
                    o.stickySidebar = _0xdc10x2("<div>").addClass("theiaStickySidebar").append(o.sidebar.children());
                    o.sidebar.append(o.stickySidebar)
                };
                o.marginTop = parseInt(o.sidebar.css("margin-top"));
                o.marginBottom = parseInt(o.sidebar.css("margin-bottom"));
                o.paddingTop = parseInt(o.sidebar.css("padding-top"));
                o.paddingBottom = parseInt(o.sidebar.css("padding-bottom"));
                var _0xdc10xc = o.stickySidebar.offset().top;
                var _0xdc10xd = o.stickySidebar.outerHeight();
                o.stickySidebar.css("padding-top", 1);
                o.stickySidebar.css("padding-bottom", 1);
                _0xdc10xc -= o.stickySidebar.offset().top;
                _0xdc10xd = o.stickySidebar.outerHeight() - _0xdc10xd - _0xdc10xc;
                if (_0xdc10xc == 0) {
                    o.stickySidebar.css("padding-top", 0);
                    o.stickySidebarPaddingTop = 0
                } else {
                    o.stickySidebarPaddingTop = 1
                };
                if (_0xdc10xd == 0) {
                    o.stickySidebar.css("padding-bottom", 0);
                    o.stickySidebarPaddingBottom = 0
                } else {
                    o.stickySidebarPaddingBottom = 1
                };
                o.previousScrollTop = null;
                o.fixedScrollTop = 0;
                _0xdc10x1d();
                o.onScroll = function (o) {
                    if (!o.stickySidebar.is(":visible")) {
                        return
                    };
                    if (_0xdc10x2("body").width() < o.options.minWidth) {
                        _0xdc10x1d();
                        return
                    };
                    if (o.sidebar.outerWidth(true) + 50 > o.container.width()) {
                        _0xdc10x1d();
                        return
                    };
                    var _0xdc10xe = _0xdc10x2(document).scrollTop();
                    var _0xdc10xf = "static";
                    if (_0xdc10xe >= o.container.offset().top + (o.paddingTop + o.marginTop - o.options.additionalMarginTop)) {
                        var _0xdc10x10 = o.paddingTop + o.marginTop + _0xdc10x3.additionalMarginTop;
                        var _0xdc10x11 = o.paddingBottom + o.marginBottom + _0xdc10x3.additionalMarginBottom;
                        var _0xdc10x12 = o.container.offset().top;
                        var _0xdc10x13 = o.container.offset().top + _0xdc10x1e(o.container);
                        var _0xdc10x14 = 0 + _0xdc10x3.additionalMarginTop;
                        var _0xdc10x15;
                        var _0xdc10x16 = (o.stickySidebar.outerHeight() + _0xdc10x10 + _0xdc10x11) < _0xdc10x2(window).height();
                        if (_0xdc10x16) {
                            _0xdc10x15 = _0xdc10x14 + o.stickySidebar.outerHeight()
                        } else {
                            _0xdc10x15 = _0xdc10x2(window).height() - o.marginBottom - o.paddingBottom - _0xdc10x3.additionalMarginBottom
                        };
                        var _0xdc10x17 = _0xdc10x12 - _0xdc10xe + o.paddingTop + o.marginTop;
                        var _0xdc10x18 = _0xdc10x13 - _0xdc10xe - o.paddingBottom - o.marginBottom;
                        var _0xdc10x19 = o.stickySidebar.offset().top - _0xdc10xe;
                        var _0xdc10x1a = o.previousScrollTop - _0xdc10xe;
                        if (o.stickySidebar.css("position") == "fixed") {
                            if (o.options.sidebarBehavior == "modern") {
                                _0xdc10x19 += _0xdc10x1a
                            }
                        };
                        if (o.options.sidebarBehavior == "legacy") {
                            _0xdc10x19 = _0xdc10x15 - o.stickySidebar.outerHeight();
                            _0xdc10x19 = Math.max(_0xdc10x19, _0xdc10x15 - o.stickySidebar.outerHeight())
                        };
                        if (_0xdc10x1a > 0) {
                            _0xdc10x19 = Math.min(_0xdc10x19, _0xdc10x14)
                        } else {
                            _0xdc10x19 = Math.max(_0xdc10x19, _0xdc10x15 - o.stickySidebar.outerHeight())
                        };
                        _0xdc10x19 = Math.max(_0xdc10x19, _0xdc10x17);
                        _0xdc10x19 = Math.min(_0xdc10x19, _0xdc10x18 - o.stickySidebar.outerHeight());
                        var _0xdc10x1b = o.container.height() == o.stickySidebar.outerHeight();
                        if (!_0xdc10x1b && _0xdc10x19 == _0xdc10x14) {
                            _0xdc10xf = "fixed"
                        } else {
                            if (!_0xdc10x1b && _0xdc10x19 == _0xdc10x15 - o.stickySidebar.outerHeight()) {
                                _0xdc10xf = "fixed"
                            } else {
                                if (_0xdc10xe + _0xdc10x19 - o.sidebar.offset().top - o.paddingTop <= _0xdc10x3.additionalMarginTop) {
                                    _0xdc10xf = "static"
                                } else {
                                    _0xdc10xf = "absolute"
                                }
                            }
                        }
                    };
                    if (_0xdc10xf == "fixed") {
                        o.stickySidebar.css({
                            "position": "fixed",
                            "width": o.sidebar.width(),
                            "top": _0xdc10x19,
                            "left": o.sidebar.offset().left + parseInt(o.sidebar.css("padding-left"))
                        })
                    } else {
                        if (_0xdc10xf == "absolute") {
                            var _0xdc10x1c = {};
                            if (o.stickySidebar.css("position") != "absolute") {
                                _0xdc10x1c.position = "absolute";
                                _0xdc10x1c.top = _0xdc10xe + _0xdc10x19 - o.sidebar.offset().top - o.stickySidebarPaddingTop - o.stickySidebarPaddingBottom
                            };
                            _0xdc10x1c.width = o.sidebar.width();
                            _0xdc10x1c.left = "";
                            o.stickySidebar.css(_0xdc10x1c)
                        } else {
                            if (_0xdc10xf == "static") {
                                _0xdc10x1d()
                            }
                        }
                    };
                    if (_0xdc10xf != "static") {
                        if (o.options.updateSidebarHeight == true) {
                            o.sidebar.css({
                                "min-height": o.stickySidebar.outerHeight() + o.stickySidebar.offset().top - o.sidebar.offset().top + o.paddingBottom
                            })
                        }
                    };
                    o.previousScrollTop = _0xdc10xe
                };
                o.onScroll(o);
                _0xdc10x2(document).scroll(function (o) {
                    return function () {
                        o.onScroll(o)
                    }
                }(o));
                _0xdc10x2(window).resize(function (o) {
                    return function () {
                        o.stickySidebar.css({
                            "position": "static"
                        });
                        o.onScroll(o)
                    }
                }(o));
                function _0xdc10x1d() {
                    o.fixedScrollTop = 0;
                    o.sidebar.css({
                        "min-height": "1px"
                    });
                    o.stickySidebar.css({
                        "position": "static",
                        "width": ""
                    })
                }
                function _0xdc10x1e(_0xdc10x1f) {
                    var _0xdc10x20 = _0xdc10x1f.height();
                    _0xdc10x1f.children().each(function () {
                        _0xdc10x20 = Math.max(_0xdc10x20, _0xdc10x2(this).height())
                    });
                    return _0xdc10x20
                }
            })
        }
    }
})(jQuery);
window.selectnav = function () {
    "use strict";
    var _0xdc10x1f = function (_0xdc10x1f, _0xdc10x21) {
        function c(_0xdc10x1f) {
            var _0xdc10x21;
            if (!_0xdc10x1f) {
                _0xdc10x1f = window.event
            };
            if (_0xdc10x1f.target) {
                _0xdc10x21 = _0xdc10x1f.target
            } else {
                if (_0xdc10x1f.srcElement) {
                    _0xdc10x21 = _0xdc10x1f.srcElement
                }
            };
            if (_0xdc10x21.nodeType === 3) {
                _0xdc10x21 = _0xdc10x21.parentNode
            };
            if (_0xdc10x21.value) {
                window.location.href = _0xdc10x21.value
            }
        }
        function _0xdc10x23(_0xdc10x1f) {
            var _0xdc10x21 = _0xdc10x1f.nodeName.toLowerCase();
            return _0xdc10x21 === "ul" || _0xdc10x21 === "ol"
        }
        function _0xdc10x24(_0xdc10x1f) {
            for (var _0xdc10x21 = 1; document.getElementById("selectnav" + _0xdc10x21); _0xdc10x21++) {;
            };
            return _0xdc10x1f ? "selectnav" + _0xdc10x21 : "selectnav" + (_0xdc10x21 - 1)
        }
        function _0xdc10x25(_0xdc10x1f) {
            _0xdc10x31++;
            var _0xdc10x21 = _0xdc10x1f.children.length,
                _0xdc10x26 = "",
                _0xdc10x27 = "",
                c = _0xdc10x31 - 1;
            if (!_0xdc10x21) {
                return
            };
            if (c) {
                while (c--) {
                    _0xdc10x27 += o
                };
                _0xdc10x27 += " "
            };
            for (var _0xdc10x28 = 0; _0xdc10x28 < _0xdc10x21; _0xdc10x28++) {
                var _0xdc10x29 = _0xdc10x1f.children[_0xdc10x28].children[0];
                if (typeof _0xdc10x29 !== "undefined") {
                    var _0xdc10x2a = _0xdc10x29.innerText || _0xdc10x29.textContent;
                    var _0xdc10x2b = "";
                    if (_0xdc10x2d) {
                        _0xdc10x2b = _0xdc10x29.className.search(_0xdc10x2d) !== -1 || _0xdc10x29.parentNode.className.search(_0xdc10x2d) !== -1 ? _0xdc10x32 : ""
                    };
                    if (_0xdc10x2e && !_0xdc10x2b) {
                        _0xdc10x2b = _0xdc10x29.href === document.URL ? _0xdc10x32 : ""
                    };
                    _0xdc10x26 += "<option value=\"" + _0xdc10x29.href + "\" " + _0xdc10x2b + ">" + _0xdc10x27 + _0xdc10x2a + "</option>";
                    if (s) {
                        var _0xdc10x2c = _0xdc10x1f.children[_0xdc10x28].children[1];
                        if (_0xdc10x2c && _0xdc10x23(_0xdc10x2c)) {
                            _0xdc10x26 += _0xdc10x25(_0xdc10x2c)
                        }
                    }
                }
            };
            if (_0xdc10x31 === 1 && u) {
                _0xdc10x26 = "<option value=\"\">" + u + "</option>" + _0xdc10x26
            };
            if (_0xdc10x31 === 1) {
                _0xdc10x26 = "<select class=\"selectnav\" id=\"" + _0xdc10x24(true) + "\">" + _0xdc10x26 + "</select>"
            };
            _0xdc10x31--;
            return _0xdc10x26
        }
        _0xdc10x1f = document.getElementById(_0xdc10x1f);
        if (!_0xdc10x1f) {
            return
        };
        if (!_0xdc10x23(_0xdc10x1f)) {
            return
        };
        if (!("insertAdjacentHTML" in window.document.documentElement)) {
            return
        };
        document.documentElement.className += " js";
        var _0xdc10x26 = _0xdc10x21 || {},
            _0xdc10x2d = _0xdc10x26.activeclass || "active",
            _0xdc10x2e = typeof _0xdc10x26.autoselect === "boolean" ? _0xdc10x26.autoselect : true,
            s = typeof _0xdc10x26.nested === "boolean" ? _0xdc10x26.nested : true,
            o = _0xdc10x26.indent || "-",
            u = _0xdc10x26.label || "القائمة",
            _0xdc10x31 = 0,
            _0xdc10x32 = " selected ";
        _0xdc10x1f.insertAdjacentHTML("afterend", _0xdc10x25(_0xdc10x1f));
        var _0xdc10x27 = document.getElementById(_0xdc10x24());
        if (_0xdc10x27.addEventListener) {
            _0xdc10x27.addEventListener("change", c)
        };
        if (_0xdc10x27.attachEvent) {
            _0xdc10x27.attachEvent("onchange", c)
        };
        return _0xdc10x27
    };
    return function (_0xdc10x21, _0xdc10x26) {
        _0xdc10x1f(_0xdc10x21, _0xdc10x26)
    }
}();
(function () {
    var _0xdc10x33 = {
        frameRate: 150,
        animationTime: 800,
        stepSize: 120,
        pulseAlgorithm: true,
        pulseScale: 8,
        pulseNormalize: 1,
        accelerationDelta: 20,
        accelerationMax: 1,
        keyboardSupport: true,
        arrowScroll: 50,
        touchpadSupport: true,
        fixedBackground: true,
        excluded: ""
    };
    var _0xdc10x3 = _0xdc10x33;
    var _0xdc10x34 = false;
    var _0xdc10x35 = false;
    var _0xdc10x36 = {
        x: 0,
        y: 0
    };
    var _0xdc10x37 = false;
    var _0xdc10x38 = document.documentElement;
    var _0xdc10x39;
    var _0xdc10x3a;
    var _0xdc10x3b = [120, 120, 120];
    var _0xdc10x3c = {
        left: 37,
        up: 38,
        right: 39,
        down: 40,
        spacebar: 32,
        pageup: 33,
        pagedown: 34,
        end: 35,
        home: 36
    };
    var _0xdc10x3 = _0xdc10x33;
    function _0xdc10x3d() {
        var _0xdc10x3e = false;
        if (_0xdc10x3e) {
            _0xdc10x6f("keydown", _0xdc10x5d)
        };
        if (_0xdc10x3.keyboardSupport && !_0xdc10x3e) {
            _0xdc10x6b("keydown", _0xdc10x5d)
        }
    }
    function _0xdc10xa() {
        if (!document.body) {
            return
        };
        var _0xdc10x3f = document.body;
        var _0xdc10x40 = document.documentElement;
        var _0xdc10x41 = window.innerHeight;
        var _0xdc10x42 = _0xdc10x3f.scrollHeight;
        _0xdc10x38 = (document.compatMode.indexOf("CSS") >= 0) ? _0xdc10x40 : _0xdc10x3f;
        _0xdc10x39 = _0xdc10x3f;
        _0xdc10x3d();
        _0xdc10x37 = true;
        if (top != self) {
            _0xdc10x35 = true
        } else {
            if (_0xdc10x42 > _0xdc10x41 && (_0xdc10x3f.offsetHeight <= _0xdc10x41 || _0xdc10x40.offsetHeight <= _0xdc10x41)) {
                var _0xdc10x43 = false;
                var _0xdc10x44 = function () {
                    if (!_0xdc10x43 && _0xdc10x40.scrollHeight != document.height) {
                        _0xdc10x43 = true;
                        setTimeout(function () {
                            _0xdc10x40.style.height = document.height + "px";
                            _0xdc10x43 = false
                        }, 500)
                    }
                };
                _0xdc10x40.style.height = "auto";
                setTimeout(_0xdc10x44, 10);
                if (_0xdc10x38.offsetHeight <= _0xdc10x41) {
                    var _0xdc10x45 = document.createElement("div");
                    _0xdc10x45.style.clear = "both";
                    _0xdc10x3f.appendChild(_0xdc10x45)
                }
            }
        };
        if (!_0xdc10x3.fixedBackground && !_0xdc10x34) {
            _0xdc10x3f.style.backgroundAttachment = "scroll";
            _0xdc10x40.style.backgroundAttachment = "scroll"
        }
    }
    var _0xdc10x46 = [];
    var _0xdc10x43 = false;
    var _0xdc10x47 = +new Date;
    function _0xdc10x48(_0xdc10x49, _0xdc10x4a, _0xdc10x19, _0xdc10x4b) {
        _0xdc10x4b || (_0xdc10x4b = 1000);
        _0xdc10x72(_0xdc10x4a, _0xdc10x19);
        if (_0xdc10x3.accelerationMax != 1) {
            var _0xdc10x4c = +new Date;
            var _0xdc10x4d = _0xdc10x4c - _0xdc10x47;
            if (_0xdc10x4d < _0xdc10x3.accelerationDelta) {
                var _0xdc10x4e = (1 + (30 / _0xdc10x4d)) / 2;
                if (_0xdc10x4e > 1) {
                    _0xdc10x4e = Math.min(_0xdc10x4e, _0xdc10x3.accelerationMax);
                    _0xdc10x4a *= _0xdc10x4e;
                    _0xdc10x19 *= _0xdc10x4e
                }
            };
            _0xdc10x47 = +new Date
        };
        _0xdc10x46.push({
            x: _0xdc10x4a,
            y: _0xdc10x19,
            lastX: (_0xdc10x4a < 0) ? 0.99 : -0.99,
            lastY: (_0xdc10x19 < 0) ? 0.99 : -0.99,
            start: +new Date
        });
        if (_0xdc10x43) {
            return
        };
        var _0xdc10x4f = (_0xdc10x49 === document.body);
        var _0xdc10x50 = function (_0xdc10x51) {
            var _0xdc10x4c = +new Date;
            var _0xdc10x52 = 0;
            var _0xdc10x53 = 0;
            for (var _0xdc10x2e = 0; _0xdc10x2e < _0xdc10x46.length; _0xdc10x2e++) {
                var _0xdc10x54 = _0xdc10x46[_0xdc10x2e];
                var _0xdc10x4d = _0xdc10x4c - _0xdc10x54.start;
                var _0xdc10x55 = (_0xdc10x4d >= _0xdc10x3.animationTime);
                var _0xdc10xf = (_0xdc10x55) ? 1 : _0xdc10x4d / _0xdc10x3.animationTime;
                if (_0xdc10x3.pulseAlgorithm) {
                    _0xdc10xf = _0xdc10x7f(_0xdc10xf)
                };
                var _0xdc10x56 = (_0xdc10x54.x * _0xdc10xf - _0xdc10x54.lastX) >> 0;
                var _0xdc10x2b = (_0xdc10x54.y * _0xdc10xf - _0xdc10x54.lastY) >> 0;
                _0xdc10x52 += _0xdc10x56;
                _0xdc10x53 += _0xdc10x2b;
                _0xdc10x54.lastX += _0xdc10x56;
                _0xdc10x54.lastY += _0xdc10x2b;
                if (_0xdc10x55) {
                    _0xdc10x46.splice(_0xdc10x2e, 1);
                    _0xdc10x2e--
                }
            };
            if (_0xdc10x4f) {
                window.scrollBy(_0xdc10x52, _0xdc10x53)
            } else {
                if (_0xdc10x52) {
                    _0xdc10x49.scrollLeft += _0xdc10x52
                };
                if (_0xdc10x53) {
                    _0xdc10x49.scrollTop += _0xdc10x53
                }
            };
            if (!_0xdc10x4a && !_0xdc10x19) {
                _0xdc10x46 = []
            };
            if (_0xdc10x46.length) {
                _0xdc10x78(_0xdc10x50, _0xdc10x49, (_0xdc10x4b / _0xdc10x3.frameRate + 1))
            } else {
                _0xdc10x43 = false
            }
        };
        _0xdc10x78(_0xdc10x50, _0xdc10x49, 0);
        _0xdc10x43 = true
    }
    function _0xdc10x57(_0xdc10x58) {
        if (!_0xdc10x37) {
            _0xdc10xa()
        };
        var _0xdc10x59 = _0xdc10x58.target;
        var _0xdc10x5a = _0xdc10x68(_0xdc10x59);
        if (!_0xdc10x5a || _0xdc10x58.defaultPrevented || _0xdc10x70(_0xdc10x39, "embed") || (_0xdc10x70(_0xdc10x59, "embed") && /\.pdf/i.test(_0xdc10x59.src))) {
            return true
        };
        var _0xdc10x5b = _0xdc10x58.wheelDeltaX || 0;
        var _0xdc10x5c = _0xdc10x58.wheelDeltaY || 0;
        if (!_0xdc10x5b && !_0xdc10x5c) {
            _0xdc10x5c = _0xdc10x58.wheelDelta || 0
        };
        if (!_0xdc10x3.touchpadSupport && _0xdc10x74(_0xdc10x5c)) {
            return true
        };
        if (Math.abs(_0xdc10x5b) > 1.2) {
            _0xdc10x5b *= _0xdc10x3.stepSize / 120
        };
        if (Math.abs(_0xdc10x5c) > 1.2) {
            _0xdc10x5c *= _0xdc10x3.stepSize / 120
        };
        _0xdc10x48(_0xdc10x5a, -_0xdc10x5b, -_0xdc10x5c);
        _0xdc10x58.preventDefault()
    }
    function _0xdc10x5d(_0xdc10x58) {
        var _0xdc10x59 = _0xdc10x58.target;
        var _0xdc10x5e = _0xdc10x58.ctrlKey || _0xdc10x58.altKey || _0xdc10x58.metaKey || (_0xdc10x58.shiftKey && _0xdc10x58.keyCode !== _0xdc10x3c.spacebar);
        if (/input|textarea|select|embed/i.test(_0xdc10x59.nodeName) || _0xdc10x59.isContentEditable || _0xdc10x58.defaultPrevented || _0xdc10x5e) {
            return true
        };
        if (_0xdc10x70(_0xdc10x59, "button") && _0xdc10x58.keyCode === _0xdc10x3c.spacebar) {
            return true
        };
        var _0xdc10x5f, _0xdc10x56 = 0,
            _0xdc10x2b = 0;
        var _0xdc10x49 = _0xdc10x68(_0xdc10x39);
        var _0xdc10x60 = _0xdc10x49.clientHeight;
        if (_0xdc10x49 == document.body) {
            _0xdc10x60 = window.innerHeight
        };
        switch (_0xdc10x58.keyCode) {
        case _0xdc10x3c.up:
            _0xdc10x2b = -_0xdc10x3.arrowScroll;
            break;
        case _0xdc10x3c.down:
            _0xdc10x2b = _0xdc10x3.arrowScroll;
            break;
        case _0xdc10x3c.spacebar:
            _0xdc10x5f = _0xdc10x58.shiftKey ? 1 : -1;
            _0xdc10x2b = -_0xdc10x5f * _0xdc10x60 * 0.9;
            break;
        case _0xdc10x3c.pageup:
            _0xdc10x2b = -_0xdc10x60 * 0.9;
            break;
        case _0xdc10x3c.pagedown:
            _0xdc10x2b = _0xdc10x60 * 0.9;
            break;
        case _0xdc10x3c.home:
            _0xdc10x2b = -_0xdc10x49.scrollTop;
            break;
        case _0xdc10x3c.end:
            var _0xdc10x61 = _0xdc10x49.scrollHeight - _0xdc10x49.scrollTop - _0xdc10x60;
            _0xdc10x2b = (_0xdc10x61 > 0) ? _0xdc10x61 + 10 : 0;
            break;
        case _0xdc10x3c.left:
            _0xdc10x56 = -_0xdc10x3.arrowScroll;
            break;
        case _0xdc10x3c.right:
            _0xdc10x56 = _0xdc10x3.arrowScroll;
            break;
        default:
            return true
        };
        _0xdc10x48(_0xdc10x49, _0xdc10x56, _0xdc10x2b);
        _0xdc10x58.preventDefault()
    }
    function _0xdc10x62(_0xdc10x58) {
        _0xdc10x39 = _0xdc10x58.target
    }
    var _0xdc10x63 = {};
    setInterval(function () {
        _0xdc10x63 = {}
    }, 10 * 1000);
    var _0xdc10x64 = (function () {
        var _0xdc10x2e = 0;
        return function (_0xdc10x65) {
            return _0xdc10x65.uniqueID || (_0xdc10x65.uniqueID = _0xdc10x2e++)
        }
    })();
    function _0xdc10x66(_0xdc10x67, _0xdc10x5a) {
        for (var _0xdc10x2e = _0xdc10x67.length; _0xdc10x2e--;) {
            _0xdc10x63[_0xdc10x64(_0xdc10x67[_0xdc10x2e])] = _0xdc10x5a
        };
        return _0xdc10x5a
    }
    function _0xdc10x68(_0xdc10x65) {
        var _0xdc10x67 = [];
        var _0xdc10x69 = _0xdc10x38.scrollHeight;
        do {
            var _0xdc10x6a = _0xdc10x63[_0xdc10x64(_0xdc10x65)];
            if (_0xdc10x6a) {
                return _0xdc10x66(_0xdc10x67, _0xdc10x6a)
            };
            _0xdc10x67.push(_0xdc10x65);
            if (_0xdc10x69 === _0xdc10x65.scrollHeight) {
                if (!_0xdc10x35 || _0xdc10x38.clientHeight + 10 < _0xdc10x69) {
                    return _0xdc10x66(_0xdc10x67, document.body)
                }
            } else {
                if (_0xdc10x65.clientHeight + 10 < _0xdc10x65.scrollHeight) {
                    overflow = getComputedStyle(_0xdc10x65, "").getPropertyValue("overflow-y");
                    if (overflow === "scroll" || overflow === "auto") {
                        return _0xdc10x66(_0xdc10x67, _0xdc10x65)
                    }
                }
            }
        } while (_0xdc10x65 = _0xdc10x65.parentNode);
    }
    function _0xdc10x6b(_0xdc10x6c, _0xdc10x6d, _0xdc10x6e) {
        window.addEventListener(_0xdc10x6c, _0xdc10x6d, (_0xdc10x6e || false))
    }
    function _0xdc10x6f(_0xdc10x6c, _0xdc10x6d, _0xdc10x6e) {
        window.removeEventListener(_0xdc10x6c, _0xdc10x6d, (_0xdc10x6e || false))
    }
    function _0xdc10x70(_0xdc10x65, _0xdc10x71) {
        return (_0xdc10x65.nodeName || "").toLowerCase() === _0xdc10x71.toLowerCase()
    }
    function _0xdc10x72(_0xdc10x56, _0xdc10x2b) {
        _0xdc10x56 = (_0xdc10x56 > 0) ? 1 : -1;
        _0xdc10x2b = (_0xdc10x2b > 0) ? 1 : -1;
        if (_0xdc10x36.x !== _0xdc10x56 || _0xdc10x36.y !== _0xdc10x2b) {
            _0xdc10x36.x = _0xdc10x56;
            _0xdc10x36.y = _0xdc10x2b;
            _0xdc10x46 = [];
            _0xdc10x47 = 0
        }
    }
    var _0xdc10x73;
    function _0xdc10x74(_0xdc10x5c) {
        if (!_0xdc10x5c) {
            return
        };
        _0xdc10x5c = Math.abs(_0xdc10x5c);
        _0xdc10x3b.push(_0xdc10x5c);
        _0xdc10x3b.shift();
        clearTimeout(_0xdc10x73);
        var _0xdc10x75 = (_0xdc10x76(_0xdc10x3b[0], 120) && _0xdc10x76(_0xdc10x3b[1], 120) && _0xdc10x76(_0xdc10x3b[2], 120));
        return !_0xdc10x75
    }
    function _0xdc10x76(_0xdc10x26, _0xdc10x77) {
        return (Math.floor(_0xdc10x26 / _0xdc10x77) == _0xdc10x26 / _0xdc10x77)
    }
    var _0xdc10x78 = (function () {
        return window.requestAnimationFrame || window.webkitRequestAnimationFrame || function (_0xdc10x79, _0xdc10x7a, _0xdc10x4b) {
            window.setTimeout(_0xdc10x79, _0xdc10x4b || (1000 / 60))
        }
    })();
    function _0xdc10x7b(_0xdc10x56) {
        var _0xdc10x7c, _0xdc10x7d, _0xdc10x7e;
        _0xdc10x56 = _0xdc10x56 * _0xdc10x3.pulseScale;
        if (_0xdc10x56 < 1) {
            _0xdc10x7c = _0xdc10x56 - (1 - Math.exp(-_0xdc10x56))
        } else {
            _0xdc10x7d = Math.exp(-1);
            _0xdc10x56 -= 1;
            _0xdc10x7e = 1 - Math.exp(-_0xdc10x56);
            _0xdc10x7c = _0xdc10x7d + (_0xdc10x7e * (1 - _0xdc10x7d))
        };
        return _0xdc10x7c * _0xdc10x3.pulseNormalize
    }
    function _0xdc10x7f(_0xdc10x56) {
        if (_0xdc10x56 >= 1) {
            return 1
        };
        if (_0xdc10x56 <= 0) {
            return 0
        };
        if (_0xdc10x3.pulseNormalize == 1) {
            _0xdc10x3.pulseNormalize /= _0xdc10x7b(1)
        };
        return _0xdc10x7b(_0xdc10x56)
    }
    var _0xdc10x80 = /chrome/i.test(window.navigator.userAgent);
    var _0xdc10x81 = null;
    if ("onwheel" in document.createElement("div")) {
        _0xdc10x81 = "wheel"
    } else {
        if ("onmousewheel" in document.createElement("div")) {
            _0xdc10x81 = "mousewheel"
        }
    };
    if (_0xdc10x81 && _0xdc10x80) {
        _0xdc10x6b(_0xdc10x81, _0xdc10x57);
        _0xdc10x6b("mousedown", _0xdc10x62);
        _0xdc10x6b("load", _0xdc10xa)
    }
})();
(function (_0xdc10x1f) {
    _0xdc10x1f.fn.replaceText = function (_0xdc10x21, _0xdc10x26, _0xdc10x2d) {
        return this.each(function () {
            var _0xdc10x2e = this.firstChild,
                s, o, u = [];
            if (_0xdc10x2e) {
                do {
                    if (_0xdc10x2e.nodeType === 3) {
                        s = _0xdc10x2e.nodeValue;
                        o = s.replace(_0xdc10x21, _0xdc10x26);
                        if (o !== s) {
                            if (!_0xdc10x2d && /</.test(o)) {
                                _0xdc10x1f(_0xdc10x2e).before(o);
                                u.push(_0xdc10x2e)
                            } else {
                                _0xdc10x2e.nodeValue = o
                            }
                        }
                    }
                } while (_0xdc10x2e = _0xdc10x2e.nextSibling);
            };
            u.length && _0xdc10x1f(u).remove()
        })
    }
})(jQuery);
var recentp = "[recent]";
var randomp = "[random]";
var rc = "[recent-comments]";
var s = "[full-width]";
var o = "[left-sidebar]";
var u = "[right-sidebar]";
var c = "[contact-form]";
var li = "[line]";
var fa = "[favorite]";
$(".post *").replaceText(s, "<style>#content-wrapper{width:100% !important;float:none!important;}.post-footer-line>* {margin-right: 0 !important;}#sidebar-wrapper{display:none;}</style>");
$(".post-body *").replaceText(o, "<style>#content-wrapper{float:right!important;}#sidebar-wrapper{float:left!important;}}</style>");
$(".post-body *").replaceText(u, "<style>#content-wrapper{float:left!important;}#sidebar-wrapper{float:right!important;}}</style>");
$(".post-body *").replaceText(c, "<div class='blogger-items-contact'></div>");
$(".post-body *").replaceText(li, "<div class='line'></div>");
$(".sidebar *, .footer *").replaceText(recentp, "<div id='recent-posts'></div>");
$(".sidebar *, .footer *").replaceText(randomp, "<div id='random-posts'></div>");
$(".sidebar *, .footer *").replaceText(rc, "<div id='recent-comments'></div>");
$(".post-body *").replaceText(fa, "<style>.post-cover-thumb{display: block !important;}</style>");
$.ajax({
    url: "/feeds/posts/default?alt=json-in-script&max-results=4&callback=?",
    type: "get",
    dataType: "jsonp",
    success: function (_0xdc10x87) {
        var _0xdc10x88 = "";
        var _0xdc10x89 = "<ul>";
        for (var _0xdc10x2e = 0; _0xdc10x2e < _0xdc10x87.feed.entry.length; _0xdc10x2e++) {
            for (var _0xdc10x8a = 0; _0xdc10x8a < _0xdc10x87.feed.entry[_0xdc10x2e].link.length; _0xdc10x8a++) {
                if (_0xdc10x87.feed.entry[_0xdc10x2e].link[_0xdc10x8a].rel == "alternate") {
                    _0xdc10x88 = _0xdc10x87.feed.entry[_0xdc10x2e].link[_0xdc10x8a].href;
                    break
                }
            };
            var _0xdc10x8b = _0xdc10x87.feed.entry[_0xdc10x2e].title["$t"];
            var _0xdc10x8c = " ";
            var _0xdc10x8d = _0xdc10x87.feed.entry[_0xdc10x2e].published["$t"];
            var _0xdc10x8e = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12];
            var _0xdc10x8f = ["يناير", "فبراير", "مارس", "أبريل", "مايو", "يونيو", " يوليو", " أغسطس", "سبتمبر", "أكتوبر", "نوفمبر", " ديسمبر"];
            var _0xdc10x90 = _0xdc10x8d.split("-")[2].substring(0, 2);
            var _0xdc10x29 = _0xdc10x8d.split("-")[1];
            var _0xdc10x91 = _0xdc10x8d.split("-")[0];
            for (var _0xdc10x92 = 0; _0xdc10x92 < _0xdc10x8e.length; _0xdc10x92++) {
                if (parseInt(_0xdc10x29) == _0xdc10x8e[_0xdc10x92]) {
                    _0xdc10x29 = _0xdc10x8f[_0xdc10x92];
                    break
                }
            };
            _0xdc10x8d = _0xdc10x29 + " " + _0xdc10x90 + ", " + _0xdc10x91;
            try {
                _0xdc10x8c = _0xdc10x87.feed.entry[_0xdc10x2e]["media$thumbnail"].url
            } catch (nl) {
                _0xdc10x8c = "http://4.bp.blogspot.com/-OI0BoYP677M/VZu1TW7a3DI/AAAAAAAAFsE/4BRdE2YFS5A/s1600/noimg.png"
            };
            _0xdc10x89 += "<li><div class=\"recent-outer\"><div class=\"recent-thumb\"><a href=\"" + _0xdc10x88 + "\"><img src=\"" + _0xdc10x8c.replace("/s72-c/", "/w85-h75-p-k-nu/") + "\"/></a></div><div class=\"recent-content\"><div class=\"recent-title\"><a href=\"" + _0xdc10x88 + "\">" + _0xdc10x8b + "</a></div><span>" + _0xdc10x8d + "</span></div></div></li>"
        };
        _0xdc10x89 += "</ul>";
        document.getElementById("recent-posts").innerHTML = _0xdc10x89
    }
});
$.ajax({
    url: "/feeds/comments/default?alt=json-in-script&max-results=4",
    type: "get",
    dataType: "jsonp",
    success: function (_0xdc10x87) {
        var _0xdc10x88 = "";
        var _0xdc10x89 = "<ul>";
        for (var _0xdc10x2e = 0; _0xdc10x2e < _0xdc10x87.feed.entry.length; _0xdc10x2e++) {
            for (var _0xdc10x8a = 0; _0xdc10x8a < _0xdc10x87.feed.entry[_0xdc10x2e].link.length; _0xdc10x8a++) {
                if (_0xdc10x87.feed.entry[_0xdc10x2e].link[_0xdc10x8a].rel == "alternate") {
                    _0xdc10x88 = _0xdc10x87.feed.entry[_0xdc10x2e].link[_0xdc10x8a].href;
                    break
                }
            };
            var _0xdc10x8b = _0xdc10x87.feed.entry[_0xdc10x2e].title["$t"];
            var _0xdc10x93 = _0xdc10x87.feed.entry[_0xdc10x2e].author[0].name["$t"];
            var _0xdc10x94 = _0xdc10x87.feed.entry[_0xdc10x2e].author[0]["gd$image"].src;
            if ("content" in _0xdc10x87.feed.entry[_0xdc10x2e]) {
                var _0xdc10x95 = _0xdc10x87.feed.entry[_0xdc10x2e].content["$t"]
            } else {
                if ("summary" in b_rc) {
                    var _0xdc10x95 = _0xdc10x87.feed.entry[_0xdc10x2e].summary["$t"]
                } else {
                    var _0xdc10x95 = ""
                }
            };
            var _0xdc10x96 = /<\S[^>]*>/g;
            _0xdc10x95 = _0xdc10x95.replace(_0xdc10x96, "");
            if (_0xdc10x95.length > 90) {
                _0xdc10x95 = "" + _0xdc10x95.substring(0, 70) + "..."
            };
            if (_0xdc10x94.match("http://img1.blogblog.com/img/blank.gif")) {
                var _0xdc10x97 = "<div class=\"avatar-comments-image\"><img src=\"http://i.imgur.com/EUs1nSg.png\"/></div>"
            } else {
                if (_0xdc10x94.match("http://img2.blogblog.com/img/b16-rounded.gif")) {
                    var _0xdc10x97 = "<div class=\"avatar-comments-image\"><img src=\"http://i.imgur.com/EUs1nSg.png\"/></div>"
                } else {
                    var _0xdc10x97 = "<div class=\"avatar-comments-image\"><img src=\"" + _0xdc10x94.replace("/s512-c/", "/s75-c/") + "\"/></div>"
                }
            };
            _0xdc10x89 += "<li><div class=\"recent-outer\"><div class=\"recent-thumb\"><a href=\"" + _0xdc10x88 + "\">" + _0xdc10x97 + "</div><div class=\"recent-content\"><div class=\"recent-title\"><a href=\"" + _0xdc10x88 + "\"><i class=\"lnr lnr-user\" aria-hidden=\"true\"></i>" + _0xdc10x93 + "</a></div><span class=\"comment-content\">" + _0xdc10x95 + "</span></div></div></li>"
        };
        _0xdc10x89 += "</ul>";
        document.getElementById("recent-comments").innerHTML = _0xdc10x89
    }
});
$(document).ready(function () {
    var _0xdc10x98 = new Swiper(".swiper-container", {
        nextButton: ".swiper-button-next",
        prevButton: ".swiper-button-prev",
        loop: true,
        speed: 1000,
        effect: "slide",
        slidesPerView: 1,
        paginationClickable: true,
        spaceBetween: 0,
        centeredSlides: true,
        autoplay: 3000,
        autoplayDisableOnInteraction: false
    })
});
$(document).ready(function () {
    var _0xdc10x98 = new Swiper(".swiper-container-2", {
        nextButton: ".swiper-button-next-2",
        prevButton: ".swiper-button-prev-2",
        loop: true,
        speed: 1000,
        effect: "slide",
        slidesPerView: 4,
        spaceBetween: 10,
        autoplay: 3000,
        autoplayDisableOnInteraction: false,
        breakpoints: {
            768: {
                slidesPerView: 2,
                spaceBetween: 10
            },
            640: {
                slidesPerView: 1,
                spaceBetween: 10
            },
            320: {
                slidesPerView: 1,
                spaceBetween: 10
            }
        }
    })
});
$(document).ready(function () {
    selectnav("nav1");
    selectnav("nav2");
    selectnav("nav3")
});
jQuery(document).ready(function () {
    jQuery("#sidebar-wrapper").theiaStickySidebar({
        additionalMarginTop: 20,
        additionalMarginBottom: 20
    })
});
var scrollbtn = $("#scroll-top");
$(window).scroll(function () {
    $(this).scrollTop() >= 700 ? scrollbtn.show() : scrollbtn.hide()
});
scrollbtn.click(function () {
    $("html,body").animate({
        scrollTop: 0
    }, 600)
});
$(".search-btn a, .fixed-search").click(function () {
    return $(".search-box-overlay").addClass("search-box-overlay-show"), !1
}), $(".search-box-close").click(function () {
    return $(".search-box-overlay").removeClass("search-box-overlay-show"), !1
}), $(document).click(function (_0xdc10x1f) {
    return $(_0xdc10x1f.target).closest(".search-box-wrapper").length > 0 ? !0 : void(($(".search-box-overlay").removeClass("search-box-overlay-show")))
});
$(document).ready(function () {
    $(".post-outer-andalus").each(function () {
        var _0xdc10x21 = $(this),
            _0xdc10x2e = _0xdc10x21.find(".post-url").attr("data-url");
        $.get(_0xdc10x2e, function (_0xdc10x2e) {
            $(_0xdc10x2e).find(".post-body iframe[src*=\"youtube.com\"]").length && _0xdc10x21.find(".post-thumb").after("<div class=\"post-format\"><i id=\"youtube-icon\" class=\"fa fa-play\"></i></div>"), $(_0xdc10x2e).find(".post-body iframe[src*=\"google.com/maps\"]").length && _0xdc10x21.find(".post-thumb").after("<div class=\"post-format\"><i id=\"map-icon\" class=\"fa fa-map-marker\"></i></div>"), $(_0xdc10x2e).find(".post-body iframe[src*=\"player.vimeo.com\"]").length && _0xdc10x21.find(".post-thumb").after("<div class=\"post-format\"><i id=\"vi\" class=\"fa fa-vimeo-square\"></i><div>"), $(_0xdc10x2e).find(".post-body iframe[src*=\"w.soundcloud.com\"]").length && _0xdc10x21.find(".post-thumb").after("<div class=\"post-format\"><i id=\"su\" class=\"fa fa-soundcloud\"></i></div>"), $(_0xdc10x2e).find(".post-body .twitter-tweet").length && (_0xdc10x21.find(".post-thumb").after("<div class=\"post-format\"><i id=\"tw\" class=\"fa fa-twitter\"></i></div>"), _0xdc10x21.find(".post-type-twitter").html($(_0xdc10x2e).find(".post-body .twitter-tweet")))
        }, "html")
    })
}), ! function (_0xdc10x21) {
    _0xdc10x21(".data-snippet").each(function () {
        var _0xdc10x31 = _0xdc10x21(this);
        _0xdc10x21("body").hasClass("blog-classic") ? _0xdc10x21.get(_0xdc10x31.attr("data-post"), function (_0xdc10x1f) {
            _0xdc10x31.html("<span>" + _0xdc10x21(_0xdc10x1f).find(".post-body").text().substr(0, 350) + " ...</span>")
        }, "html") : _0xdc10x21.get(_0xdc10x31.attr("data-post"), function (_0xdc10x1f) {
            _0xdc10x31.html("<span>" + _0xdc10x21(_0xdc10x1f).find(".post-body").text().substr(0, 350) + " ...</span>")
        }, "html")
    })
}(jQuery), $(".post-thumb a").attr("style", function (_0xdc10x21, _0xdc10x31) {
    return _0xdc10x31.replace("/s72-c", "/s1600")
});
$(document).ready(function () {
    (function (_0xdc10x1f) {
        var _0xdc10x21 = _0xdc10x1f("a.newer-link");
        var _0xdc10x26 = _0xdc10x1f("a.older-link");
        _0xdc10x1f.get(_0xdc10x21.attr("href"), function (_0xdc10x26) {
            _0xdc10x21.html(" <strong> المقال التالي <i class=\"lnr lnr-arrow-right\"></i></strong><br/><div class=\"post-pager-title\"><span>" + _0xdc10x1f(_0xdc10x26).find(".post .post-title").text() + "</span></div>")
        }, "html");
        _0xdc10x1f.get(_0xdc10x26.attr("href"), function (_0xdc10x21) {
            _0xdc10x26.html("<strong><i class=\"lnr lnr-arrow-left\"></i> المقال السابق </strong><br/><div class=\"post-pager-title\"><span>" + _0xdc10x1f(_0xdc10x21).find(".post .post-title").text() + "</span></div>")
        }, "html")
    })(jQuery)
});
$(".post-thumb a").attr("style", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("/s72-c", "/s1600")
});
$(".post-thumb a").attr("style", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("/default.jpg", "/hqdefault.jpg")
});
$(".slider_thumb").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("s72-c", "s1600")
});
$(".slider_thumb").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("default.jpg", "mqdefault.jpg")
});
$(".post-cover-thumb img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("w72-h72", "w345-h180")
});
$(".post-cover-thumb img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("/default.jpg", "/hqdefault.jpg")
});
$(".PopularPosts img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("w72-h72", "w345-h180")
});
$(".related-item img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("/default.jpg", "/hqdefault.jpg")
});
$(".related-thumbnail img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("/default.jpg", "/hqdefault.jpg")
});
$(".avatar-image-container img").attr("src", function (_0xdc10x2e, _0xdc10x9a) {
    return _0xdc10x9a.replace("//img1.blogblog.com/img/blank.gif", "//3.bp.blogspot.com/-fgwrcZWeRrU/V26tvNcGtsI/AAAAAAAAAG4/lGwGnQDZsNY7bAPr8hVorZruD-jHHxxOgCLcB/s50/anonyme.png")
});
$(".sidebar .widget h2").wrap("<div class='widget-title'/>");
$(".ContactForm").appendTo(".blogger-items-contact");
$(".popular-posts li").each(function () {
    $(this).find(".item-title, .item-snippet").wrapAll("<div class=\"item-caption\" />")
});
$(document).ready(function () {
    $(document).on("click", ".whatsapp-send", function () {
        if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
            var _0xdc10x9b = $(this).attr("data-text");
            var _0xdc10x9c = $(this).attr("data-href");
            var _0xdc10x9d = encodeURIComponent(_0xdc10x9b) + " - " + encodeURIComponent(_0xdc10x9c);
            var _0xdc10x9e = "whatsapp://send?text=" + _0xdc10x9d;
            window.location.href = _0xdc10x9e
        } else {
            $(".error-message").fadeIn(500).delay(3500);
            $(".error-message").fadeOut("slow")
        }
    })
});
$(".social-counter").each(function () {
    var _0xdc10x1f = $(this);
    var _0xdc10x21 = $(this).find(".social-item");
    if (_0xdc10x21.length === 0) {
        _0xdc10x1f.remove()
    };
    $(this).find(".widget").removeClass("LinkList");
    $(".social-counter .social-item.facebook").find(".item-text").text("معجب");
    $(".social-counter .social-item.rss,.social-counter .social-item.youtube").find(".item-text").text("مشترك");
    var _0xdc10x26 = "[";
    var _0xdc10x2d = "]";
    $(".social-counter *").replaceText(_0xdc10x26, "<span class=\"item-count\">");
    $(".social-counter *").replaceText(_0xdc10x2d, "</span>");
    $(".social-item").each(function () {
        var _0xdc10x1f = $(this).find(".remove-count");
        var _0xdc10x21 = $(this).find(".item-count");
        $(_0xdc10x1f).before($(_0xdc10x21));
        $(_0xdc10x1f).remove()
    })
});
$(".widget-content").each(function () {
    var _0xdc10x1f = $(this).text();
    if (_0xdc10x1f.substr(0, 10).match("fbbox")) {
        _0xdc10x1f = _0xdc10x1f.replace("fbbox/", "");
        $(this).html("<iframe allowtransparency=\"true\" frameborder=\"0\" scrolling=\"no\" src=\"//www.facebook.com/plugins/likebox.php?href=" + _0xdc10x1f + "&width=340px&height=258&colorscheme=light&show_faces=true&header=false&stream=false&show_border=false&appId=492409184153294\" style=\"border:none; overflow:hidden; width:100%; height:230px;\"></iframe>")
    }
})

//]]>
