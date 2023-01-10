[![Badge Commits]][commit rate]
[![Badge Issues]][issues]
[![Badge Localization]][crowdin]
[![Badge License]][license]
[![Badge NPM]][npm]
[![Badge Mozilla]][mozilla]
[![Badge Chrome]][chrome]

---

<h1 align="center">
<sub>
<img src="https://github.com/gorhill/uBlock/blob/master/src/img/ublock.svg" height="38" width="38">
</sub>
uBlock Origin (uBO)
</h1>
<p align="center">
<sub><a href="https://github.com/gorhill/uBlock/wiki/uBlock-Origin-is-completely-unrelated-to-the-web-site-ublock.org"><b>BEWARE!</b> uBO is (and has always been) COMPLETELY UNRELATED to the website <code>ublock.org</code></a>.</sub>
</p>

---

<p align="center">
<a href="https://addons.mozilla.org/addon/ublock-origin/"><img src="https://user-images.githubusercontent.com/585534/107280546-7b9b2a00-6a26-11eb-8f9f-f95932f4bfec.png" alt="Get uBlock Origin for Firefox"></a>
<a href="https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm"><img src="https://user-images.githubusercontent.com/585534/107280622-91a8ea80-6a26-11eb-8d07-77c548b28665.png" alt="Get uBlock Origin for Chromium"></a>
<a href="https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak"><img src="https://user-images.githubusercontent.com/585534/107280673-a5ece780-6a26-11eb-9cc7-9fa9f9f81180.png" alt="Get uBlock Origin for Microsoft Edge"></a>
<a href="https://addons.opera.com/extensions/details/ublock/"><img src="https://user-images.githubusercontent.com/585534/107280692-ac7b5f00-6a26-11eb-85c7-088926504452.png" alt="Get uBlock Origin for Opera"></a>
</p>

---

uBO is **NOT** an "ad blocker";(uBO **BUKANLAH** sebuah "adblocker") it is a [wide-spectrum content blocker][blocking] for Chromium and Firefox with CPU and memory efficiency as primary features. After a new installation, the default behavior of uBO is to block ads, trackers, and malware sites through [EasyList][easylist], [EasyPrivacy][easyprivacy], [Peter Lowe's Blocklist][peter lowe's blocklist], [Online Malicious URL Blocklist][malicious blocklist], and uBO's [filter lists][ubo filters].

---

