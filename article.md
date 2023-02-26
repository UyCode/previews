# JavaScript ھەققىدە

بىز JavaScript نىڭ  ئالاھىدىلىكىنى، ئۇنىڭ بىلەن نېمىلەرنى ئەمەلگە ئاشۇرالايدىغانلىقىمىزنى ۋە باشقا قايسى تېخنىكىلارنىڭ ئۇنىڭ بىلەن ياخشى ئوينايدىغانلىقىنى كۆرۈپ باقايلى.

## JavaScript دىگەن نىمە؟

*JavaScript* دەسلەپتە «تور بەتلەرنى جانلاندۇرۇش» ئۈچۈن قۇرۇلغان.

بۇ تىلدىكى پروگراممىلار *scripts* دەپ ئاتىلىدۇ. ئۇلار تور بەتنىڭ HTML ئىچىدە  يېزىلىپ، بەت يۈكلەنگەندە ئاپتوماتىك ئىجرا بولالايدۇ.

Scriptلار ئادەتتىكى تېكىست يىزىق شەكلىدە تەمىنلىنىدۇ ۋە ئىجرا قىلىنىدۇ. ئۇلار ئېجرا بولۇش ئۈچۈن ئالاھىدە مۇھىت تەييارلىقى ياكى ئالدىن «تەرجىمە» قىلىشقا مۇھتاج ئەمەس.

