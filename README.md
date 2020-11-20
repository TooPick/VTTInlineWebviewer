![GitHub All Releases](https://img.shields.io/github/downloads/ardittristan/VTTInlineWebviewer/total)
[![Donate](https://img.shields.io/badge/Donate-PayPal-Green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=TF3LJHWV9U7HN)

# Inline Webviewer

## Installation

To install, import this [Manifest](https://raw.githubusercontent.com/ardittristan/VTTInlineWebviewer/master/module.json) into your module browser.

Make sure you've also have the [ColorSettings](https://raw.githubusercontent.com/ardittristan/VTTColorSettings/master/module.json) library installed!

## Usage

### As HUD button

You can add new webviews in the settings, for more info on this click the help button on the settings' popup.

All webviews appear on the left HUD under the <a href=""><img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/master/svgs/regular/window-maximize.svg" alt="" height="16" /></a> menu.

### When sending popup as GM

For GMs, a <a href=""><img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/master/svgs/solid/upload.svg" alt="" height="16" /></a> should be visible in the <a href=""><img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/master/svgs/regular/window-maximize.svg" alt="" height="16" /></a> menu. If clicked on, the GM can enter an url. This url will pop up on the screen of all players inside a webviewer.

&nbsp;  
You can also use this in a macro, it functions the same as the popup, but can be called as a function:

```js
/**
 * @param {String} url - webview url
 * @param {Boolean} compat - compatibility mode on or off
 * @param {Number} w - width
 * @param {Number} h - height
 * @param {String} name - title of application
 * @param {String} customCSS - css selectors for elements to be removed, comma seperated
 * @param {String[]} userList - array of user id's to which the webview gets send, if empty it sends to everyone
 */
window.Ardittristan.InlineViewer.sendUrl(url, compat = false, w = 512, h = 512, name, customCSS, userList)
```

## Troubleshooting

* If the site disallows embedding in iframes you can try enabling compatibility mode, compatibility mode might not fully fix the issue and logs domain names to prevent abuse.

## Example

![Preview](https://i.imgur.com/5E36O9u.gif)

## Changelog

Check the [Changelog](https://github.com/ardittristan/VTTInlineWebviewer/blob/master/CHANGELOG.md)