- [Documentation](#documentation)
- [General Information](#general-information)
- [Installation](#installation)
  - [Chromium](#chromium)
  - [Firefox / Firefox for Android](#firefox--firefox-for-android)
- [Release History](#release-history)
- [About](#about)
- [License](#license)
- [Privacy Policy]
- [Wiki](https://github.com/gorhill/uBlock/wiki)

## Documentation

|                                                                                                         Basic mode                                                                                                          |                                                                                                                                                   Advanced-user mode                                                                                                                                                    |
| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                                                                   [Popup user interface]                                                                                                    |                                                                                                                 [A point-and-click firewall that is configurable on a per-site basis][dynamic filters]                                                                                                                  |
| <a href="https://github.com/gorhill/uBlock/wiki/Quick-guide:-popup-user-interface"><img src="https://user-images.githubusercontent.com/585534/84045360-b10ee580-a976-11ea-9e91-29c2107b47c2.png"/></a><br><sup>.<br>.</sup> | <a href="https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide"><img src="https://user-images.githubusercontent.com/585534/84045366-b1a77c00-a976-11ea-9121-e8c8f35c66c8.png"/></a><br><sup>Configure as you wish.<br>The image shows 3rd-party scripts and frames blocked by default everywhere.</sup> |

Visit the [wiki][wiki] for documentation.

For support, questions, or help, visit [/r/uBlockOrigin][reddit].

## General Information

uBO is **NOT** an "ad blocker"; it is a wide-spectrum content blocker. uBO blocks ads through the EasyList filter syntax and [extends][extended syntax] the syntax to work with custom rules and filters. Furthermore, the advanced mode allows uBO to work in [default-deny mode][default deny], which will cause [all 3rd-party network requests][3rd party requests] to be blocked by default unless allowed by the user.

It is important to note that using a blocker is **NOT** [theft]. Do not fall for this creepy idea. The _ultimate_ logical consequence of `blocking = theft` is the criminalization of the inalienable right to privacy.

Ads, "unintrusive" or not, are just the visible portion of the privacy-invading means entering your browser when you visit most sites. **uBO's primary goal is to help users neutralize these privacy-invading methods** in a way that welcomes those users who do not wish to use more technical, involved means (such as [uMatrix]).

EasyList, EasyPrivacy, Peter Lowe's Blocklist, Online Malicious URL Blocklist, and uBO's filter lists are default enabled when you install uBO. Many other lists are available to block trackers, analytics, and more. Hosts files are also supported.

Once you install uBO, you may easily unselect any preselected filter lists if you think uBO blocks too much. For reference, Adblock Plus installs with only EasyList, ABP filters, and Acceptable Ads enabled by default.

## Installation

[Required Permissions][permissions]

#### Chromium

[Chrome Web Store][chrome]

[Microsoft Edge Add-ons][edge] (Published by: [Nicole Rolls][nicole rolls])

[Opera Add-ons][opera]

[Development Build][chrome dev]

uBO should be compatible with any Chromium-based browser.

#### Firefox / Firefox for Android

[Firefox Add-ons][mozilla]

[Development Build][beta]

#### All Browsers

Do **NOT** use any other content blocker concurrently with uBO to benefit from its higher efficiency. uBO will [perform][performance] as well as or better than most of the other popular ad blockers. Other blockers can prevent uBO's privacy or anti-blocker-defusing features from working correctly.

Do **NOT** use uBO along with other [similarly-purposed blockers][similarly-purposed].

[Manual Installation][manual installation]

#### Enterprise Deployment

[Deploying uBO][deployment]

## Release History

[Releases Page][releases]

## About

[Manifesto][manifesto]

Free. Open-source. For users by users. No donations sought.

Without the preset filter lists, this extension is nothing. If you ever want to contribute something, think about the people working hard to maintain the filter lists you are using, which were made available to use by all for free.

You can help contribute by translating uBO on [Crowdin].

## License

[GPLv3][license]

<!----------------------------------------------------------------------------->

[peter lowe's blocklist]: https://pgl.yoyo.org/adservers/
[malicious blocklist]: https://gitlab.com/malware-filter/urlhaus-filter#malicious-url-blocklist
[3rd party requests]: https://requestpolicycontinued.github.io/#what-are-cross-site-requests
[similarly-purposed]: https://twitter.com/gorhill/status/1033706103782170625
[performance]: https://www.debugbear.com/blog/chrome-extension-performance-2021#how-do-ad-blockers-and-privacy-tools-affect-browser-performance
[easyprivacy]: https://easylist.to/#easyprivacy
[chrome dev]: https://chrome.google.com/webstore/detail/ublock-origin-development/cgbcahbpdhpcegmbfconppldiemgcoii
[easylist]: https://easylist.to/#easylist
[mozilla]: https://addons.mozilla.org/addon/ublock-origin/
[crowdin]: https://crowdin.com/project/ublock
[chrome]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm
[reddit]: https://www.reddit.com/r/uBlockOrigin/
[theft]: https://twitter.com/LeaVerou/status/518154828166725632
[opera]: https://addons.opera.com/extensions/details/ublock/
[edge]: https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak
[npm]: https://www.npmjs.com/package/@gorhill/ubo-core
[manifesto]: MANIFESTO.md
[license]: LICENSE.txt
[nicole rolls]: https://github.com/nicole-ashley

<!---------------------------------[ Internal ]-------------------------------->

[popup user interface]: https://github.com/gorhill/uBlock/wiki/Quick-guide:-popup-user-interface
[manual installation]: https://github.com/gorhill/uBlock/tree/master/dist#install
[extended syntax]: https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#extended-syntax
[dynamic filters]: https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide
[privacy policy]: https://github.com/gorhill/uBlock/wiki/Privacy-policy
[default deny]: https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-default-deny
[ubo filters]: https://github.com/uBlockOrigin/uAssets/tree/master/filters
[permissions]: https://github.com/gorhill/uBlock/wiki/Permissions
[commit rate]: https://github.com/gorhill/uBlock/commits/master
[deployment]: https://github.com/gorhill/uBlock/wiki/Deploying-uBlock-Origin
[blocking]: https://github.com/gorhill/uBlock/wiki/Blocking-mode
[releases]: https://github.com/gorhill/uBlock/releases
[umatrix]: https://github.com/gorhill/uMatrix
[issues]: https://github.com/uBlockOrigin/uBlock-issues/issues
[beta]: https://github.com/gorhill/uBlock/blob/master/dist/README.md#for-beta-version
[wiki]: https://github.com/gorhill/uBlock/wiki

<!----------------------------------[ Badges ]--------------------------------->

[badge localization]: https://d322cqt584bo4o.cloudfront.net/ublock/localized.svg
[badge commits]: https://img.shields.io/github/commit-activity/m/gorhill/ublock?label=Commits
[badge mozilla]: https://img.shields.io/amo/rating/ublock-origin?label=Firefox
[badge license]: https://img.shields.io/badge/License-GPLv3-blue.svg
[badge chrome]: https://img.shields.io/chrome-web-store/rating/cjpalhdlnbpafiamejdnhcphjbkeiagm?label=Chrome
[badge issues]: https://img.shields.io/github/issues/uBlockOrigin/uBlock-issues
[badge npm]: https://img.shields.io/npm/v/@gorhill/ubo-core