بۇ جەھەتتە JavaScript بولسا [Java](https://en.wikipedia.org/wiki/Java_programming_language) بىلەن ئىنتايىن پەرىقلىنىدۇ

> JavaScript قۇرۇلغاندا دەسلەپكى قەدەمدە يەنە بىر ئىسمى بار ئىدى: `LiveScript`. لېكىن ئەينى ۋاقىتتا Java ناھايىتى ئالقىشقا ئېرىشكەن، شۇڭا يېڭى بىر تىلنى Java نىڭ «كىچىك ئىنىسى» قىلىپ بېكىتىشنى قارار قىلىنغان.
>
> ئەمما ئۇنىڭ تەرەققىي قىلىشىغا ئەگىشىپ JavaScript ئۆزىنىڭ خاسلىقى [ECMAScript](http://en.wikipedia.org/wiki/ECMAScript) دەپ ئاتىلىدىغان تولۇق مۇستەقىل تىلغا ئايلاندى، ھازىر ئۇنىڭ Java بىلەن ئازراقمۇ مۇناسىۋىتى يوق.



بۈگۈن JavaScript تور كۆرگۈچتىلا ئەمەس، بەلكى مۇلازىمىتېردامۇ ئىجرا بولالايدۇ، ياكى ئەمەلىيەتتە [JavaScript ماتورى](https://en.wikipedia.org/wiki/JavaScript_engine) دەپ ئاتىلىدىغان ئالاھىدە پىروگرامما بار ھەرقانداق ئۈسكۈنىدە ئىجرا بولالايدۇ.

تور كۆرگۈچتە «JavaScript مەۋھۇم ماشىنىسى» دەپ ئاتىلىدىغان بىر خىل قىستۇرما ھالەتتىكى گىرەلەشتۈرۋىتىلگەن ماتور بار.

ئوخشىمىغان ماتورلارنىڭ ئوخشىمىغان «كود نامى» بار. مەسلەن:

-  Chrome, Opera ياكى Edge دا – [V8](https://en.wikipedia.org/wiki/V8_JavaScript_engine)
- Firefox دا – [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey)
- IE ئۈچۈن "چاكرا"، سافارى ( Safari ) ئۈچۈن "JavaScriptCore", "Nitro" ياكى "SquirrelFish" دىگەندەك

يۇقارقى ئاتالغۇلارنى ئەستە ساقلاش ئاسان، چۈنكى توردىكى ئاچقۇچىلار يېتەكچى ماتىرياللىرىدا كوپ ئىشلىتىلىدۇ. بىزمۇ ئۇلارنى ئىشلىتىمىز. مەسىلەن، ئەگەر «بىر ئىقتىدار X نى V8 قوللىغان» بولسا، بەلكىم Chrome، Opera ۋە Edge دا ئىشلىشى مۇمكىن.



> ماتور مۇرەككەپ. ئەمما ئاساسىي ئىشلار ئاسان.
>
> 1. ماتور (ئەگەر تور كۆرگۈچ بولسا ئاللىبۇرۇن تەييار) ئاۋۋال Script نى ئوقۇپ يېشىدۇ.
> 2. ئاندىن ماتور ئۇنى ماشىنا كودىغا ئايلاندۇرىدۇ (تەرجىمە قىلىدۇ).
> 3. ئاندىن ماشىنا كودى خېلى تىز سۈرئەتتە ئېجرا بولىدۇ.
>
> ماتور بۇ جەرياننىڭ ھەر بىر قەدىمىدە ئەلالاشتۇرۇش ئىلىپ بارىدۇ. ئۇ ھەتتا ماشىنا كودىغا تەرجىمە قىلىنغان Script ئېجىرا بولۇش جەريانىدا كۆزىتىش ئىلىپ بىرىپ، ئۇنىڭدا ئىشلەتكەن سانلىق مەلۇماتلارنى تەھلىل قىلىپ، ھەم شۇ بىلىملەرگە ئاساسەن ماشىنا كودىنى يەنىمۇ ئەلالاشتۇرىدۇ.



```smart header="How do engines work?"

ماتور مۇرەككەپ. ئەمما ئاساسىي ئىشلار ئاسان.

1. ماتور (ئەگەر تور كۆرگۈچ بولسا ئاللىبۇرۇن تەييار) ئاۋۋال Script نى ئوقۇپ يېشىدۇ.
2. ئاندىن ماتور ئۇنى ماشىنا كودىغا ئايلاندۇرىدۇ (تەرجىمە قىلىدۇ).
3. ئاندىن ماشىنا كودى خېلى تىز سۈرئەتتە ئېجرا بولىدۇ.

ماتور بۇ جەرياننىڭ ھەر بىر قەدىمىدە ئەلالاشتۇرۇش ئىلىپ بارىدۇ. ئۇ ھەتتا ماشىنا كودىغا تەرجىمە قىلىنغان Script ئېجىرا بولۇش جەريانىدا كۆزىتىش ئىلىپ بىرىپ، ئۇنىڭدا ئىشلەتكەن سانلىق مەلۇماتلارنى تەھلىل قىلىپ، ھەم شۇ بىلىملەرگە ئاساسەن ماشىنا كودىنى يەنىمۇ ئەلالاشتۇرىدۇ.
```

## What can in-browser JavaScript do?

Modern JavaScript is a "safe" programming language. It does not provide low-level access to memory or the CPU, because it was initially created for browsers which do not require it.

JavaScript's capabilities greatly depend on the environment it's running in. For instance, [Node.js](https://wikipedia.org/wiki/Node.js) supports functions that allow JavaScript to read/write arbitrary files, perform network requests, etc.

In-browser JavaScript can do everything related to webpage manipulation, interaction with the user, and the webserver.

For instance, in-browser JavaScript is able to:

- Add new HTML to the page, change the existing content, modify styles.
- React to user actions, run on mouse clicks, pointer movements, key presses.
- Send requests over the network to remote servers, download and upload files (so-called [AJAX](https://en.wikipedia.org/wiki/Ajax_(programming)) and [COMET](https://en.wikipedia.org/wiki/Comet_(programming)) technologies).
- Get and set cookies, ask questions to the visitor, show messages.
- Remember the data on the client-side ("local storage").

## What CAN'T in-browser JavaScript do?

JavaScript's abilities in the browser are limited to protect the user's safety. The aim is to prevent an evil webpage from accessing private information or harming the user's data.

Examples of such restrictions include:

- JavaScript on a webpage may not read/write arbitrary files on the hard disk, copy them or execute programs. It has no direct access to OS functions.

    Modern browsers allow it to work with files, but the access is limited and only provided if the user does certain actions, like "dropping" a file into a browser window or selecting it via an `<input>` tag.

    There are ways to interact with the camera/microphone and other devices, but they require a user's explicit permission. So a JavaScript-enabled page may not sneakily enable a web-camera, observe the surroundings and send the information to the [NSA](https://en.wikipedia.org/wiki/National_Security_Agency).
- Different tabs/windows generally do not know about each other. Sometimes they do, for example when one window uses JavaScript to open the other one. But even in this case, JavaScript from one page may not access the other page if they come from different sites (from a different domain, protocol or port).

    This is called the "Same Origin Policy". To work around that, *both pages* must agree for data exchange and must contain special JavaScript code that handles it. We'll cover that in the tutorial.

    This limitation is, again, for the user's safety. A page from `http://anysite.com` which a user has opened must not be able to access another browser tab with the URL `http://gmail.com`, for example, and steal information from there.
- JavaScript can easily communicate over the net to the server where the current page came from. But its ability to receive data from other sites/domains is crippled. Though possible, it requires explicit agreement (expressed in HTTP headers) from the remote side. Once again, that's a safety limitation.

![](limitations.svg)

Such limitations do not exist if JavaScript is used outside of the browser, for example on a server. Modern browsers also allow plugins/extensions which may ask for extended permissions.

## What makes JavaScript unique?

There are at least *three* great things about JavaScript:

```compare
+ Full integration with HTML/CSS.
+ Simple things are done simply.
+ Supported by all major browsers and enabled by default.
```
JavaScript is the only browser technology that combines these three things.

That's what makes JavaScript unique. That's why it's the most widespread tool for creating browser interfaces.

That said, JavaScript can be used to create servers, mobile applications, etc.

## Languages "over" JavaScript

The syntax of JavaScript does not suit everyone's needs. Different people want different features.

That's to be expected, because projects and requirements are different for everyone.

So, recently a plethora of new languages appeared, which are *transpiled* (converted) to JavaScript before they run in the browser.

Modern tools make the transpilation very fast and transparent, actually allowing developers to code in another language and auto-converting it "under the hood".

Examples of such languages:

- [CoffeeScript](https://coffeescript.org/) is "syntactic sugar" for JavaScript. It introduces shorter syntax, allowing us to write clearer and more precise code. Usually, Ruby devs like it.
- [TypeScript](https://www.typescriptlang.org/) is concentrated on adding "strict data typing" to simplify the development and support of complex systems. It is developed by Microsoft.
- [Flow](https://flow.org/) also adds data typing, but in a different way. Developed by Facebook.
- [Dart](https://www.dartlang.org/) is a standalone language that has its own engine that runs in non-browser environments (like mobile apps), but also can be transpiled to JavaScript. Developed by Google.
- [Brython](https://brython.info/) is a Python transpiler to JavaScript that enables the writing of applications in pure Python without JavaScript.
- [Kotlin](https://kotlinlang.org/docs/reference/js-overview.html) is a modern, concise and safe programming language that can target the browser or Node.

There are more. Of course, even if we use one of these transpiled languages, we should also know JavaScript to really understand what we're doing.

## Summary

- JavaScript was initially created as a browser-only language, but it is now used in many other environments as well.
- Today, JavaScript has a unique position as the most widely-adopted browser language, fully integrated with HTML/CSS.
- There are many languages that get "transpiled" to JavaScript and provide certain features. It is recommended to take a look at them, at least briefly, after mastering JavaScript.
