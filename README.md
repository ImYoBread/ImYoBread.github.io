"use strict";
// This code is licensed under the GPL-2.
// https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html
var __spreadArray = (this && this.__spreadArray) || function (to, from, pack) {
    if (pack || arguments.length === 2) for (var i = 0, l = from.length, ar; i < l; i++) {
        if (ar || !(i in from)) {
            if (!ar) ar = Array.prototype.slice.call(from, 0, i);
            ar[i] = from[i];
        }
    }
    return to.concat(ar || Array.prototype.slice.call(from));
};
// Read the license and USE AT YOUR OWN RISK. It has only been minimally tested.
(function () {
    // Change this to your Amazon tag.
    var myTag = "imyobread-20";
    document.addEventListener("DOMContentLoaded", affiliatize);
    function affiliatize() {
        var links = __spreadArray([], document.querySelectorAll("a[href]"), true);
        for (var i = 0; i < links.length; i++) {
            processLink(links[i]);
        }
    }
    function processLink(link) {
        var u = new URL(link.href);
        if (u.hostname.startsWith("www.amazon.") ||
            u.hostname.startsWith("amazon.")) {
            console.log("u.hostname: ".concat(u.hostname));
            if (!u.searchParams.has("tag")) {
                console.log("adding tag to ".concat(link.href));
                u.searchParams.append("tag", myTag);
                link.href = u.toString();
                console.log("new URL ".concat(link.href));
            }
            else {
                console.log("skipping: URL already contains an Amazon tag: ".concat(link.href));
            }
        }
        else {
            console.log("Not an Amazon link: ".concat(link.href));
        }
        console.log("=======");
    }
