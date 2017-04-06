# api documentation for  [botbuilder (v3.7.0)](https://github.com/Microsoft/BotBuilder#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-botbuilder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-botbuilder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-botbuilder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-botbuilder)
#### Bot Builder is a dialog system for building rich bots on virtually any platform.

[![NPM](https://nodei.co/npm/botbuilder.png?downloads=true)](https://www.npmjs.com/package/botbuilder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-botbuilder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-botbuilder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-botbuilder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-botbuilder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-botbuilder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Microsoft Corp."
    },
    "bugs": {
        "url": "https://github.com/Microsoft/BotBuilder/issues"
    },
    "dependencies": {
        "async": "^1.5.2",
        "base64url": "^1.0.6",
        "chrono-node": "^1.1.3",
        "jsonwebtoken": "^7.0.1",
        "promise": "^7.1.1",
        "request": "^2.69.0",
        "rsa-pem-from-mod-exp": "^0.8.4",
        "sprintf-js": "^1.0.3",
        "url-join": "^1.1.0"
    },
    "description": "Bot Builder is a dialog system for building rich bots on virtually any platform.",
    "devDependencies": {
        "@types/url-join": "^0.8.1",
        "mocha": "^2.4.5"
    },
    "directories": {},
    "dist": {
        "shasum": "6a9c0c9336dddcfc7034d08ea7e8671caf060e6b",
        "tarball": "https://registry.npmjs.org/botbuilder/-/botbuilder-3.7.0.tgz"
    },
    "homepage": "https://github.com/Microsoft/BotBuilder#readme",
    "keywords": [
        "botbuilder",
        "bots",
        "chatbots"
    ],
    "license": "MIT",
    "main": "./lib/botbuilder.js",
    "maintainers": [
        {
            "name": "botframework",
            "email": "botframework@microsoft.com"
        }
    ],
    "name": "botbuilder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Microsoft/BotBuilder.git"
    },
    "scripts": {
        "test": "mocha tests/*.js"
    },
    "typings": "./lib/botbuilder.d.ts",
    "version": "3.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module botbuilder](#apidoc.module.botbuilder)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>AnimationCard (session)](#apidoc.element.botbuilder.AnimationCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>AudioCard (session)](#apidoc.element.botbuilder.AudioCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>BotConnectorBot (options)](#apidoc.element.botbuilder.BotConnectorBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardAction (session)](#apidoc.element.botbuilder.CardAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardImage (session)](#apidoc.element.botbuilder.CardImage)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardMedia (session)](#apidoc.element.botbuilder.CardMedia)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ChatConnector (settings)](#apidoc.element.botbuilder.ChatConnector)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CommandDialog (serviceUri)](#apidoc.element.botbuilder.CommandDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ConsoleConnector ()](#apidoc.element.botbuilder.ConsoleConnector)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Dialog ()](#apidoc.element.botbuilder.Dialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>DialogAction ()](#apidoc.element.botbuilder.DialogAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>EntityRecognizer ()](#apidoc.element.botbuilder.EntityRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Fact (session)](#apidoc.element.botbuilder.Fact)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>HeroCard (session)](#apidoc.element.botbuilder.HeroCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>IntentDialog (options)](#apidoc.element.botbuilder.IntentDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>IntentRecognizerSet (options)](#apidoc.element.botbuilder.IntentRecognizerSet)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Keyboard (session)](#apidoc.element.botbuilder.Keyboard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Library (name)](#apidoc.element.botbuilder.Library)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>LuisDialog (serviceUri)](#apidoc.element.botbuilder.LuisDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>LuisRecognizer (models)](#apidoc.element.botbuilder.LuisRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>MediaCard (session)](#apidoc.element.botbuilder.MediaCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>MemoryBotStorage ()](#apidoc.element.botbuilder.MemoryBotStorage)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Message (session)](#apidoc.element.botbuilder.Message)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Middleware ()](#apidoc.element.botbuilder.Middleware)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Prompts ()](#apidoc.element.botbuilder.Prompts)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptCard (session)](#apidoc.element.botbuilder.ReceiptCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptItem (session)](#apidoc.element.botbuilder.ReceiptItem)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>RegExpRecognizer (intent, expressions)](#apidoc.element.botbuilder.RegExpRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Session (options)](#apidoc.element.botbuilder.Session)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SigninCard (session)](#apidoc.element.botbuilder.SigninCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SimpleDialog (fn)](#apidoc.element.botbuilder.SimpleDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SimplePromptRecognizer ()](#apidoc.element.botbuilder.SimplePromptRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>TextBot (options)](#apidoc.element.botbuilder.TextBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ThumbnailCard (session)](#apidoc.element.botbuilder.ThumbnailCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>UniversalBot (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>VideoCard (session)](#apidoc.element.botbuilder.VideoCard)
1.  object <span class="apidocSignatureSpan">botbuilder.</span>AnimationCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>AttachmentLayout
1.  object <span class="apidocSignatureSpan">botbuilder.</span>AudioCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>BotConnectorBot.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>CardAction.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>CardImage.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>CardMedia.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Channel
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ChatConnector.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>CommandDialog.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ConsoleConnector.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>DefaultLocalizer
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Dialog.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Fact.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>HeroCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>IntentDialog.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>IntentRecognizerSet.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Keyboard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Library.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ListStyle
1.  object <span class="apidocSignatureSpan">botbuilder.</span>LuisDialog.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>LuisRecognizer.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>MediaCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>MemoryBotStorage.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Message.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>PromptType
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Prompts.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ReceiptCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ReceiptItem.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>RecognizeMode
1.  object <span class="apidocSignatureSpan">botbuilder.</span>RecognizeOrder
1.  object <span class="apidocSignatureSpan">botbuilder.</span>RegExpRecognizer.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ResumeReason
1.  object <span class="apidocSignatureSpan">botbuilder.</span>Session.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>SigninCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>SimpleDialog.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>SimplePromptRecognizer.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>TextBot.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>TextFormat
1.  object <span class="apidocSignatureSpan">botbuilder.</span>ThumbnailCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>UniversalBot.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>VideoCard.prototype
1.  object <span class="apidocSignatureSpan">botbuilder.</span>logger
1.  object <span class="apidocSignatureSpan">botbuilder.</span>utils

#### [module botbuilder.AnimationCard](#apidoc.module.botbuilder.AnimationCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>AnimationCard (session)](#apidoc.element.botbuilder.AnimationCard.AnimationCard)

#### [module botbuilder.AnimationCard.prototype](#apidoc.module.botbuilder.AnimationCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.AnimationCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.AnimationCard.prototype.constructor)

#### [module botbuilder.AudioCard](#apidoc.module.botbuilder.AudioCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>AudioCard (session)](#apidoc.element.botbuilder.AudioCard.AudioCard)

#### [module botbuilder.AudioCard.prototype](#apidoc.module.botbuilder.AudioCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.AudioCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.AudioCard.prototype.constructor)

#### [module botbuilder.BotConnectorBot](#apidoc.module.botbuilder.BotConnectorBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>BotConnectorBot (options)](#apidoc.element.botbuilder.BotConnectorBot.BotConnectorBot)

#### [module botbuilder.BotConnectorBot.prototype](#apidoc.module.botbuilder.BotConnectorBot.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>add (id, dialog)](#apidoc.element.botbuilder.BotConnectorBot.prototype.add)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>beginDialog (address, dialogId, dialogArgs)](#apidoc.element.botbuilder.BotConnectorBot.prototype.beginDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>configure (options)](#apidoc.element.botbuilder.BotConnectorBot.prototype.configure)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>listen (dialogId, dialogArgs)](#apidoc.element.botbuilder.BotConnectorBot.prototype.listen)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>on (event, listener)](#apidoc.element.botbuilder.BotConnectorBot.prototype.on)
1.  [function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>verifyBotFramework (options)](#apidoc.element.botbuilder.BotConnectorBot.prototype.verifyBotFramework)

#### [module botbuilder.CardAction](#apidoc.module.botbuilder.CardAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardAction (session)](#apidoc.element.botbuilder.CardAction.CardAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>call (session, number, title)](#apidoc.element.botbuilder.CardAction.call)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>dialogAction (session, action, data, title)](#apidoc.element.botbuilder.CardAction.dialogAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>downloadFile (session, url, title)](#apidoc.element.botbuilder.CardAction.downloadFile)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>imBack (session, msg, title)](#apidoc.element.botbuilder.CardAction.imBack)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>openUrl (session, url, title)](#apidoc.element.botbuilder.CardAction.openUrl)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>playAudio (session, url, title)](#apidoc.element.botbuilder.CardAction.playAudio)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>playVideo (session, url, title)](#apidoc.element.botbuilder.CardAction.playVideo)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>postBack (session, msg, title)](#apidoc.element.botbuilder.CardAction.postBack)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>showImage (session, url, title)](#apidoc.element.botbuilder.CardAction.showImage)

#### [module botbuilder.CardAction.prototype](#apidoc.module.botbuilder.CardAction.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>image (url)](#apidoc.element.botbuilder.CardAction.prototype.image)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>title (text)](#apidoc.element.botbuilder.CardAction.prototype.title)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>toAction ()](#apidoc.element.botbuilder.CardAction.prototype.toAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>type (t)](#apidoc.element.botbuilder.CardAction.prototype.type)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>value (v)](#apidoc.element.botbuilder.CardAction.prototype.value)

#### [module botbuilder.CardImage](#apidoc.module.botbuilder.CardImage)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardImage (session)](#apidoc.element.botbuilder.CardImage.CardImage)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardImage.</span>create (session, url)](#apidoc.element.botbuilder.CardImage.create)

#### [module botbuilder.CardImage.prototype](#apidoc.module.botbuilder.CardImage.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>alt (text)](#apidoc.element.botbuilder.CardImage.prototype.alt)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>tap (action)](#apidoc.element.botbuilder.CardImage.prototype.tap)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>toImage ()](#apidoc.element.botbuilder.CardImage.prototype.toImage)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>url (u)](#apidoc.element.botbuilder.CardImage.prototype.url)

#### [module botbuilder.CardMedia](#apidoc.module.botbuilder.CardMedia)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CardMedia (session)](#apidoc.element.botbuilder.CardMedia.CardMedia)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardMedia.</span>create (session, url)](#apidoc.element.botbuilder.CardMedia.create)

#### [module botbuilder.CardMedia.prototype](#apidoc.module.botbuilder.CardMedia.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>profile (text)](#apidoc.element.botbuilder.CardMedia.prototype.profile)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>toMedia ()](#apidoc.element.botbuilder.CardMedia.prototype.toMedia)
1.  [function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>url (u)](#apidoc.element.botbuilder.CardMedia.prototype.url)

#### [module botbuilder.Channel](#apidoc.module.botbuilder.Channel)
1.  [function <span class="apidocSignatureSpan">botbuilder.Channel.</span>getChannelId (addressable)](#apidoc.element.botbuilder.Channel.getChannelId)
1.  [function <span class="apidocSignatureSpan">botbuilder.Channel.</span>supportsCardActions (session, buttonCnt)](#apidoc.element.botbuilder.Channel.supportsCardActions)
1.  [function <span class="apidocSignatureSpan">botbuilder.Channel.</span>supportsKeyboards (session, buttonCnt)](#apidoc.element.botbuilder.Channel.supportsKeyboards)
1.  object <span class="apidocSignatureSpan">botbuilder.Channel.</span>channels

#### [module botbuilder.ChatConnector](#apidoc.module.botbuilder.ChatConnector)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ChatConnector (settings)](#apidoc.element.botbuilder.ChatConnector.ChatConnector)

#### [module botbuilder.ChatConnector.prototype](#apidoc.module.botbuilder.ChatConnector.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>addAccessToken (options, cb)](#apidoc.element.botbuilder.ChatConnector.prototype.addAccessToken)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>addUserAgent (options)](#apidoc.element.botbuilder.ChatConnector.prototype.addUserAgent)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>authenticatedRequest (options, callback, refresh)](#apidoc.element.botbuilder.ChatConnector.prototype.authenticatedRequest)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>dispatch (msg, res)](#apidoc.element.botbuilder.ChatConnector.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getAccessToken (cb)](#apidoc.element.botbuilder.ChatConnector.prototype.getAccessToken)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getData (context, callback)](#apidoc.element.botbuilder.ChatConnector.prototype.getData)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getStoragePath (address)](#apidoc.element.botbuilder.ChatConnector.prototype.getStoragePath)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>isInvoke (message)](#apidoc.element.botbuilder.ChatConnector.prototype.isInvoke)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>listen ()](#apidoc.element.botbuilder.ChatConnector.prototype.listen)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>onEvent (handler)](#apidoc.element.botbuilder.ChatConnector.prototype.onEvent)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>onInvoke (handler)](#apidoc.element.botbuilder.ChatConnector.prototype.onInvoke)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>postMessage (msg, cb)](#apidoc.element.botbuilder.ChatConnector.prototype.postMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>prepIncomingMessage (msg)](#apidoc.element.botbuilder.ChatConnector.prototype.prepIncomingMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>prepOutgoingMessage (msg)](#apidoc.element.botbuilder.ChatConnector.prototype.prepOutgoingMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>saveData (context, data, callback)](#apidoc.element.botbuilder.ChatConnector.prototype.saveData)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.ChatConnector.prototype.send)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>startConversation (address, done)](#apidoc.element.botbuilder.ChatConnector.prototype.startConversation)
1.  [function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>verifyBotFramework (req, res)](#apidoc.element.botbuilder.ChatConnector.prototype.verifyBotFramework)

#### [module botbuilder.CommandDialog](#apidoc.module.botbuilder.CommandDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>CommandDialog (serviceUri)](#apidoc.element.botbuilder.CommandDialog.CommandDialog)

#### [module botbuilder.CommandDialog.prototype](#apidoc.module.botbuilder.CommandDialog.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.CommandDialog.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>constructor (serviceUri)](#apidoc.element.botbuilder.CommandDialog.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.CommandDialog.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>matches (patterns, dialogId, dialogArgs)](#apidoc.element.botbuilder.CommandDialog.prototype.matches)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.CommandDialog.prototype.onBegin)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.CommandDialog.prototype.onDefault)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.CommandDialog.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.CommandDialog.prototype.replyReceived)

#### [module botbuilder.ConsoleConnector](#apidoc.module.botbuilder.ConsoleConnector)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ConsoleConnector ()](#apidoc.element.botbuilder.ConsoleConnector.ConsoleConnector)

#### [module botbuilder.ConsoleConnector.prototype](#apidoc.module.botbuilder.ConsoleConnector.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>listen ()](#apidoc.element.botbuilder.ConsoleConnector.prototype.listen)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>onEvent (handler)](#apidoc.element.botbuilder.ConsoleConnector.prototype.onEvent)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>onInvoke (handler)](#apidoc.element.botbuilder.ConsoleConnector.prototype.onInvoke)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>processMessage (line)](#apidoc.element.botbuilder.ConsoleConnector.prototype.processMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.ConsoleConnector.prototype.send)
1.  [function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>startConversation (address, cb)](#apidoc.element.botbuilder.ConsoleConnector.prototype.startConversation)

#### [module botbuilder.DefaultLocalizer](#apidoc.module.botbuilder.DefaultLocalizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>DefaultLocalizer (root, defaultLocale)](#apidoc.element.botbuilder.DefaultLocalizer.DefaultLocalizer)

#### [module botbuilder.Dialog](#apidoc.module.botbuilder.Dialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Dialog ()](#apidoc.element.botbuilder.Dialog.Dialog)

#### [module botbuilder.Dialog.prototype](#apidoc.module.botbuilder.Dialog.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.Dialog.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>constructor ()](#apidoc.element.botbuilder.Dialog.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.Dialog.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.Dialog.prototype.recognize)

#### [module botbuilder.DialogAction](#apidoc.module.botbuilder.DialogAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>DialogAction ()](#apidoc.element.botbuilder.DialogAction.DialogAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>beginDialog (id, args)](#apidoc.element.botbuilder.DialogAction.beginDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>endDialog (result)](#apidoc.element.botbuilder.DialogAction.endDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>send (msg)](#apidoc.element.botbuilder.DialogAction.send)
1.  [function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>validatedPrompt (promptType, validator)](#apidoc.element.botbuilder.DialogAction.validatedPrompt)

#### [module botbuilder.EntityRecognizer](#apidoc.module.botbuilder.EntityRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>EntityRecognizer ()](#apidoc.element.botbuilder.EntityRecognizer.EntityRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>expandChoices (choices)](#apidoc.element.botbuilder.EntityRecognizer.expandChoices)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findAllEntities (entities, type)](#apidoc.element.botbuilder.EntityRecognizer.findAllEntities)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findAllMatches (choices, utterance, threshold)](#apidoc.element.botbuilder.EntityRecognizer.findAllMatches)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findBestMatch (choices, utterance, threshold)](#apidoc.element.botbuilder.EntityRecognizer.findBestMatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findEntity (entities, type)](#apidoc.element.botbuilder.EntityRecognizer.findEntity)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseBoolean (utterance)](#apidoc.element.botbuilder.EntityRecognizer.parseBoolean)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseNumber (entities)](#apidoc.element.botbuilder.EntityRecognizer.parseNumber)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseTime (entities)](#apidoc.element.botbuilder.EntityRecognizer.parseTime)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>recognizeTime (utterance, refDate)](#apidoc.element.botbuilder.EntityRecognizer.recognizeTime)
1.  [function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>resolveTime (entities)](#apidoc.element.botbuilder.EntityRecognizer.resolveTime)
1.  object <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>dateExp
1.  object <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>noExp
1.  object <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>numberExp
1.  object <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>yesExp
1.  string <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>ordinalWords

#### [module botbuilder.Fact](#apidoc.module.botbuilder.Fact)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Fact (session)](#apidoc.element.botbuilder.Fact.Fact)
1.  [function <span class="apidocSignatureSpan">botbuilder.Fact.</span>create (session, value, key)](#apidoc.element.botbuilder.Fact.create)

#### [module botbuilder.Fact.prototype](#apidoc.module.botbuilder.Fact.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>key (text)](#apidoc.element.botbuilder.Fact.prototype.key)
1.  [function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>toFact ()](#apidoc.element.botbuilder.Fact.prototype.toFact)
1.  [function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>value (v)](#apidoc.element.botbuilder.Fact.prototype.value)

#### [module botbuilder.HeroCard](#apidoc.module.botbuilder.HeroCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>HeroCard (session)](#apidoc.element.botbuilder.HeroCard.HeroCard)

#### [module botbuilder.HeroCard.prototype](#apidoc.module.botbuilder.HeroCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.HeroCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.HeroCard.prototype.constructor)

#### [module botbuilder.IntentDialog](#apidoc.module.botbuilder.IntentDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>IntentDialog (options)](#apidoc.element.botbuilder.IntentDialog.IntentDialog)

#### [module botbuilder.IntentDialog.prototype](#apidoc.module.botbuilder.IntentDialog.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.IntentDialog.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>constructor (options)](#apidoc.element.botbuilder.IntentDialog.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.IntentDialog.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>emitError (session, err)](#apidoc.element.botbuilder.IntentDialog.prototype.emitError)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>invokeIntent (session, recognizeResult)](#apidoc.element.botbuilder.IntentDialog.prototype.invokeIntent)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>matches (intent, dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.matches)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>matchesAny (intents, dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.matchesAny)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.IntentDialog.prototype.onBegin)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.onDefault)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.IntentDialog.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.IntentDialog.prototype.recognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.IntentDialog.prototype.replyReceived)

#### [module botbuilder.IntentRecognizerSet](#apidoc.module.botbuilder.IntentRecognizerSet)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>IntentRecognizerSet (options)](#apidoc.element.botbuilder.IntentRecognizerSet.IntentRecognizerSet)

#### [module botbuilder.IntentRecognizerSet.prototype](#apidoc.module.botbuilder.IntentRecognizerSet.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>clone (copyTo)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.clone)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognize (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizeInParallel (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInParallel)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizeInSeries (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInSeries)
1.  [function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizer)

#### [module botbuilder.Keyboard](#apidoc.module.botbuilder.Keyboard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Keyboard (session)](#apidoc.element.botbuilder.Keyboard.Keyboard)

#### [module botbuilder.Keyboard.prototype](#apidoc.module.botbuilder.Keyboard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Keyboard.prototype.</span>buttons (list)](#apidoc.element.botbuilder.Keyboard.prototype.buttons)
1.  [function <span class="apidocSignatureSpan">botbuilder.Keyboard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.Keyboard.prototype.toAttachment)

#### [module botbuilder.Library](#apidoc.module.botbuilder.Library)
1.  boolean <span class="apidocSignatureSpan">botbuilder.Library.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Library (name)](#apidoc.element.botbuilder.Library.Library)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.</span>EventEmitter ()](#apidoc.element.botbuilder.Library.EventEmitter)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.</span>addRouteResult (route, current)](#apidoc.element.botbuilder.Library.addRouteResult)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.</span>bestRouteResult (routes, dialogStack, rootLibraryName)](#apidoc.element.botbuilder.Library.bestRouteResult)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.</span>init ()](#apidoc.element.botbuilder.Library.init)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.Library.listenerCount)
1.  number <span class="apidocSignatureSpan">botbuilder.Library.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">botbuilder.Library.</span>RouteTypes

#### [module botbuilder.Library.prototype](#apidoc.module.botbuilder.Library.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>beginDialogAction (name, id, options)](#apidoc.element.botbuilder.Library.prototype.beginDialogAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>clone (copyTo, newName)](#apidoc.element.botbuilder.Library.prototype.clone)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>constructor (name)](#apidoc.element.botbuilder.Library.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>defaultFindRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.defaultFindRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>defaultSelectRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.defaultSelectRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>dialog (id, dialog)](#apidoc.element.botbuilder.Library.prototype.dialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>endConversationAction (name, msg, options)](#apidoc.element.botbuilder.Library.prototype.endConversationAction)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findActiveDialogRoutes (context, callback, dialogStack)](#apidoc.element.botbuilder.Library.prototype.findActiveDialogRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findDialog (libName, dialogId)](#apidoc.element.botbuilder.Library.prototype.findDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findGlobalActionRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.findGlobalActionRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.findRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findStackActionRoutes (context, callback, dialogStack)](#apidoc.element.botbuilder.Library.prototype.findStackActionRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>forEachDialog (callback)](#apidoc.element.botbuilder.Library.prototype.forEachDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>forEachLibrary (callback)](#apidoc.element.botbuilder.Library.prototype.forEachLibrary)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>library (lib)](#apidoc.element.botbuilder.Library.prototype.library)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>libraryList (reverse)](#apidoc.element.botbuilder.Library.prototype.libraryList)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>localePath (path)](#apidoc.element.botbuilder.Library.prototype.localePath)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>onFindRoutes (handler)](#apidoc.element.botbuilder.Library.prototype.onFindRoutes)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>onSelectRoute (handler)](#apidoc.element.botbuilder.Library.prototype.onSelectRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>recognize (context, callback)](#apidoc.element.botbuilder.Library.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.Library.prototype.recognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectActiveDialogRoute (session, route, newStack)](#apidoc.element.botbuilder.Library.prototype.selectActiveDialogRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectGlobalActionRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.selectGlobalActionRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.selectRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectStackActionRoute (session, route, newStack)](#apidoc.element.botbuilder.Library.prototype.selectStackActionRoute)

#### [module botbuilder.LuisDialog](#apidoc.module.botbuilder.LuisDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>LuisDialog (serviceUri)](#apidoc.element.botbuilder.LuisDialog.LuisDialog)

#### [module botbuilder.LuisDialog.prototype](#apidoc.module.botbuilder.LuisDialog.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.LuisDialog.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>constructor (serviceUri)](#apidoc.element.botbuilder.LuisDialog.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.LuisDialog.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>on (intent, dialogId, dialogArgs)](#apidoc.element.botbuilder.LuisDialog.prototype.on)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.LuisDialog.prototype.onBegin)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.LuisDialog.prototype.onDefault)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.LuisDialog.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.LuisDialog.prototype.replyReceived)

#### [module botbuilder.LuisRecognizer](#apidoc.module.botbuilder.LuisRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>LuisRecognizer (models)](#apidoc.element.botbuilder.LuisRecognizer.LuisRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisRecognizer.</span>recognize (utterance, modelUrl, callback)](#apidoc.element.botbuilder.LuisRecognizer.recognize)

#### [module botbuilder.LuisRecognizer.prototype](#apidoc.module.botbuilder.LuisRecognizer.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.LuisRecognizer.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.LuisRecognizer.prototype.recognize)

#### [module botbuilder.MediaCard](#apidoc.module.botbuilder.MediaCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>MediaCard (session)](#apidoc.element.botbuilder.MediaCard.MediaCard)

#### [module botbuilder.MediaCard.prototype](#apidoc.module.botbuilder.MediaCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>autoloop (choice)](#apidoc.element.botbuilder.MediaCard.prototype.autoloop)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>autostart (choice)](#apidoc.element.botbuilder.MediaCard.prototype.autostart)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.MediaCard.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>image (image)](#apidoc.element.botbuilder.MediaCard.prototype.image)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>media (list)](#apidoc.element.botbuilder.MediaCard.prototype.media)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>shareable (choice)](#apidoc.element.botbuilder.MediaCard.prototype.shareable)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.MediaCard.prototype.subtitle)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>text (text)](#apidoc.element.botbuilder.MediaCard.prototype.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>title (text)](#apidoc.element.botbuilder.MediaCard.prototype.title)

#### [module botbuilder.MemoryBotStorage](#apidoc.module.botbuilder.MemoryBotStorage)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>MemoryBotStorage ()](#apidoc.element.botbuilder.MemoryBotStorage.MemoryBotStorage)

#### [module botbuilder.MemoryBotStorage.prototype](#apidoc.module.botbuilder.MemoryBotStorage.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>deleteData (context)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.deleteData)
1.  [function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>getData (context, callback)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.getData)
1.  [function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>saveData (context, data, callback)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.saveData)

#### [module botbuilder.Message](#apidoc.module.botbuilder.Message)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Message (session)](#apidoc.element.botbuilder.Message.Message)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.</span>composePrompt (session, prompts, args)](#apidoc.element.botbuilder.Message.composePrompt)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.</span>randomPrompt (prompts)](#apidoc.element.botbuilder.Message.randomPrompt)

#### [module botbuilder.Message.prototype](#apidoc.module.botbuilder.Message.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>addAttachment (attachment)](#apidoc.element.botbuilder.Message.prototype.addAttachment)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>addEntity (obj)](#apidoc.element.botbuilder.Message.prototype.addEntity)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>address (adr)](#apidoc.element.botbuilder.Message.prototype.address)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>attachmentLayout (style)](#apidoc.element.botbuilder.Message.prototype.attachmentLayout)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>attachments (list)](#apidoc.element.botbuilder.Message.prototype.attachments)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>compose (prompts)](#apidoc.element.botbuilder.Message.prototype.compose)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>composePrompt (session, prompts)](#apidoc.element.botbuilder.Message.prototype.composePrompt)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>entities (list)](#apidoc.element.botbuilder.Message.prototype.entities)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>ntext (msg, msg_plural, count)](#apidoc.element.botbuilder.Message.prototype.ntext)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setChannelData (data)](#apidoc.element.botbuilder.Message.prototype.setChannelData)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setLanguage (local)](#apidoc.element.botbuilder.Message.prototype.setLanguage)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setNText (session, msg, msg_plural, count)](#apidoc.element.botbuilder.Message.prototype.setNText)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setText (session, prompts)](#apidoc.element.botbuilder.Message.prototype.setText)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>sourceEvent (map)](#apidoc.element.botbuilder.Message.prototype.sourceEvent)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>summary (text)](#apidoc.element.botbuilder.Message.prototype.summary)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>text (text)](#apidoc.element.botbuilder.Message.prototype.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>textFormat (style)](#apidoc.element.botbuilder.Message.prototype.textFormat)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>textLocale (locale)](#apidoc.element.botbuilder.Message.prototype.textLocale)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>timestamp (time)](#apidoc.element.botbuilder.Message.prototype.timestamp)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>toMessage ()](#apidoc.element.botbuilder.Message.prototype.toMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>upgradeAttachment (a)](#apidoc.element.botbuilder.Message.prototype.upgradeAttachment)

#### [module botbuilder.Middleware](#apidoc.module.botbuilder.Middleware)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Middleware ()](#apidoc.element.botbuilder.Middleware.Middleware)
1.  [function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>dialogVersion (options)](#apidoc.element.botbuilder.Middleware.dialogVersion)
1.  [function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>firstRun (options)](#apidoc.element.botbuilder.Middleware.firstRun)
1.  [function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>sendTyping ()](#apidoc.element.botbuilder.Middleware.sendTyping)

#### [module botbuilder.Prompts](#apidoc.module.botbuilder.Prompts)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Prompts ()](#apidoc.element.botbuilder.Prompts.Prompts)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>attachment (session, prompt, options)](#apidoc.element.botbuilder.Prompts.attachment)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>choice (session, prompt, choices, options)](#apidoc.element.botbuilder.Prompts.choice)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>configure (options)](#apidoc.element.botbuilder.Prompts.configure)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>confirm (session, prompt, options)](#apidoc.element.botbuilder.Prompts.confirm)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>disambiguate (session, prompt, choices, options)](#apidoc.element.botbuilder.Prompts.disambiguate)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>number (session, prompt, options)](#apidoc.element.botbuilder.Prompts.number)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>text (session, prompt, options)](#apidoc.element.botbuilder.Prompts.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>time (session, prompt, options)](#apidoc.element.botbuilder.Prompts.time)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>validateSession (session)](#apidoc.element.botbuilder.Prompts.validateSession)
1.  object <span class="apidocSignatureSpan">botbuilder.Prompts.</span>defaultRetryPrompt
1.  object <span class="apidocSignatureSpan">botbuilder.Prompts.</span>options

#### [module botbuilder.Prompts.prototype](#apidoc.module.botbuilder.Prompts.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.Prompts.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>constructor ()](#apidoc.element.botbuilder.Prompts.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>createPrompt (session, args, retry)](#apidoc.element.botbuilder.Prompts.prototype.createPrompt)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.Prompts.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.Prompts.prototype.recognize)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>replyReceived (session, result)](#apidoc.element.botbuilder.Prompts.prototype.replyReceived)
1.  [function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>sendPrompt (session, args, retry)](#apidoc.element.botbuilder.Prompts.prototype.sendPrompt)

#### [module botbuilder.ReceiptCard](#apidoc.module.botbuilder.ReceiptCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptCard (session)](#apidoc.element.botbuilder.ReceiptCard.ReceiptCard)

#### [module botbuilder.ReceiptCard.prototype](#apidoc.module.botbuilder.ReceiptCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>buttons (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.buttons)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>facts (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.facts)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>items (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.items)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>tap (action)](#apidoc.element.botbuilder.ReceiptCard.prototype.tap)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>tax (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.tax)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>title (text)](#apidoc.element.botbuilder.ReceiptCard.prototype.title)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.ReceiptCard.prototype.toAttachment)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>total (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.total)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>vat (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.vat)

#### [module botbuilder.ReceiptItem](#apidoc.module.botbuilder.ReceiptItem)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptItem (session)](#apidoc.element.botbuilder.ReceiptItem.ReceiptItem)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.</span>create (session, price, title)](#apidoc.element.botbuilder.ReceiptItem.create)

#### [module botbuilder.ReceiptItem.prototype](#apidoc.module.botbuilder.ReceiptItem.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>image (img)](#apidoc.element.botbuilder.ReceiptItem.prototype.image)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>price (v)](#apidoc.element.botbuilder.ReceiptItem.prototype.price)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>quantity (v)](#apidoc.element.botbuilder.ReceiptItem.prototype.quantity)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.subtitle)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>tap (action)](#apidoc.element.botbuilder.ReceiptItem.prototype.tap)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>text (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>title (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.title)
1.  [function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>toItem ()](#apidoc.element.botbuilder.ReceiptItem.prototype.toItem)

#### [module botbuilder.RegExpRecognizer](#apidoc.module.botbuilder.RegExpRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>RegExpRecognizer (intent, expressions)](#apidoc.element.botbuilder.RegExpRecognizer.RegExpRecognizer)

#### [module botbuilder.RegExpRecognizer.prototype](#apidoc.module.botbuilder.RegExpRecognizer.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.RegExpRecognizer.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.RegExpRecognizer.prototype.recognize)

#### [module botbuilder.Session](#apidoc.module.botbuilder.Session)
1.  boolean <span class="apidocSignatureSpan">botbuilder.Session.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>Session (options)](#apidoc.element.botbuilder.Session.Session)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>EventEmitter ()](#apidoc.element.botbuilder.Session.EventEmitter)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>activeDialogStackEntry (stack)](#apidoc.element.botbuilder.Session.activeDialogStackEntry)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>findDialogStackEntry (stack, dialogId, reverse)](#apidoc.element.botbuilder.Session.findDialogStackEntry)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>forEachDialogStackEntry (stack, reverse, fn)](#apidoc.element.botbuilder.Session.forEachDialogStackEntry)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>init ()](#apidoc.element.botbuilder.Session.init)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.Session.listenerCount)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>popDialogStackEntry (stack)](#apidoc.element.botbuilder.Session.popDialogStackEntry)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>pruneDialogStack (stack, start)](#apidoc.element.botbuilder.Session.pruneDialogStack)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>pushDialogStackEntry (stack, entry)](#apidoc.element.botbuilder.Session.pushDialogStackEntry)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.</span>validateDialogStack (stack, root)](#apidoc.element.botbuilder.Session.validateDialogStack)
1.  number <span class="apidocSignatureSpan">botbuilder.Session.</span>defaultMaxListeners

#### [module botbuilder.Session.prototype](#apidoc.module.botbuilder.Session.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>beginDialog (id, args)](#apidoc.element.botbuilder.Session.prototype.beginDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>cancelDialog (dialogId, replaceWithId, replaceWithArgs)](#apidoc.element.botbuilder.Session.prototype.cancelDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>clearDialogStack ()](#apidoc.element.botbuilder.Session.prototype.clearDialogStack)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>constructor (options)](#apidoc.element.botbuilder.Session.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>createMessage (localizationNamespace, text, args)](#apidoc.element.botbuilder.Session.prototype.createMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>curDialog ()](#apidoc.element.botbuilder.Session.prototype.curDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>curLibraryName ()](#apidoc.element.botbuilder.Session.prototype.curLibraryName)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>deleteDialogs (dialogId)](#apidoc.element.botbuilder.Session.prototype.deleteDialogs)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>dialogStack (newStack)](#apidoc.element.botbuilder.Session.prototype.dialogStack)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>dispatch (sessionState, message, done)](#apidoc.element.botbuilder.Session.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endConversation (message)](#apidoc.element.botbuilder.Session.prototype.endConversation)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endDialog (message)](#apidoc.element.botbuilder.Session.prototype.endDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endDialogWithResult (result)](#apidoc.element.botbuilder.Session.prototype.endDialogWithResult)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>error (err)](#apidoc.element.botbuilder.Session.prototype.error)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>findDialog (id)](#apidoc.element.botbuilder.Session.prototype.findDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>getMessageReceived ()](#apidoc.element.botbuilder.Session.prototype.getMessageReceived)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>gettext (messageid)](#apidoc.element.botbuilder.Session.prototype.gettext)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>isReset ()](#apidoc.element.botbuilder.Session.prototype.isReset)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>messageSent ()](#apidoc.element.botbuilder.Session.prototype.messageSent)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>ngettext (messageid, messageid_plural, count)](#apidoc.element.botbuilder.Session.prototype.ngettext)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>popDialog ()](#apidoc.element.botbuilder.Session.prototype.popDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>preferredLocale (locale, callback)](#apidoc.element.botbuilder.Session.prototype.preferredLocale)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>prepareMessage (msg)](#apidoc.element.botbuilder.Session.prototype.prepareMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>pushDialog (ds)](#apidoc.element.botbuilder.Session.prototype.pushDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>replaceDialog (id, args)](#apidoc.element.botbuilder.Session.prototype.replaceDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>reset (dialogId, dialogArgs)](#apidoc.element.botbuilder.Session.prototype.reset)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>resolveDialogId (id)](#apidoc.element.botbuilder.Session.prototype.resolveDialogId)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>routeToActiveDialog (recognizeResult)](#apidoc.element.botbuilder.Session.prototype.routeToActiveDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>save ()](#apidoc.element.botbuilder.Session.prototype.save)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>send (message)](#apidoc.element.botbuilder.Session.prototype.send)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendBatch (callback)](#apidoc.element.botbuilder.Session.prototype.sendBatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendLocalized (localizationNamespace, message)](#apidoc.element.botbuilder.Session.prototype.sendLocalized)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendTyping ()](#apidoc.element.botbuilder.Session.prototype.sendTyping)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>startBatch ()](#apidoc.element.botbuilder.Session.prototype.startBatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>toRecognizeContext ()](#apidoc.element.botbuilder.Session.prototype.toRecognizeContext)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>validateCallstack ()](#apidoc.element.botbuilder.Session.prototype.validateCallstack)
1.  [function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>vgettext (localizationNamespace, messageid, args)](#apidoc.element.botbuilder.Session.prototype.vgettext)

#### [module botbuilder.SigninCard](#apidoc.module.botbuilder.SigninCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SigninCard (session)](#apidoc.element.botbuilder.SigninCard.SigninCard)

#### [module botbuilder.SigninCard.prototype](#apidoc.module.botbuilder.SigninCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>button (title, url)](#apidoc.element.botbuilder.SigninCard.prototype.button)
1.  [function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>text (prompts)](#apidoc.element.botbuilder.SigninCard.prototype.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.SigninCard.prototype.toAttachment)

#### [module botbuilder.SimpleDialog](#apidoc.module.botbuilder.SimpleDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SimpleDialog (fn)](#apidoc.element.botbuilder.SimpleDialog.SimpleDialog)

#### [module botbuilder.SimpleDialog.prototype](#apidoc.module.botbuilder.SimpleDialog.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.SimpleDialog.prototype.begin)
1.  [function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>constructor (fn)](#apidoc.element.botbuilder.SimpleDialog.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.SimpleDialog.prototype.dialogResumed)
1.  [function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>replyReceived (session)](#apidoc.element.botbuilder.SimpleDialog.prototype.replyReceived)

#### [module botbuilder.SimplePromptRecognizer](#apidoc.module.botbuilder.SimplePromptRecognizer)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>SimplePromptRecognizer ()](#apidoc.element.botbuilder.SimplePromptRecognizer.SimplePromptRecognizer)

#### [module botbuilder.SimplePromptRecognizer.prototype](#apidoc.module.botbuilder.SimplePromptRecognizer.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.SimplePromptRecognizer.prototype.</span>recognize (args, callback, session)](#apidoc.element.botbuilder.SimplePromptRecognizer.prototype.recognize)

#### [module botbuilder.TextBot](#apidoc.module.botbuilder.TextBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>TextBot (options)](#apidoc.element.botbuilder.TextBot.TextBot)

#### [module botbuilder.TextBot.prototype](#apidoc.module.botbuilder.TextBot.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>add (id, dialog)](#apidoc.element.botbuilder.TextBot.prototype.add)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>beginDialog (address, dialogId, dialogArgs)](#apidoc.element.botbuilder.TextBot.prototype.beginDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>configure (options)](#apidoc.element.botbuilder.TextBot.prototype.configure)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>listenStdin ()](#apidoc.element.botbuilder.TextBot.prototype.listenStdin)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>on (event, listener)](#apidoc.element.botbuilder.TextBot.prototype.on)
1.  [function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>processMessage (message, callback)](#apidoc.element.botbuilder.TextBot.prototype.processMessage)

#### [module botbuilder.ThumbnailCard](#apidoc.module.botbuilder.ThumbnailCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>ThumbnailCard (session)](#apidoc.element.botbuilder.ThumbnailCard.ThumbnailCard)

#### [module botbuilder.ThumbnailCard.prototype](#apidoc.module.botbuilder.ThumbnailCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.ThumbnailCard.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>images (list)](#apidoc.element.botbuilder.ThumbnailCard.prototype.images)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.subtitle)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>tap (action)](#apidoc.element.botbuilder.ThumbnailCard.prototype.tap)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>text (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.text)
1.  [function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>title (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.title)

#### [module botbuilder.UniversalBot](#apidoc.module.botbuilder.UniversalBot)
1.  boolean <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>UniversalBot (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot.UniversalBot)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>EventEmitter ()](#apidoc.element.botbuilder.UniversalBot.EventEmitter)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>addRouteResult (route, current)](#apidoc.element.botbuilder.UniversalBot.addRouteResult)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>bestRouteResult (routes, dialogStack, rootLibraryName)](#apidoc.element.botbuilder.UniversalBot.bestRouteResult)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>init ()](#apidoc.element.botbuilder.UniversalBot.init)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.UniversalBot.listenerCount)
1.  number <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>RouteTypes

#### [module botbuilder.UniversalBot.prototype](#apidoc.module.botbuilder.UniversalBot.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>beginDialog (address, dialogId, dialogArgs, done)](#apidoc.element.botbuilder.UniversalBot.prototype.beginDialog)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>clone (copyTo, newName)](#apidoc.element.botbuilder.UniversalBot.prototype.clone)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>connector (channelId, connector)](#apidoc.element.botbuilder.UniversalBot.prototype.connector)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>constructor (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>createSession (storageCtx, message, dialogId, dialogArgs, done, newStack)](#apidoc.element.botbuilder.UniversalBot.prototype.createSession)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>dispatch (storageCtx, message, dialogId, dialogArgs, done, newStack)](#apidoc.element.botbuilder.UniversalBot.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>emitError (err)](#apidoc.element.botbuilder.UniversalBot.prototype.emitError)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>ensureConversation (address, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.ensureConversation)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>errorLogger (done)](#apidoc.element.botbuilder.UniversalBot.prototype.errorLogger)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>eventMiddleware (event, middleware, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.eventMiddleware)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>get (name)](#apidoc.element.botbuilder.UniversalBot.prototype.get)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>getStorage ()](#apidoc.element.botbuilder.UniversalBot.prototype.getStorage)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>getStorageData (storageCtx, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.getStorageData)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>isInConversation (address, cb)](#apidoc.element.botbuilder.UniversalBot.prototype.isInConversation)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>isMessage (message)](#apidoc.element.botbuilder.UniversalBot.prototype.isMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>loadSession (address, done)](#apidoc.element.botbuilder.UniversalBot.prototype.loadSession)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>lookupUser (address, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.lookupUser)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>onDisambiguateRoute (handler)](#apidoc.element.botbuilder.UniversalBot.prototype.onDisambiguateRoute)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>receive (events, done)](#apidoc.element.botbuilder.UniversalBot.prototype.receive)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>routeMessage (session, done)](#apidoc.element.botbuilder.UniversalBot.prototype.routeMessage)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>saveStorageData (storageCtx, data, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.saveStorageData)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.UniversalBot.prototype.send)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>set (name, value)](#apidoc.element.botbuilder.UniversalBot.prototype.set)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>tryCatch (fn, error)](#apidoc.element.botbuilder.UniversalBot.prototype.tryCatch)
1.  [function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>use ()](#apidoc.element.botbuilder.UniversalBot.prototype.use)

#### [module botbuilder.VideoCard](#apidoc.module.botbuilder.VideoCard)
1.  [function <span class="apidocSignatureSpan">botbuilder.</span>VideoCard (session)](#apidoc.element.botbuilder.VideoCard.VideoCard)

#### [module botbuilder.VideoCard.prototype](#apidoc.module.botbuilder.VideoCard.prototype)
1.  [function <span class="apidocSignatureSpan">botbuilder.VideoCard.prototype.</span>aspect (text)](#apidoc.element.botbuilder.VideoCard.prototype.aspect)
1.  [function <span class="apidocSignatureSpan">botbuilder.VideoCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.VideoCard.prototype.constructor)

#### [module botbuilder.logger](#apidoc.module.botbuilder.logger)
1.  [function <span class="apidocSignatureSpan">botbuilder.logger.</span>debug (fmt)](#apidoc.element.botbuilder.logger.debug)
1.  [function <span class="apidocSignatureSpan">botbuilder.logger.</span>error (fmt)](#apidoc.element.botbuilder.logger.error)
1.  [function <span class="apidocSignatureSpan">botbuilder.logger.</span>info (addressable, fmt)](#apidoc.element.botbuilder.logger.info)
1.  [function <span class="apidocSignatureSpan">botbuilder.logger.</span>trace (fmt)](#apidoc.element.botbuilder.logger.trace)
1.  [function <span class="apidocSignatureSpan">botbuilder.logger.</span>warn (addressable, fmt)](#apidoc.element.botbuilder.logger.warn)

#### [module botbuilder.utils](#apidoc.module.botbuilder.utils)
1.  [function <span class="apidocSignatureSpan">botbuilder.utils.</span>clone (obj)](#apidoc.element.botbuilder.utils.clone)
1.  [function <span class="apidocSignatureSpan">botbuilder.utils.</span>copyFieldsTo (frm, to, fields)](#apidoc.element.botbuilder.utils.copyFieldsTo)
1.  [function <span class="apidocSignatureSpan">botbuilder.utils.</span>copyTo (frm, to)](#apidoc.element.botbuilder.utils.copyTo)
1.  [function <span class="apidocSignatureSpan">botbuilder.utils.</span>moveFieldsTo (frm, to, fields)](#apidoc.element.botbuilder.utils.moveFieldsTo)
1.  [function <span class="apidocSignatureSpan">botbuilder.utils.</span>toDate8601 (date)](#apidoc.element.botbuilder.utils.toDate8601)



# <a name="apidoc.module.botbuilder"></a>[module botbuilder](#apidoc.module.botbuilder)

#### <a name="apidoc.element.botbuilder.AnimationCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>AnimationCard (session)](#apidoc.element.botbuilder.AnimationCard)
- description and source-code
```javascript
function AnimationCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.animation';
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.AudioCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>AudioCard (session)](#apidoc.element.botbuilder.AudioCard)
- description and source-code
```javascript
function AudioCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.audio';
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>BotConnectorBot (options)](#apidoc.element.botbuilder.BotConnectorBot)
- description and source-code
```javascript
function BotConnectorBot(options) {
    console.warn('BotConnectorBot class is deprecated. Use UniversalBot with a ChatConnector class.');
    var oConnector = {};
    var oBot = {};
    for (var key in options) {
        switch (key) {
            case 'appId':
                oConnector.appId = options.appId;
                break;
            case 'appSecret':
                oConnector.appPassword = options.appSecret;
                break;
            case 'defaultDialogId':
                oBot.defaultDialogId = options.defaultDialogId;
                break;
            case 'defaultDialogArgs':
                oBot.defaultDialogArgs = options.defaultDialogArgs;
                break;
            case 'groupWelcomeMessage':
                this.groupWelcomeMessage = options.groupWelcomeMessage;
                break;
            case 'userWelcomeMessage':
                this.userWelcomeMessage = options.userWelcomeMessage;
                break;
            case 'goodbyeMessage':
                this.goodbyeMessage = options.goodbyeMessage;
                break;
            case 'userStore':
            case 'conversationStore':
            case 'perUserInConversationStore':
                console.error('BotConnectorBot custom stores no longer supported. Use UniversalBot with a custom IBotStorage implementation
 instead.');
                throw new Error('BotConnectorBot custom stores no longer supported.');
        }
    }
    this.connector = new ChatConnector_1.ChatConnector(oConnector);
    this.bot = new UniversalBot_1.UniversalBot(this.connector, oBot);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardAction (session)](#apidoc.element.botbuilder.CardAction)
- description and source-code
```javascript
function CardAction(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardImage"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardImage (session)](#apidoc.element.botbuilder.CardImage)
- description and source-code
```javascript
function CardImage(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
...
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
...
```

#### <a name="apidoc.element.botbuilder.CardMedia"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardMedia (session)](#apidoc.element.botbuilder.CardMedia)
- description and source-code
```javascript
function CardMedia(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ChatConnector (settings)](#apidoc.element.botbuilder.ChatConnector)
- description and source-code
```javascript
function ChatConnector(settings) {
    if (settings === void 0) { settings = {}; }
    this.settings = settings;
    if (!this.settings.endpoint) {
        this.settings.endpoint = {
            refreshEndpoint: 'https://login.microsoftonline.com/botframework.com/oauth2/v2.0/token',
            refreshScope: 'https://api.botframework.com/.default',
            botConnectorOpenIdMetadata: this.settings.openIdMetadata || 'https://login.botframework.com/v1/.well-known/openidconfiguration
',
            botConnectorIssuer: 'https://api.botframework.com',
            botConnectorAudience: this.settings.appId,
            msaOpenIdMetadata: 'https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration',
            msaIssuer: 'https://sts.windows.net/72f988bf-86f1-41af-91ab-2d7cd011db47/',
            msaAudience: 'https://graph.microsoft.com',
            emulatorOpenIdMetadata: 'https://login.microsoftonline.com/botframework.com/v2.0/.well-known/openid-configuration',
            emulatorAudience: 'https://sts.windows.net/d6d49420-f39b-4df7-a1dc-d59a935871db/',
            emulatorIssuer: this.settings.appId,
            stateEndpoint: this.settings.stateEndpoint || 'https://state.botframework.com'
        };
    }
    this.botConnectorOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.botConnectorOpenIdMetadata);
    this.msaOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.msaOpenIdMetadata);
    this.emulatorOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.emulatorOpenIdMetadata);
}
```
- example usage
```shell
...

Create a file named app.js and say hello in a few lines of code.

var restify = require('restify');
var builder = require('botbuilder');

// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});
...
```

#### <a name="apidoc.element.botbuilder.CommandDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CommandDialog (serviceUri)](#apidoc.element.botbuilder.CommandDialog)
- description and source-code
```javascript
function CommandDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('CommandDialog class is deprecated. Use IntentDialog class instead.');
    _this.dialog = new IntentDialog_1.IntentDialog();
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ConsoleConnector ()](#apidoc.element.botbuilder.ConsoleConnector)
- description and source-code
```javascript
function ConsoleConnector() {
    this.replyCnt = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Dialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Dialog ()](#apidoc.element.botbuilder.Dialog)
- description and source-code
```javascript
function Dialog() {
    return _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.DialogAction"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>DialogAction ()](#apidoc.element.botbuilder.DialogAction)
- description and source-code
```javascript
function DialogAction() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>EntityRecognizer ()](#apidoc.element.botbuilder.EntityRecognizer)
- description and source-code
```javascript
function EntityRecognizer() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Fact"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Fact (session)](#apidoc.element.botbuilder.Fact)
- description and source-code
```javascript
function Fact(session) {
    this.session = session;
    this.data = { value: '' };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.HeroCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>HeroCard (session)](#apidoc.element.botbuilder.HeroCard)
- description and source-code
```javascript
function HeroCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.hero';
    return _this;
}
```
- example usage
```shell
...
            isOldSchema = true;
            break;
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
...
```

#### <a name="apidoc.element.botbuilder.IntentDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>IntentDialog (options)](#apidoc.element.botbuilder.IntentDialog)
- description and source-code
```javascript
function IntentDialog(options) {
    if (options === void 0) { options = {}; }
    var _this = _super.call(this) || this;
    _this.handlers = {};
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet(options);
    if (typeof options.recognizeMode !== "undefined") {
        _this.recognizeMode = options.recognizeMode;
    }
    else {
        _this.recognizeMode = RecognizeMode.onBeginIfRoot;
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>IntentRecognizerSet (options)](#apidoc.element.botbuilder.IntentRecognizerSet)
- description and source-code
```javascript
function IntentRecognizerSet(options) {
    if (options === void 0) { options = {}; }
    this.options = options;
    if (typeof this.options.intentThreshold !== 'number') {
        this.options.intentThreshold = 0.1;
    }
    if (!this.options.hasOwnProperty('recognizeOrder')) {
        this.options.recognizeOrder = RecognizeOrder.parallel;
    }
    if (!this.options.recognizers) {
        this.options.recognizers = [];
    }
    if (!this.options.processLimit) {
        this.options.processLimit = 4;
    }
    if (!this.options.hasOwnProperty('stopIfExactMatch')) {
        this.options.stopIfExactMatch = true;
    }
    this.length = this.options.recognizers.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Keyboard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Keyboard (session)](#apidoc.element.botbuilder.Keyboard)
- description and source-code
```javascript
function Keyboard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.keyboard',
        content: {}
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Library (name)](#apidoc.element.botbuilder.Library)
- description and source-code
```javascript
function Library(name) {
    var _this = _super.call(this) || this;
    _this.name = name;
    _this.dialogs = {};
    _this.libraries = {};
    _this.actions = new ActionSet_1.ActionSet();
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet();
    _this.triggersAdded = false;
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>LuisDialog (serviceUri)](#apidoc.element.botbuilder.LuisDialog)
- description and source-code
```javascript
function LuisDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('LuisDialog class is deprecated. Use IntentDialog with a LuisRecognizer instead.');
    var recognizer = new LuisRecognizer_1.LuisRecognizer(serviceUri);
    _this.dialog = new IntentDialog_1.IntentDialog({ recognizers: [recognizer] });
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>LuisRecognizer (models)](#apidoc.element.botbuilder.LuisRecognizer)
- description and source-code
```javascript
function LuisRecognizer(models) {
    if (typeof models == 'string') {
        this.models = { '*': models };
    }
    else {
        this.models = (models || {});
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>MediaCard (session)](#apidoc.element.botbuilder.MediaCard)
- description and source-code
```javascript
function MediaCard(session) {
    return _super.call(this, session) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MemoryBotStorage"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>MemoryBotStorage ()](#apidoc.element.botbuilder.MemoryBotStorage)
- description and source-code
```javascript
function MemoryBotStorage() {
    this.userStore = {};
    this.conversationStore = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Message (session)](#apidoc.element.botbuilder.Message)
- description and source-code
```javascript
function Message(session) {
    this.session = session;
    this.data = {};
    this.data.type = consts.messageType;
    this.data.agent = consts.agent;
    if (this.session) {
        var m = this.session.message;
        if (m.source) {
            this.data.source = m.source;
        }
        if (m.textLocale) {
            this.data.textLocale = m.textLocale;
        }
        if (m.address) {
            this.data.address = m.address;
        }
    }
}
```
- example usage
```shell
...
        }
        this.batchTimer = setTimeout(function () {
            _this.sendBatch();
        }, this.options.autoBatchDelay);
    }
};
Session.prototype.createMessage = function (localizationNamespace, text, args) {
    var message = new Message_1.Message(this)
        .text(this.vgettext(localizationNamespace, Message_1.Message.randomPrompt(text), args));
    return message.toMessage();
};
Session.prototype.prepareMessage = function (msg) {
    if (!msg.type) {
        msg.type = 'message';
    }
...
```

#### <a name="apidoc.element.botbuilder.Middleware"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Middleware ()](#apidoc.element.botbuilder.Middleware)
- description and source-code
```javascript
function Middleware() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Prompts ()](#apidoc.element.botbuilder.Prompts)
- description and source-code
```javascript
function Prompts() {
    return _super !== null && _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptCard (session)](#apidoc.element.botbuilder.ReceiptCard)
- description and source-code
```javascript
function ReceiptCard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.card.receipt',
        content: {}
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptItem"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptItem (session)](#apidoc.element.botbuilder.ReceiptItem)
- description and source-code
```javascript
function ReceiptItem(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.RegExpRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>RegExpRecognizer (intent, expressions)](#apidoc.element.botbuilder.RegExpRecognizer)
- description and source-code
```javascript
function RegExpRecognizer(intent, expressions) {
    this.intent = intent;
    if (expressions instanceof RegExp || typeof expressions.exec === 'function') {
        this.expressions = { '*': expressions };
    }
    else {
        this.expressions = (expressions || {});
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Session (options)](#apidoc.element.botbuilder.Session)
- description and source-code
```javascript
function Session(options) {
    var _this = _super.call(this) || this;
    _this.options = options;
    _this.msgSent = false;
    _this._isReset = false;
    _this.lastSendTime = new Date().getTime();
    _this.batch = [];
    _this.batchStarted = false;
    _this.sendingBatch = false;
    _this.inMiddleware = false;
    _this._locale = null;
    _this.localizer = null;
    _this.library = options.library;
    _this.localizer = options.localizer;
    if (typeof _this.options.autoBatchDelay !== 'number') {
        _this.options.autoBatchDelay = 250;
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.SigninCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SigninCard (session)](#apidoc.element.botbuilder.SigninCard)
- description and source-code
```javascript
function SigninCard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.card.signin',
        content: {}
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.SimpleDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SimpleDialog (fn)](#apidoc.element.botbuilder.SimpleDialog)
- description and source-code
```javascript
function SimpleDialog(fn) {
    var _this = _super.call(this) || this;
    _this.fn = fn;
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.SimplePromptRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SimplePromptRecognizer ()](#apidoc.element.botbuilder.SimplePromptRecognizer)
- description and source-code
```javascript
function SimplePromptRecognizer() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.TextBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>TextBot (options)](#apidoc.element.botbuilder.TextBot)
- description and source-code
```javascript
function TextBot(options) {
    if (options === void 0) { options = {}; }
    console.warn('TextBot class is deprecated. Use UniversalBot with a ConsoleConnector class.');
    var oBot = {};
    for (var key in options) {
        switch (key) {
            case 'defaultDialogId':
                oBot.defaultDialogId = options.defaultDialogId;
                break;
            case 'defaultDialogArgs':
                oBot.defaultDialogArgs = options.defaultDialogArgs;
                break;
            case 'groupWelcomeMessage':
                this.groupWelcomeMessage = options.groupWelcomeMessage;
                break;
            case 'userWelcomeMessage':
                this.userWelcomeMessage = options.userWelcomeMessage;
                break;
            case 'goodbyeMessage':
                this.goodbyeMessage = options.goodbyeMessage;
                break;
            case 'userStore':
            case 'sessionStore':
                console.error('TextBot custom stores no longer supported. Use UniversalBot with a custom IBotStorage implementation
 instead.');
                throw new Error('TextBot custom stores no longer supported.');
        }
    }
    this.connector = new ConsoleConnector_1.ConsoleConnector();
    this.bot = new UniversalBot_1.UniversalBot(this.connector, oBot);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ThumbnailCard (session)](#apidoc.element.botbuilder.ThumbnailCard)
- description and source-code
```javascript
function ThumbnailCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.thumbnail';
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>UniversalBot (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot)
- description and source-code
```javascript
function UniversalBot(connector, defaultDialog, libraryName) {
    var _this = _super.call(this, libraryName || consts.Library.default) || this;
    _this.settings = {
        processLimit: 4,
        persistUserData: true,
        persistConversationData: false
    };
    _this.connectors = {};
    _this.mwReceive = [];
    _this.mwSend = [];
    _this.mwSession = [];
    _this.localePath('./locale/');
    _this.library(Library_1.systemLib);
    if (defaultDialog) {
        if (typeof defaultDialog === 'function' || Array.isArray(defaultDialog)) {
            _this.dialog('/', defaultDialog);
        }
        else {
            var settings = defaultDialog;
            for (var name in settings) {
                if (settings.hasOwnProperty(name)) {
                    _this.set(name, settings[name]);
                }
            }
        }
    }
    if (connector) {
        _this.connector(consts.defaultConnector, connector);
    }
    return _this;
}
```
- example usage
```shell
...
var builder = require('botbuilder');

// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
...
```

#### <a name="apidoc.element.botbuilder.VideoCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>VideoCard (session)](#apidoc.element.botbuilder.VideoCard)
- description and source-code
```javascript
function VideoCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.video';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.AnimationCard"></a>[module botbuilder.AnimationCard](#apidoc.module.botbuilder.AnimationCard)

#### <a name="apidoc.element.botbuilder.AnimationCard.AnimationCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>AnimationCard (session)](#apidoc.element.botbuilder.AnimationCard.AnimationCard)
- description and source-code
```javascript
function AnimationCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.animation';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.AnimationCard.prototype"></a>[module botbuilder.AnimationCard.prototype](#apidoc.module.botbuilder.AnimationCard.prototype)

#### <a name="apidoc.element.botbuilder.AnimationCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.AnimationCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.AnimationCard.prototype.constructor)
- description and source-code
```javascript
function AnimationCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.animation';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.AudioCard"></a>[module botbuilder.AudioCard](#apidoc.module.botbuilder.AudioCard)

#### <a name="apidoc.element.botbuilder.AudioCard.AudioCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>AudioCard (session)](#apidoc.element.botbuilder.AudioCard.AudioCard)
- description and source-code
```javascript
function AudioCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.audio';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.AudioCard.prototype"></a>[module botbuilder.AudioCard.prototype](#apidoc.module.botbuilder.AudioCard.prototype)

#### <a name="apidoc.element.botbuilder.AudioCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.AudioCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.AudioCard.prototype.constructor)
- description and source-code
```javascript
function AudioCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.audio';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.BotConnectorBot"></a>[module botbuilder.BotConnectorBot](#apidoc.module.botbuilder.BotConnectorBot)

#### <a name="apidoc.element.botbuilder.BotConnectorBot.BotConnectorBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>BotConnectorBot (options)](#apidoc.element.botbuilder.BotConnectorBot.BotConnectorBot)
- description and source-code
```javascript
function BotConnectorBot(options) {
    console.warn('BotConnectorBot class is deprecated. Use UniversalBot with a ChatConnector class.');
    var oConnector = {};
    var oBot = {};
    for (var key in options) {
        switch (key) {
            case 'appId':
                oConnector.appId = options.appId;
                break;
            case 'appSecret':
                oConnector.appPassword = options.appSecret;
                break;
            case 'defaultDialogId':
                oBot.defaultDialogId = options.defaultDialogId;
                break;
            case 'defaultDialogArgs':
                oBot.defaultDialogArgs = options.defaultDialogArgs;
                break;
            case 'groupWelcomeMessage':
                this.groupWelcomeMessage = options.groupWelcomeMessage;
                break;
            case 'userWelcomeMessage':
                this.userWelcomeMessage = options.userWelcomeMessage;
                break;
            case 'goodbyeMessage':
                this.goodbyeMessage = options.goodbyeMessage;
                break;
            case 'userStore':
            case 'conversationStore':
            case 'perUserInConversationStore':
                console.error('BotConnectorBot custom stores no longer supported. Use UniversalBot with a custom IBotStorage implementation
 instead.');
                throw new Error('BotConnectorBot custom stores no longer supported.');
        }
    }
    this.connector = new ChatConnector_1.ChatConnector(oConnector);
    this.bot = new UniversalBot_1.UniversalBot(this.connector, oBot);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.BotConnectorBot.prototype"></a>[module botbuilder.BotConnectorBot.prototype](#apidoc.module.botbuilder.BotConnectorBot.prototype)

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.add"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>add (id, dialog)](#apidoc.element.botbuilder.BotConnectorBot.prototype.add)
- description and source-code
```javascript
add = function (id, dialog) {
    this.bot.dialog(id, dialog);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.beginDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>beginDialog (address, dialogId, dialogArgs)](#apidoc.element.botbuilder.BotConnectorBot.prototype.beginDialog)
- description and source-code
```javascript
beginDialog = function (address, dialogId, dialogArgs) {
    console.error("BotConnectorBot.beginDialog() is no longer supported. The schema for sending proactive messages has changed and
 you should update your code to use the new UniversalBot class.");
    throw new Error("BotConnectorBot.beginDialog() is no longer supported.");
}
```
- example usage
```shell
...
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
...
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.configure"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>configure (options)](#apidoc.element.botbuilder.BotConnectorBot.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
    console.error("BotConnectorBot.configure() is no longer supported. You should either pass all options into the constructor or
 update code to use the new UniversalBot class.");
    throw new Error("BotConnectorBot.configure() is no longer supported.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.listen"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>listen (dialogId, dialogArgs)](#apidoc.element.botbuilder.BotConnectorBot.prototype.listen)
- description and source-code
```javascript
listen = function (dialogId, dialogArgs) {
    if (dialogId) {
        console.error("Calling BotConnectorBot.listen() with a custom dialogId is no longer supported. You should either pass as
 defaultDialogId into the constructor or update code to use the new UniversalBot class.");
        throw new Error("Calling BotConnectorBot.listen() with a custom dialogId is no longer supported.");
    }
    return this.connector.listen();
}
```
- example usage
```shell
...
    var bot = new builder.UniversalBot(connector);
    bot.dialog('/', function (session) {
        session.send('Hello World');
    });

    // Setup Restify Server
    var server = restify.createServer();
    server.post('/api/messages', connector.listen());
    server.listen(process.env.port || 3978, function () {
        console.log('%s listening to %s', server.name, server.url);
    });

## Test your bot
Use the [Bot Framework Emulator](http://docs.botframework.com/connector/tools/bot-framework-emulator/) to test your bot on localhost
.
...
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.on"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>on (event, listener)](#apidoc.element.botbuilder.BotConnectorBot.prototype.on)
- description and source-code
```javascript
on = function (event, listener) {
    this.bot.on(event, listener);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.BotConnectorBot.prototype.verifyBotFramework"></a>[function <span class="apidocSignatureSpan">botbuilder.BotConnectorBot.prototype.</span>verifyBotFramework (options)](#apidoc.element.botbuilder.BotConnectorBot.prototype.verifyBotFramework)
- description and source-code
```javascript
verifyBotFramework = function (options) {
    if (options) {
        console.error("Calling BotConnectorBot.verifyBotFramework() with options is no longer supported. You should either pass
all options into the constructor or update code to use the new UniversalBot class.");
        throw new Error("Calling BotConnectorBot.verifyBotFramework() with options is no longer supported.");
    }
    return function (req, res, next) { return next(); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.CardAction"></a>[module botbuilder.CardAction](#apidoc.module.botbuilder.CardAction)

#### <a name="apidoc.element.botbuilder.CardAction.CardAction"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardAction (session)](#apidoc.element.botbuilder.CardAction.CardAction)
- description and source-code
```javascript
function CardAction(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.call"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>call (session, number, title)](#apidoc.element.botbuilder.CardAction.call)
- description and source-code
```javascript
call = function (session, number, title) {
    return new CardAction(session).type('call').value(number).title(title || "Click to call");
}
```
- example usage
```shell
...
var consts = require("./consts");
var logger = require("./logger");
var sprintf = require("sprintf-js");
var events = require("events");
var Session = (function (_super) {
__extends(Session, _super);
function Session(options) {
    var _this = _super.call(this) || this;
    _this.options = options;
    _this.msgSent = false;
    _this._isReset = false;
    _this.lastSendTime = new Date().getTime();
    _this.batch = [];
    _this.batchStarted = false;
    _this.sendingBatch = false;
...
```

#### <a name="apidoc.element.botbuilder.CardAction.dialogAction"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>dialogAction (session, action, data, title)](#apidoc.element.botbuilder.CardAction.dialogAction)
- description and source-code
```javascript
dialogAction = function (session, action, data, title) {
    var value = 'action?' + action;
    if (data) {
        value += '=' + data;
    }
    return new CardAction(session).type('postBack').value(value).title(title || "Click to send response to bot");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.downloadFile"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>downloadFile (session, url, title)](#apidoc.element.botbuilder.CardAction.downloadFile)
- description and source-code
```javascript
downloadFile = function (session, url, title) {
    return new CardAction(session).type('downloadFile').value(url).title(title || "Click to download file");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.imBack"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>imBack (session, msg, title)](#apidoc.element.botbuilder.CardAction.imBack)
- description and source-code
```javascript
imBack = function (session, msg, title) {
    return new CardAction(session).type('imBack').value(msg).title(title || "Click to send response to bot");
}
```
- example usage
```shell
...
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
            CardAction_1.CardAction.openUrl(null, old.url, old.title);
        if (old.image) {
            btn.image(old.image);
        }
        list.push(btn);
    }
    card.buttons(list);
...
```

#### <a name="apidoc.element.botbuilder.CardAction.openUrl"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>openUrl (session, url, title)](#apidoc.element.botbuilder.CardAction.openUrl)
- description and source-code
```javascript
openUrl = function (session, url, title) {
    return new CardAction(session).type('openUrl').value(url).title(title || "Click to open website in your browser");
}
```
- example usage
```shell
...
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
...
```

#### <a name="apidoc.element.botbuilder.CardAction.playAudio"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>playAudio (session, url, title)](#apidoc.element.botbuilder.CardAction.playAudio)
- description and source-code
```javascript
playAudio = function (session, url, title) {
    return new CardAction(session).type('playAudio').value(url).title(title || "Click to play audio file");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.playVideo"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>playVideo (session, url, title)](#apidoc.element.botbuilder.CardAction.playVideo)
- description and source-code
```javascript
playVideo = function (session, url, title) {
    return new CardAction(session).type('playVideo').value(url).title(title || "Click to play video");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.postBack"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>postBack (session, msg, title)](#apidoc.element.botbuilder.CardAction.postBack)
- description and source-code
```javascript
postBack = function (session, msg, title) {
    return new CardAction(session).type('postBack').value(msg).title(title || "Click to send response to bot");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.showImage"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.</span>showImage (session, url, title)](#apidoc.element.botbuilder.CardAction.showImage)
- description and source-code
```javascript
showImage = function (session, url, title) {
    return new CardAction(session).type('showImage').value(url).title(title || "Click to view image");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.CardAction.prototype"></a>[module botbuilder.CardAction.prototype](#apidoc.module.botbuilder.CardAction.prototype)

#### <a name="apidoc.element.botbuilder.CardAction.prototype.image"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>image (url)](#apidoc.element.botbuilder.CardAction.prototype.image)
- description and source-code
```javascript
image = function (url) {
    if (url) {
        this.data.image = url;
    }
    return this;
}
```
- example usage
```shell
...
        var list = [];
        for (var i = 0; i < v2.actions.length; i++) {
            var old = v2.actions[i];
            var btn = old.message ?
                CardAction_1.CardAction.imBack(null, old.message, old.title) :
                CardAction_1.CardAction.openUrl(null, old.url, old.title);
            if (old.image) {
                btn.image(old.image);
            }
            list.push(btn);
        }
        card.buttons(list);
    }
    return card.toAttachment();
}
...
```

#### <a name="apidoc.element.botbuilder.CardAction.prototype.title"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>title (text)](#apidoc.element.botbuilder.CardAction.prototype.title)
- description and source-code
```javascript
title = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.title = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
        card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
    }
...
```

#### <a name="apidoc.element.botbuilder.CardAction.prototype.toAction"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>toAction ()](#apidoc.element.botbuilder.CardAction.prototype.toAction)
- description and source-code
```javascript
toAction = function () {
    return this.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.prototype.type"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>type (t)](#apidoc.element.botbuilder.CardAction.prototype.type)
- description and source-code
```javascript
type = function (t) {
    if (t) {
        this.data.type = t;
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardAction.prototype.value"></a>[function <span class="apidocSignatureSpan">botbuilder.CardAction.prototype.</span>value (v)](#apidoc.element.botbuilder.CardAction.prototype.value)
- description and source-code
```javascript
value = function (v) {
    if (v) {
        this.data.value = v;
    }
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.CardImage"></a>[module botbuilder.CardImage](#apidoc.module.botbuilder.CardImage)

#### <a name="apidoc.element.botbuilder.CardImage.CardImage"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardImage (session)](#apidoc.element.botbuilder.CardImage.CardImage)
- description and source-code
```javascript
function CardImage(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
...
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
...
```

#### <a name="apidoc.element.botbuilder.CardImage.create"></a>[function <span class="apidocSignatureSpan">botbuilder.CardImage.</span>create (session, url)](#apidoc.element.botbuilder.CardImage.create)
- description and source-code
```javascript
create = function (session, url) {
    return new CardImage(session).url(url);
}
```
- example usage
```shell
...



"use strict";
var __extends = (this && this.__extends) || function (d, b) {
    for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p];
    function __() { this.constructor = d; }
    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());
};
var Dialog_1 = require("./dialogs/Dialog");
var Message_1 = require("./Message");
var consts = require("./consts");
var logger = require("./logger");
var sprintf = require("sprintf-js");
var events = require("events");
...
```



# <a name="apidoc.module.botbuilder.CardImage.prototype"></a>[module botbuilder.CardImage.prototype](#apidoc.module.botbuilder.CardImage.prototype)

#### <a name="apidoc.element.botbuilder.CardImage.prototype.alt"></a>[function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>alt (text)](#apidoc.element.botbuilder.CardImage.prototype.alt)
- description and source-code
```javascript
alt = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.alt = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardImage.prototype.tap"></a>[function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>tap (action)](#apidoc.element.botbuilder.CardImage.prototype.tap)
- description and source-code
```javascript
tap = function (action) {
    if (action) {
        this.data.tap = action.toAction ? action.toAction() : action;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
...
```

#### <a name="apidoc.element.botbuilder.CardImage.prototype.toImage"></a>[function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>toImage ()](#apidoc.element.botbuilder.CardImage.prototype.toImage)
- description and source-code
```javascript
toImage = function () {
    return this.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardImage.prototype.url"></a>[function <span class="apidocSignatureSpan">botbuilder.CardImage.prototype.</span>url (u)](#apidoc.element.botbuilder.CardImage.prototype.url)
- description and source-code
```javascript
url = function (u) {
    if (u) {
        this.data.url = u;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
...
```



# <a name="apidoc.module.botbuilder.CardMedia"></a>[module botbuilder.CardMedia](#apidoc.module.botbuilder.CardMedia)

#### <a name="apidoc.element.botbuilder.CardMedia.CardMedia"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CardMedia (session)](#apidoc.element.botbuilder.CardMedia.CardMedia)
- description and source-code
```javascript
function CardMedia(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardMedia.create"></a>[function <span class="apidocSignatureSpan">botbuilder.CardMedia.</span>create (session, url)](#apidoc.element.botbuilder.CardMedia.create)
- description and source-code
```javascript
create = function (session, url) {
    return new CardMedia(session).url(url);
}
```
- example usage
```shell
...



"use strict";
var __extends = (this && this.__extends) || function (d, b) {
    for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p];
    function __() { this.constructor = d; }
    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());
};
var Dialog_1 = require("./dialogs/Dialog");
var Message_1 = require("./Message");
var consts = require("./consts");
var logger = require("./logger");
var sprintf = require("sprintf-js");
var events = require("events");
...
```



# <a name="apidoc.module.botbuilder.CardMedia.prototype"></a>[module botbuilder.CardMedia.prototype](#apidoc.module.botbuilder.CardMedia.prototype)

#### <a name="apidoc.element.botbuilder.CardMedia.prototype.profile"></a>[function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>profile (text)](#apidoc.element.botbuilder.CardMedia.prototype.profile)
- description and source-code
```javascript
profile = function (text) {
    if (text) {
        this.data.profile = text;
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardMedia.prototype.toMedia"></a>[function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>toMedia ()](#apidoc.element.botbuilder.CardMedia.prototype.toMedia)
- description and source-code
```javascript
toMedia = function () {
    return this.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CardMedia.prototype.url"></a>[function <span class="apidocSignatureSpan">botbuilder.CardMedia.prototype.</span>url (u)](#apidoc.element.botbuilder.CardMedia.prototype.url)
- description and source-code
```javascript
url = function (u) {
    if (u) {
        this.data.url = u;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
...
```



# <a name="apidoc.module.botbuilder.Channel"></a>[module botbuilder.Channel](#apidoc.module.botbuilder.Channel)

#### <a name="apidoc.element.botbuilder.Channel.getChannelId"></a>[function <span class="apidocSignatureSpan">botbuilder.Channel.</span>getChannelId (addressable)](#apidoc.element.botbuilder.Channel.getChannelId)
- description and source-code
```javascript
function getChannelId(addressable) {
    var channelId;
    if (addressable) {
        if (addressable.hasOwnProperty('message')) {
            channelId = addressable.message.address.channelId;
        }
        else if (addressable.hasOwnProperty('address')) {
            channelId = addressable.address.channelId;
        }
        else if (addressable.hasOwnProperty('channelId')) {
            channelId = addressable.channelId;
        }
    }
    return channelId ? channelId.toLowerCase() : '';
}
```
- example usage
```shell
...
}
exports.warn = warn;
function info(addressable, fmt) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    var channelId = Channel.getChannelId(addressable);
    if (channelId === Channel.channels.emulator || debugLoggingEnabled) {
        var prefix = getPrefix(addressable);
        var msg = args.length > 0 ? sprintf.vsprintf(fmt, args) : fmt;
        console.info(prefix + msg);
    }
}
exports.info = info;
...
```

#### <a name="apidoc.element.botbuilder.Channel.supportsCardActions"></a>[function <span class="apidocSignatureSpan">botbuilder.Channel.</span>supportsCardActions (session, buttonCnt)](#apidoc.element.botbuilder.Channel.supportsCardActions)
- description and source-code
```javascript
function supportsCardActions(session, buttonCnt) {
    if (buttonCnt === void 0) { buttonCnt = 100; }
    switch (getChannelId(session)) {
        case exports.channels.facebook:
        case exports.channels.skype:
        case exports.channels.msteams:
            return (buttonCnt <= 3);
        case exports.channels.slack:
        case exports.channels.emulator:
        case exports.channels.directline:
        case exports.channels.webchat:
            return (buttonCnt <= 100);
        default:
            return false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Channel.supportsKeyboards"></a>[function <span class="apidocSignatureSpan">botbuilder.Channel.</span>supportsKeyboards (session, buttonCnt)](#apidoc.element.botbuilder.Channel.supportsKeyboards)
- description and source-code
```javascript
function supportsKeyboards(session, buttonCnt) {
    if (buttonCnt === void 0) { buttonCnt = 100; }
    switch (getChannelId(session)) {
        case exports.channels.facebook:
            return (buttonCnt <= 10);
        case exports.channels.kik:
            return (buttonCnt <= 20);
        case exports.channels.slack:
        case exports.channels.telegram:
            return (buttonCnt <= 100);
        default:
            return false;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ChatConnector"></a>[module botbuilder.ChatConnector](#apidoc.module.botbuilder.ChatConnector)

#### <a name="apidoc.element.botbuilder.ChatConnector.ChatConnector"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ChatConnector (settings)](#apidoc.element.botbuilder.ChatConnector.ChatConnector)
- description and source-code
```javascript
function ChatConnector(settings) {
    if (settings === void 0) { settings = {}; }
    this.settings = settings;
    if (!this.settings.endpoint) {
        this.settings.endpoint = {
            refreshEndpoint: 'https://login.microsoftonline.com/botframework.com/oauth2/v2.0/token',
            refreshScope: 'https://api.botframework.com/.default',
            botConnectorOpenIdMetadata: this.settings.openIdMetadata || 'https://login.botframework.com/v1/.well-known/openidconfiguration
',
            botConnectorIssuer: 'https://api.botframework.com',
            botConnectorAudience: this.settings.appId,
            msaOpenIdMetadata: 'https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration',
            msaIssuer: 'https://sts.windows.net/72f988bf-86f1-41af-91ab-2d7cd011db47/',
            msaAudience: 'https://graph.microsoft.com',
            emulatorOpenIdMetadata: 'https://login.microsoftonline.com/botframework.com/v2.0/.well-known/openid-configuration',
            emulatorAudience: 'https://sts.windows.net/d6d49420-f39b-4df7-a1dc-d59a935871db/',
            emulatorIssuer: this.settings.appId,
            stateEndpoint: this.settings.stateEndpoint || 'https://state.botframework.com'
        };
    }
    this.botConnectorOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.botConnectorOpenIdMetadata);
    this.msaOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.msaOpenIdMetadata);
    this.emulatorOpenIdMetadata = new OpenIdMetadata_1.OpenIdMetadata(this.settings.endpoint.emulatorOpenIdMetadata);
}
```
- example usage
```shell
...

Create a file named app.js and say hello in a few lines of code.

var restify = require('restify');
var builder = require('botbuilder');

// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});
...
```



# <a name="apidoc.module.botbuilder.ChatConnector.prototype"></a>[module botbuilder.ChatConnector.prototype](#apidoc.module.botbuilder.ChatConnector.prototype)

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.addAccessToken"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>addAccessToken (options, cb)](#apidoc.element.botbuilder.ChatConnector.prototype.addAccessToken)
- description and source-code
```javascript
addAccessToken = function (options, cb) {
    this.addUserAgent(options);
    if (this.settings.appId && this.settings.appPassword) {
        this.getAccessToken(function (err, token) {
            if (!err && token) {
                options.headers = {
                    'Authorization': 'Bearer ' + token
                };
                cb(null);
            }
            else {
                cb(err);
            }
        });
    }
    else {
        cb(null);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.addUserAgent"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>addUserAgent (options)](#apidoc.element.botbuilder.ChatConnector.prototype.addUserAgent)
- description and source-code
```javascript
addUserAgent = function (options) {
    if (options.headers == null) {
        options.headers = {};
    }
    options.headers['User-Agent'] = USER_AGENT;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.authenticatedRequest"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>authenticatedRequest (options, callback, refresh)](#apidoc.element.botbuilder.ChatConnector.prototype.authenticatedRequest)
- description and source-code
```javascript
authenticatedRequest = function (options, callback, refresh) {
    var _this = this;
    if (refresh === void 0) { refresh = false; }
    if (refresh) {
        this.accessToken = null;
    }
    this.addAccessToken(options, function (err) {
        if (!err) {
            request(options, function (err, response, body) {
                if (!err) {
                    switch (response.statusCode) {
                        case 401:
                        case 403:
                            if (!refresh) {
                                _this.authenticatedRequest(options, callback, true);
                            }
                            else {
                                callback(null, response, body);
                            }
                            break;
                        default:
                            if (response.statusCode < 400) {
                                callback(null, response, body);
                            }
                            else {
                                var txt = "Request to '" + options.url + "' failed: [" + response.statusCode + "] " + response.statusMessage
;
                                callback(new Error(txt), response, null);
                            }
                            break;
                    }
                }
                else {
                    callback(err, null, null);
                }
            });
        }
        else {
            callback(err, null, null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>dispatch (msg, res)](#apidoc.element.botbuilder.ChatConnector.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (msg, res) {
    try {
        this.prepIncomingMessage(msg);
        logger.info(msg, 'ChatConnector: message received.');
        if (this.isInvoke(msg)) {
            this.onInvokeHandler(msg, function (err, body, status) {
                if (err) {
                    res.status(500);
                    res.end();
                    logger.error('Received error from invoke handler: ', err.message || '');
                }
                else {
                    res.send(status || 200, body);
                }
            });
        }
        else {
            this.onEventHandler([msg]);
            res.status(202);
            res.end();
        }
    }
    catch (e) {
        console.error(e instanceof Error ? e.stack : e.toString());
        res.status(500);
        res.end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.getAccessToken"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getAccessToken (cb)](#apidoc.element.botbuilder.ChatConnector.prototype.getAccessToken)
- description and source-code
```javascript
getAccessToken = function (cb) {
    var _this = this;
    if (!this.accessToken || new Date().getTime() >= this.accessTokenExpires) {
        var opt = {
            method: 'POST',
            url: this.settings.endpoint.refreshEndpoint,
            form: {
                grant_type: 'client_credentials',
                client_id: this.settings.appId,
                client_secret: this.settings.appPassword,
                scope: this.settings.endpoint.refreshScope
            }
        };
        request(opt, function (err, response, body) {
            if (!err) {
                if (body && response.statusCode < 300) {
                    var oauthResponse = JSON.parse(body);
                    _this.accessToken = oauthResponse.access_token;
                    _this.accessTokenExpires = new Date().getTime() + ((oauthResponse.expires_in - 300) * 1000);
                    cb(null, _this.accessToken);
                }
                else {
                    cb(new Error('Refresh access token failed with status code: ' + response.statusCode), null);
                }
            }
            else {
                cb(err, null);
            }
        });
    }
    else {
        cb(null, this.accessToken);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.getData"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getData (context, callback)](#apidoc.element.botbuilder.ChatConnector.prototype.getData)
- description and source-code
```javascript
getData = function (context, callback) {
    var _this = this;
    try {
        var root = this.getStoragePath(context.address);
        var list = [];
        if (context.userId) {
            if (context.persistUserData) {
                list.push({
                    field: 'userData',
                    url: root + '/users/' + encodeURIComponent(context.userId)
                });
            }
            if (context.conversationId) {
                list.push({
                    field: 'privateConversationData',
                    url: root + '/conversations/' + encodeURIComponent(context.conversationId) +
                        '/users/' + encodeURIComponent(context.userId)
                });
            }
        }
        if (context.persistConversationData && context.conversationId) {
            list.push({
                field: 'conversationData',
                url: root + '/conversations/' + encodeURIComponent(context.conversationId)
            });
        }
        var data = {};
        async.each(list, function (entry, cb) {
            var options = {
                method: 'GET',
                url: entry.url,
                json: true
            };
            _this.authenticatedRequest(options, function (err, response, body) {
                if (!err && body) {
                    var botData = body.data ? body.data : {};
                    if (typeof botData === 'string') {
                        zlib.gunzip(new Buffer(botData, 'base64'), function (err, result) {
                            if (!err) {
                                try {
                                    var txt = result.toString();
                                    data[entry.field + 'Hash'] = txt;
                                    data[entry.field] = JSON.parse(txt);
                                }
                                catch (e) {
                                    err = e;
                                }
                            }
                            cb(err);
                        });
                    }
                    else {
                        try {
                            data[entry.field + 'Hash'] = JSON.stringify(botData);
                            data[entry.field] = botData;
                        }
                        catch (e) {
                            err = e;
                        }
                        cb(err);
                    }
                }
                else {
                    cb(err);
                }
            });
        }, function (err) {
            if (!err) {
                callback(null, data);
            }
            else {
                var m = err.toString();
                callback(err instanceof Error ? err : new Error(m), null);
            }
        });
    }
    catch (e) {
        callback(e instanceof Error ? e : new Error(e.toString()), null);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.getStoragePath"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>getStoragePath (address)](#apidoc.element.botbuilder.ChatConnector.prototype.getStoragePath)
- description and source-code
```javascript
getStoragePath = function (address) {
    var path;
    switch (address.channelId) {
        case 'emulator':
            if (address.serviceUrl) {
                path = address.serviceUrl;
            }
            else {
                throw new Error('ChatConnector.getStoragePath() missing address.serviceUrl.');
            }
            break;
        default:
            path = this.settings.endpoint.stateEndpoint;
            break;
    }
    return path + '/v3/botstate/' + encodeURIComponent(address.channelId);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.isInvoke"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>isInvoke (message)](#apidoc.element.botbuilder.ChatConnector.prototype.isInvoke)
- description and source-code
```javascript
isInvoke = function (message) {
    return (message && message.type && message.type.toLowerCase() == consts.invokeType);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.listen"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>listen ()](#apidoc.element.botbuilder.ChatConnector.prototype.listen)
- description and source-code
```javascript
listen = function () {
    var _this = this;
    return function (req, res) {
        if (req.body) {
            _this.verifyBotFramework(req, res);
        }
        else {
            var requestData = '';
            req.on('data', function (chunk) {
                requestData += chunk;
            });
            req.on('end', function () {
                req.body = JSON.parse(requestData);
                _this.verifyBotFramework(req, res);
            });
        }
    };
}
```
- example usage
```shell
...
    var bot = new builder.UniversalBot(connector);
    bot.dialog('/', function (session) {
        session.send('Hello World');
    });

    // Setup Restify Server
    var server = restify.createServer();
    server.post('/api/messages', connector.listen());
    server.listen(process.env.port || 3978, function () {
        console.log('%s listening to %s', server.name, server.url);
    });

## Test your bot
Use the [Bot Framework Emulator](http://docs.botframework.com/connector/tools/bot-framework-emulator/) to test your bot on localhost
.
...
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.onEvent"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>onEvent (handler)](#apidoc.element.botbuilder.ChatConnector.prototype.onEvent)
- description and source-code
```javascript
onEvent = function (handler) {
    this.onEventHandler = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.onInvoke"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>onInvoke (handler)](#apidoc.element.botbuilder.ChatConnector.prototype.onInvoke)
- description and source-code
```javascript
onInvoke = function (handler) {
    this.onInvokeHandler = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.postMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>postMessage (msg, cb)](#apidoc.element.botbuilder.ChatConnector.prototype.postMessage)
- description and source-code
```javascript
postMessage = function (msg, cb) {
    logger.info(address, 'ChatConnector: sending message.');
    this.prepOutgoingMessage(msg);
    var address = msg.address;
    msg['from'] = address.bot;
    msg['recipient'] = address.user;
    delete msg.address;
    var path = '/v3/conversations/' + encodeURIComponent(address.conversation.id) + '/activities';
    if (address.id && address.channelId !== 'skype') {
        path += '/' + encodeURIComponent(address.id);
    }
    var options = {
        method: 'POST',
        url: urlJoin(address.serviceUrl, path),
        body: msg,
        json: true
    };
    if (address.useAuth) {
        this.authenticatedRequest(options, function (err, response, body) { return cb(err); });
    }
    else {
        this.addUserAgent(options);
        request(options, function (err, response, body) {
            if (!err && response.statusCode >= 400) {
                var txt = "Request to '" + options.url + "' failed: [" + response.statusCode + "] " + response.statusMessage;
                err = new Error(txt);
            }
            cb(err);
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.prepIncomingMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>prepIncomingMessage (msg)](#apidoc.element.botbuilder.ChatConnector.prototype.prepIncomingMessage)
- description and source-code
```javascript
prepIncomingMessage = function (msg) {
    utils.moveFieldsTo(msg, msg, {
        'locale': 'textLocale',
        'channelData': 'sourceEvent'
    });
    msg.text = msg.text || '';
    msg.attachments = msg.attachments || [];
    msg.entities = msg.entities || [];
    var address = {};
    utils.moveFieldsTo(msg, address, toAddress);
    msg.address = address;
    msg.source = address.channelId;
    if (msg.source == 'facebook' && msg.sourceEvent && msg.sourceEvent.message && msg.sourceEvent.message.quick_reply) {
        msg.text = msg.sourceEvent.message.quick_reply.payload;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.prepOutgoingMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>prepOutgoingMessage (msg)](#apidoc.element.botbuilder.ChatConnector.prototype.prepOutgoingMessage)
- description and source-code
```javascript
prepOutgoingMessage = function (msg) {
    if (msg.attachments) {
        var attachments = [];
        for (var i = 0; i < msg.attachments.length; i++) {
            var a = msg.attachments[i];
            switch (a.contentType) {
                case 'application/vnd.microsoft.keyboard':
                    if (msg.address.channelId == 'facebook') {
                        msg.sourceEvent = { quick_replies: [] };
                        a.content.buttons.forEach(function (action) {
                            switch (action.type) {
                                case 'imBack':
                                case 'postBack':
                                    msg.sourceEvent.quick_replies.push({
                                        content_type: 'text',
                                        title: action.title,
                                        payload: action.value
                                    });
                                    break;
                                default:
                                    logger.warn(msg, "Invalid keyboard '%s' button sent to facebook.", action.type);
                                    break;
                            }
                        });
                    }
                    else {
                        a.contentType = 'application/vnd.microsoft.card.hero';
                        attachments.push(a);
                    }
                    break;
                default:
                    attachments.push(a);
                    break;
            }
        }
        msg.attachments = attachments;
    }
    utils.moveFieldsTo(msg, msg, {
        'textLocale': 'locale',
        'sourceEvent': 'channelData'
    });
    delete msg.agent;
    delete msg.source;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.saveData"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>saveData (context, data, callback)](#apidoc.element.botbuilder.ChatConnector.prototype.saveData)
- description and source-code
```javascript
saveData = function (context, data, callback) {
    var _this = this;
    var list = [];
    function addWrite(field, botData, url) {
        var hashKey = field + 'Hash';
        var hash = JSON.stringify(botData);
        if (!data[hashKey] || hash !== data[hashKey]) {
            data[hashKey] = hash;
            list.push({ botData: botData, url: url, hash: hash });
        }
    }
    try {
        var root = this.getStoragePath(context.address);
        if (context.userId) {
            if (context.persistUserData) {
                addWrite('userData', data.userData || {}, root + '/users/' + encodeURIComponent(context.userId));
            }
            if (context.conversationId) {
                var url = root + '/conversations/' + encodeURIComponent(context.conversationId) +
                    '/users/' + encodeURIComponent(context.userId);
                addWrite('privateConversationData', data.privateConversationData || {}, url);
            }
        }
        if (context.persistConversationData && context.conversationId) {
            addWrite('conversationData', data.conversationData || {}, root + '/conversations/' + encodeURIComponent(context.conversationId
));
        }
        async.each(list, function (entry, cb) {
            if (_this.settings.gzipData) {
                zlib.gzip(entry.hash, function (err, result) {
                    if (!err && result.length > MAX_DATA_LENGTH) {
                        err = new Error("Data of " + result.length + " bytes gzipped exceeds the " + MAX_DATA_LENGTH + " byte limit
. Can't post to: " + entry.url);
                        err.code = consts.Errors.EMSGSIZE;
                    }
                    if (!err) {
                        var options = {
                            method: 'POST',
                            url: entry.url,
                            body: { eTag: '*', data: result.toString('base64') },
                            json: true
                        };
                        _this.authenticatedRequest(options, function (err, response, body) {
                            cb(err);
                        });
                    }
                    else {
                        cb(err);
                    }
                });
            }
            else if (entry.hash.length < MAX_DATA_LENGTH) {
                var options = {
                    method: 'POST',
                    url: entry.url,
                    body: { eTag: '*', data: entry.botData },
                    json: true
                };
                _this.authenticatedRequest(options, function (err, response, body) {
                    cb(err);
                });
            }
            else {
                var err = new Error("Data of " + entry.hash.length + " bytes exceeds the " + MAX_DATA_LENGTH + " byte limit. Consider
 setting connectors gzipData option. Can't post to: " + entry.url);
                err.code = consts.Errors.EMSGSIZE;
                cb(err);
            }
        }, function (err) {
            if (callback) {
                if (!err) {
                    callback(null);
                }
                else {
                    var m = err.toString();
                    callback(err instanceof Error ? err : new Error(m));
                }
            }
        });
    }
    catch (e) {
        if (callback) {
            var err = e instanceof Error ? e : new Error(e.toString());
            err.code = consts.Errors.EBADMSG;
            callback(err);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.send"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.ChatConnector.prototype.send)
- description and source-code
```javascript
send = function (messages, done) {
    var _this = this;
    async.eachSeries(messages, function (msg, cb) {
        try {
            if (msg.address && msg.address.serviceUrl) {
                _this.postMessage(msg, cb);
            }
            else {
                logger.error('ChatConnector: send - message is missing address or serviceUrl.');
                cb(new Error('Message missing address or serviceUrl.'));
            }
        }
        catch (e) {
            cb(e);
        }
    }, done);
}
```
- example usage
```shell
...
// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
    console.log('%s listening to %s', server.name, server.url);
...
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.startConversation"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>startConversation (address, done)](#apidoc.element.botbuilder.ChatConnector.prototype.startConversation)
- description and source-code
```javascript
startConversation = function (address, done) {
    if (address && address.user && address.bot && address.serviceUrl) {
        var options = {
            method: 'POST',
            url: urlJoin(address.serviceUrl, '/v3/conversations'),
            body: {
                bot: address.bot,
                members: [address.user]
            },
            json: true
        };
        this.authenticatedRequest(options, function (err, response, body) {
            var adr;
            if (!err) {
                try {
                    var obj = typeof body === 'string' ? JSON.parse(body) : body;
                    if (obj && obj.hasOwnProperty('id')) {
                        adr = utils.clone(address);
                        adr.conversation = { id: obj['id'] };
                        if (adr.id) {
                            delete adr.id;
                        }
                    }
                    else {
                        err = new Error('Failed to start conversation: no conversation ID returned.');
                    }
                }
                catch (e) {
                    err = e instanceof Error ? e : new Error(e.toString());
                }
            }
            if (err) {
                logger.error('ChatConnector: startConversation - error starting conversation.');
            }
            done(err, adr);
        });
    }
    else {
        logger.error('ChatConnector: startConversation - address is invalid.');
        done(new Error('Invalid address.'));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ChatConnector.prototype.verifyBotFramework"></a>[function <span class="apidocSignatureSpan">botbuilder.ChatConnector.prototype.</span>verifyBotFramework (req, res)](#apidoc.element.botbuilder.ChatConnector.prototype.verifyBotFramework)
- description and source-code
```javascript
verifyBotFramework = function (req, res) {
    var _this = this;
    var token;
    var isEmulator = req.body['channelId'] === 'emulator';
    var authHeaderValue = req.headers ? req.headers['authorization'] || req.headers['Authorization'] : null;
    if (authHeaderValue) {
        var auth = authHeaderValue.trim().split(' ');
        if (auth.length == 2 && auth[0].toLowerCase() == 'bearer') {
            token = auth[1];
        }
    }
    if (token) {
        req.body['useAuth'] = true;
        var decoded = jwt.decode(token, { complete: true });
        var verifyOptions;
        var openIdMetadata;
        if (isEmulator && decoded.payload.iss == this.settings.endpoint.msaIssuer) {
            openIdMetadata = this.msaOpenIdMetadata;
            verifyOptions = {
                issuer: this.settings.endpoint.msaIssuer,
                audience: this.settings.endpoint.msaAudience,
                clockTolerance: 300
            };
        }
        else if (isEmulator && decoded.payload.iss == this.settings.endpoint.emulatorIssuer) {
            openIdMetadata = this.emulatorOpenIdMetadata;
            verifyOptions = {
                issuer: this.settings.endpoint.emulatorIssuer,
                audience: this.settings.endpoint.emulatorAudience,
                clockTolerance: 300
            };
        }
        else {
            openIdMetadata = this.botConnectorOpenIdMetadata;
            verifyOptions = {
                issuer: this.settings.endpoint.botConnectorIssuer,
                audience: this.settings.endpoint.botConnectorAudience,
                clockTolerance: 300
            };
        }
        if (isEmulator && decoded.payload.appid != this.settings.appId) {
            logger.error('ChatConnector: receive - invalid token. Requested by unexpected app ID.');
            res.status(403);
            res.end();
            return;
        }
        openIdMetadata.getKey(decoded.header.kid, function (key) {
            if (key) {
                try {
                    jwt.verify(token, key, verifyOptions);
                }
                catch (err) {
                    logger.error('ChatConnector: receive - invalid token. Check bot\'s app ID & Password.');
                    res.status(403);
                    res.end();
                    return;
                }
                _this.dispatch(req.body, res);
            }
            else {
                logger.error('ChatConnector: receive - invalid signing key or OpenId metadata document.');
                res.status(500);
                res.end();
                return;
            }
        });
    }
    else if (isEmulator && !this.settings.appId && !this.settings.appPassword) {
        logger.warn(req.body, 'ChatConnector: receive - emulator running without security enabled.');
        req.body['useAuth'] = false;
        this.dispatch(req.body, res);
    }
    else {
        logger.error('ChatConnector: receive - no security token sent.');
        res.status(401);
        res.end();
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.CommandDialog"></a>[module botbuilder.CommandDialog](#apidoc.module.botbuilder.CommandDialog)

#### <a name="apidoc.element.botbuilder.CommandDialog.CommandDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>CommandDialog (serviceUri)](#apidoc.element.botbuilder.CommandDialog.CommandDialog)
- description and source-code
```javascript
function CommandDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('CommandDialog class is deprecated. Use IntentDialog class instead.');
    _this.dialog = new IntentDialog_1.IntentDialog();
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.CommandDialog.prototype"></a>[module botbuilder.CommandDialog.prototype](#apidoc.module.botbuilder.CommandDialog.prototype)

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.CommandDialog.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    this.dialog.begin(session, args);
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>constructor (serviceUri)](#apidoc.element.botbuilder.CommandDialog.prototype.constructor)
- description and source-code
```javascript
function CommandDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('CommandDialog class is deprecated. Use IntentDialog class instead.');
    _this.dialog = new IntentDialog_1.IntentDialog();
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.CommandDialog.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    this.dialog.dialogResumed(session, result);
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.matches"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>matches (patterns, dialogId, dialogArgs)](#apidoc.element.botbuilder.CommandDialog.prototype.matches)
- description and source-code
```javascript
matches = function (patterns, dialogId, dialogArgs) {
    var _this = this;
    var list = (!Array.isArray(patterns) ? [patterns] : patterns);
    list.forEach(function (p) {
        _this.dialog.matches(new RegExp(p, 'i'), dialogId, dialogArgs);
    });
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.onBegin"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.CommandDialog.prototype.onBegin)
- description and source-code
```javascript
onBegin = function (handler) {
    this.dialog.onBegin(handler);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.onDefault"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.CommandDialog.prototype.onDefault)
- description and source-code
```javascript
onDefault = function (dialogId, dialogArgs) {
    this.dialog.onDefault(dialogId, dialogArgs);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.CommandDialog.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    this.dialog.recognize(context, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.CommandDialog.prototype.replyReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.CommandDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.CommandDialog.prototype.replyReceived)
- description and source-code
```javascript
replyReceived = function (session, recognizeResult) {
}
```
- example usage
```shell
...
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
...
```



# <a name="apidoc.module.botbuilder.ConsoleConnector"></a>[module botbuilder.ConsoleConnector](#apidoc.module.botbuilder.ConsoleConnector)

#### <a name="apidoc.element.botbuilder.ConsoleConnector.ConsoleConnector"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ConsoleConnector ()](#apidoc.element.botbuilder.ConsoleConnector.ConsoleConnector)
- description and source-code
```javascript
function ConsoleConnector() {
    this.replyCnt = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ConsoleConnector.prototype"></a>[module botbuilder.ConsoleConnector.prototype](#apidoc.module.botbuilder.ConsoleConnector.prototype)

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.listen"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>listen ()](#apidoc.element.botbuilder.ConsoleConnector.prototype.listen)
- description and source-code
```javascript
listen = function () {
    var _this = this;
    this.rl = readline.createInterface({ input: process.stdin, output: process.stdout, terminal: false });
    this.rl.on('line', function (line) {
        _this.replyCnt = 0;
        line = line || '';
        if (line.toLowerCase() == 'quit') {
            _this.rl.close();
            process.exit();
        }
        else {
            _this.processMessage(line);
        }
    });
    return this;
}
```
- example usage
```shell
...
    var bot = new builder.UniversalBot(connector);
    bot.dialog('/', function (session) {
        session.send('Hello World');
    });

    // Setup Restify Server
    var server = restify.createServer();
    server.post('/api/messages', connector.listen());
    server.listen(process.env.port || 3978, function () {
        console.log('%s listening to %s', server.name, server.url);
    });

## Test your bot
Use the [Bot Framework Emulator](http://docs.botframework.com/connector/tools/bot-framework-emulator/) to test your bot on localhost
.
...
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.onEvent"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>onEvent (handler)](#apidoc.element.botbuilder.ConsoleConnector.prototype.onEvent)
- description and source-code
```javascript
onEvent = function (handler) {
    this.onEventHandler = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.onInvoke"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>onInvoke (handler)](#apidoc.element.botbuilder.ConsoleConnector.prototype.onInvoke)
- description and source-code
```javascript
onInvoke = function (handler) {
    this.onInvokeHandler = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.processMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>processMessage (line)](#apidoc.element.botbuilder.ConsoleConnector.prototype.processMessage)
- description and source-code
```javascript
processMessage = function (line) {
    if (this.onEventHandler) {
        var msg = new Message_1.Message()
            .address({
            channelId: 'console',
            user: { id: 'user', name: 'User1' },
            bot: { id: 'bot', name: 'Bot' },
            conversation: { id: 'Convo1' }
        })
            .timestamp()
            .text(line);
        this.onEventHandler([msg.toMessage()]);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.send"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.ConsoleConnector.prototype.send)
- description and source-code
```javascript
send = function (messages, done) {
    for (var i = 0; i < messages.length; i++) {
        if (this.replyCnt++ > 0) {
            console.log();
        }
        var msg = messages[i];
        if (msg.text) {
            log(msg.text);
        }
        if (msg.attachments && msg.attachments.length > 0) {
            for (var j = 0; j < msg.attachments.length; j++) {
                if (j > 0) {
                    console.log();
                }
                renderAttachment(msg.attachments[j]);
            }
        }
    }
    done(null);
}
```
- example usage
```shell
...
// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
    console.log('%s listening to %s', server.name, server.url);
...
```

#### <a name="apidoc.element.botbuilder.ConsoleConnector.prototype.startConversation"></a>[function <span class="apidocSignatureSpan">botbuilder.ConsoleConnector.prototype.</span>startConversation (address, cb)](#apidoc.element.botbuilder.ConsoleConnector.prototype.startConversation)
- description and source-code
```javascript
startConversation = function (address, cb) {
    var adr = utils.clone(address);
    adr.conversation = { id: 'Convo1' };
    cb(null, adr);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.DefaultLocalizer"></a>[module botbuilder.DefaultLocalizer](#apidoc.module.botbuilder.DefaultLocalizer)

#### <a name="apidoc.element.botbuilder.DefaultLocalizer.DefaultLocalizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>DefaultLocalizer (root, defaultLocale)](#apidoc.element.botbuilder.DefaultLocalizer.DefaultLocalizer)
- description and source-code
```javascript
function DefaultLocalizer(root, defaultLocale) {
    this.localePaths = [];
    this.locales = {};
    this.defaultLocale(defaultLocale || 'en');
    var libsSeen = {};
    var _that = this;
    function addPaths(library) {
        if (!libsSeen.hasOwnProperty(library.name)) {
            libsSeen[library.name] = true;
            library.forEachLibrary(function (child) {
                addPaths(child);
            });
            var path = library.localePath();
            if (path) {
                _that.localePaths.push(path);
            }
        }
    }
    addPaths(root);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Dialog"></a>[module botbuilder.Dialog](#apidoc.module.botbuilder.Dialog)

#### <a name="apidoc.element.botbuilder.Dialog.Dialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Dialog ()](#apidoc.element.botbuilder.Dialog.Dialog)
- description and source-code
```javascript
function Dialog() {
    return _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Dialog.prototype"></a>[module botbuilder.Dialog.prototype](#apidoc.module.botbuilder.Dialog.prototype)

#### <a name="apidoc.element.botbuilder.Dialog.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.Dialog.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    this.replyReceived(session);
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.Dialog.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>constructor ()](#apidoc.element.botbuilder.Dialog.prototype.constructor)
- description and source-code
```javascript
function Dialog() {
    return _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Dialog.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.Dialog.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    if (result.error) {
        session.error(result.error);
    }
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.Dialog.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.Dialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.Dialog.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    cb(null, { score: 0.1 });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.DialogAction"></a>[module botbuilder.DialogAction](#apidoc.module.botbuilder.DialogAction)

#### <a name="apidoc.element.botbuilder.DialogAction.DialogAction"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>DialogAction ()](#apidoc.element.botbuilder.DialogAction.DialogAction)
- description and source-code
```javascript
function DialogAction() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.DialogAction.beginDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>beginDialog (id, args)](#apidoc.element.botbuilder.DialogAction.beginDialog)
- description and source-code
```javascript
beginDialog = function (id, args) {
    return function beginDialogAction(s, a) {
        if (a && a.hasOwnProperty('resumed')) {
            var r = a;
            if (r.error) {
                s.error(r.error);
            }
        }
        else {
            if (args) {
                a = a || {};
                for (var key in args) {
                    if (args.hasOwnProperty(key)) {
                        a[key] = args[key];
                    }
                }
            }
            s.beginDialog(id, a);
        }
    };
}
```
- example usage
```shell
...
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
...
```

#### <a name="apidoc.element.botbuilder.DialogAction.endDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>endDialog (result)](#apidoc.element.botbuilder.DialogAction.endDialog)
- description and source-code
```javascript
endDialog = function (result) {
    return function endDialogAction(s) {
        s.endDialog(result);
    };
}
```
- example usage
```shell
...
};
Session.prototype.endDialog = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (typeof message === 'object' && (message.hasOwnProperty('response') || message.hasOwnProperty('resumed') || message.hasOwnProperty
('error'))) {
        console.warn('Returning results via Session.endDialog() is deprecated. Use Session.endDialogWithResult() instead.');
        return this.endDialogWithResult(message);
    }
    var cur = this.curDialog();
    if (cur) {
        var m;
        if (message) {
            if (typeof message == 'string' || Array.isArray(message)) {
...
```

#### <a name="apidoc.element.botbuilder.DialogAction.send"></a>[function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>send (msg)](#apidoc.element.botbuilder.DialogAction.send)
- description and source-code
```javascript
send = function (msg) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    args.splice(0, 0, msg);
    return function sendAction(s) {
        Session_1.Session.prototype.send.apply(s, args);
    };
}
```
- example usage
```shell
...
// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
    console.log('%s listening to %s', server.name, server.url);
...
```

#### <a name="apidoc.element.botbuilder.DialogAction.validatedPrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.DialogAction.</span>validatedPrompt (promptType, validator)](#apidoc.element.botbuilder.DialogAction.validatedPrompt)
- description and source-code
```javascript
validatedPrompt = function (promptType, validator) {
    return new SimpleDialog_1.SimpleDialog(function (s, r) {
        r = r || {};
        var valid = false;
        if (r.response) {
            try {
                valid = validator(r.response);
            }
            catch (e) {
                s.error(e);
            }
        }
        var canceled = false;
        switch (r.resumed) {
            case Dialog_1.ResumeReason.canceled:
            case Dialog_1.ResumeReason.forward:
            case Dialog_1.ResumeReason.back:
                canceled = true;
                break;
        }
        if (valid || canceled) {
            s.endDialogWithResult(r);
        }
        else if (!s.dialogData.hasOwnProperty('prompt')) {
            s.dialogData = utils.clone(r);
            s.dialogData.promptType = promptType;
            if (!s.dialogData.hasOwnProperty('maxRetries')) {
                s.dialogData.maxRetries = 2;
            }
            var a = utils.clone(s.dialogData);
            a.maxRetries = 0;
            s.beginDialog(consts.DialogId.Prompts, a);
        }
        else if (s.dialogData.maxRetries > 0) {
            s.dialogData.maxRetries--;
            var a = utils.clone(s.dialogData);
            a.maxRetries = 0;
            a.prompt = s.dialogData.retryPrompt || "I didn't understand. " + s.dialogData.prompt;
            s.beginDialog(consts.DialogId.Prompts, a);
        }
        else {
            s.endDialogWithResult({ resumed: Dialog_1.ResumeReason.notCompleted });
        }
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.EntityRecognizer"></a>[module botbuilder.EntityRecognizer](#apidoc.module.botbuilder.EntityRecognizer)

#### <a name="apidoc.element.botbuilder.EntityRecognizer.EntityRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>EntityRecognizer ()](#apidoc.element.botbuilder.EntityRecognizer.EntityRecognizer)
- description and source-code
```javascript
function EntityRecognizer() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.expandChoices"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>expandChoices (choices)](#apidoc.element.botbuilder.EntityRecognizer.expandChoices)
- description and source-code
```javascript
expandChoices = function (choices) {
    if (!choices) {
        return [];
    }
    else if (Array.isArray(choices)) {
        return choices;
    }
    else if (typeof choices == 'string') {
        return choices.split('|');
    }
    else if (typeof choices == 'object') {
        var list = [];
        for (var key in choices) {
            list.push(key);
        }
        return list;
    }
    else {
        return [choices.toString()];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.findAllEntities"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findAllEntities (entities, type)](#apidoc.element.botbuilder.EntityRecognizer.findAllEntities)
- description and source-code
```javascript
findAllEntities = function (entities, type) {
    var found = [];
    for (var i = 0; entities && i < entities.length; i++) {
        if (entities[i].type == type) {
            found.push(entities[i]);
        }
    }
    return found;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.findAllMatches"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findAllMatches (choices, utterance, threshold)](#apidoc.element.botbuilder.EntityRecognizer.findAllMatches)
- description and source-code
```javascript
findAllMatches = function (choices, utterance, threshold) {
    if (threshold === void 0) { threshold = 0.6; }
    var matches = [];
    utterance = utterance.trim().toLowerCase();
    var tokens = utterance.split(' ');
    EntityRecognizer.expandChoices(choices).forEach(function (choice, index) {
        var score = 0.0;
        var value = choice.trim().toLowerCase();
        if (value.indexOf(utterance) >= 0) {
            score = utterance.length / value.length;
        }
        else if (utterance.indexOf(value) >= 0) {
            score = Math.min(0.5 + (value.length / utterance.length), 0.9);
        }
        else {
            var matched = '';
            tokens.forEach(function (token) {
                if (value.indexOf(token) >= 0) {
                    matched += token;
                }
            });
            score = matched.length / value.length;
        }
        if (score >= threshold) {
            matches.push({ index: index, entity: choice, score: score });
        }
    });
    return matches;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.findBestMatch"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findBestMatch (choices, utterance, threshold)](#apidoc.element.botbuilder.EntityRecognizer.findBestMatch)
- description and source-code
```javascript
findBestMatch = function (choices, utterance, threshold) {
    if (threshold === void 0) { threshold = 0.6; }
    var best;
    var matches = EntityRecognizer.findAllMatches(choices, utterance, threshold);
    matches.forEach(function (value) {
        if (!best || value.score > best.score) {
            best = value;
        }
    });
    return best;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.findEntity"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>findEntity (entities, type)](#apidoc.element.botbuilder.EntityRecognizer.findEntity)
- description and source-code
```javascript
findEntity = function (entities, type) {
    for (var i = 0; entities && i < entities.length; i++) {
        if (entities[i].type == type) {
            return entities[i];
        }
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.parseBoolean"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseBoolean (utterance)](#apidoc.element.botbuilder.EntityRecognizer.parseBoolean)
- description and source-code
```javascript
parseBoolean = function (utterance) {
    utterance = utterance.trim();
    if (EntityRecognizer.yesExp.test(utterance)) {
        return true;
    }
    else if (EntityRecognizer.noExp.test(utterance)) {
        return false;
    }
    return undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.parseNumber"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseNumber (entities)](#apidoc.element.botbuilder.EntityRecognizer.parseNumber)
- description and source-code
```javascript
parseNumber = function (entities) {
    var entity;
    if (typeof entities == 'string') {
        entity = { type: 'text', entity: entities.trim() };
    }
    else {
        entity = EntityRecognizer.findEntity(entities, 'builtin.number');
    }
    if (entity) {
        var match = this.numberExp.exec(entity.entity);
        if (match) {
            return Number(match[0]);
        }
        var oWordMatch = this.findBestMatch(this.ordinalWords, entity.entity, 1.0);
        if (oWordMatch) {
            return oWordMatch.index + 1;
        }
    }
    return Number.NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.parseTime"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>parseTime (entities)](#apidoc.element.botbuilder.EntityRecognizer.parseTime)
- description and source-code
```javascript
parseTime = function (entities) {
    if (typeof entities == 'string') {
        entities = [EntityRecognizer.recognizeTime(entities)];
    }
    return EntityRecognizer.resolveTime(entities);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.recognizeTime"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>recognizeTime (utterance, refDate)](#apidoc.element.botbuilder.EntityRecognizer.recognizeTime)
- description and source-code
```javascript
recognizeTime = function (utterance, refDate) {
    var response;
    try {
        var results = chrono.parse(utterance, refDate);
        if (results && results.length > 0) {
            var duration = results[0];
            response = {
                type: 'chrono.duration',
                entity: duration.text,
                startIndex: duration.index,
                endIndex: duration.index + duration.text.length,
                resolution: {
                    resolution_type: 'chrono.duration',
                    start: duration.start.date()
                }
            };
            if (duration.end) {
                response.resolution.end = duration.end.date();
            }
            if (duration.ref) {
                response.resolution.ref = duration.ref;
            }
            response.score = duration.text.length / utterance.length;
        }
    }
    catch (err) {
        console.error('Error recognizing time: ' + err.toString());
        response = null;
    }
    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.EntityRecognizer.resolveTime"></a>[function <span class="apidocSignatureSpan">botbuilder.EntityRecognizer.</span>resolveTime (entities)](#apidoc.element.botbuilder.EntityRecognizer.resolveTime)
- description and source-code
```javascript
resolveTime = function (entities) {
    var _this = this;
    var now = new Date();
    var resolvedDate;
    var date;
    var time;
    entities.forEach(function (entity) {
        if (entity.resolution) {
            switch (entity.resolution.resolution_type || entity.type) {
                case 'builtin.datetime':
                case 'builtin.datetime.date':
                case 'builtin.datetime.time':
                    var parts = (entity.resolution.date || entity.resolution.time).split('T');
                    if (!date && _this.dateExp.test(parts[0])) {
                        date = parts[0];
                    }
                    if (!time && parts[1]) {
                        time = 'T' + parts[1];
                        if (time == 'TMO') {
                            time = 'T08:00:00';
                        }
                        else if (time == 'TNI') {
                            time = 'T20:00:00';
                        }
                        else if (time.length == 3) {
                            time = time + ':00:00';
                        }
                        else if (time.length == 6) {
                            time = time + ':00';
                        }
                    }
                    break;
                case 'chrono.duration':
                    var duration = entity;
                    resolvedDate = duration.resolution.start;
            }
        }
    });
    if (!resolvedDate && (date || time)) {
        if (!date) {
            date = utils.toDate8601(now);
        }
        if (time) {
            date += time;
        }
        resolvedDate = new Date(date);
    }
    return resolvedDate;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Fact"></a>[module botbuilder.Fact](#apidoc.module.botbuilder.Fact)

#### <a name="apidoc.element.botbuilder.Fact.Fact"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Fact (session)](#apidoc.element.botbuilder.Fact.Fact)
- description and source-code
```javascript
function Fact(session) {
    this.session = session;
    this.data = { value: '' };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Fact.create"></a>[function <span class="apidocSignatureSpan">botbuilder.Fact.</span>create (session, value, key)](#apidoc.element.botbuilder.Fact.create)
- description and source-code
```javascript
create = function (session, value, key) {
    return new Fact(session).value(value).key(key);
}
```
- example usage
```shell
...



"use strict";
var __extends = (this && this.__extends) || function (d, b) {
    for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p];
    function __() { this.constructor = d; }
    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());
};
var Dialog_1 = require("./dialogs/Dialog");
var Message_1 = require("./Message");
var consts = require("./consts");
var logger = require("./logger");
var sprintf = require("sprintf-js");
var events = require("events");
...
```



# <a name="apidoc.module.botbuilder.Fact.prototype"></a>[module botbuilder.Fact.prototype](#apidoc.module.botbuilder.Fact.prototype)

#### <a name="apidoc.element.botbuilder.Fact.prototype.key"></a>[function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>key (text)](#apidoc.element.botbuilder.Fact.prototype.key)
- description and source-code
```javascript
key = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.key = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Fact.prototype.toFact"></a>[function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>toFact ()](#apidoc.element.botbuilder.Fact.prototype.toFact)
- description and source-code
```javascript
toFact = function () {
    return this.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Fact.prototype.value"></a>[function <span class="apidocSignatureSpan">botbuilder.Fact.prototype.</span>value (v)](#apidoc.element.botbuilder.Fact.prototype.value)
- description and source-code
```javascript
value = function (v) {
    this.data.value = v || '';
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.HeroCard"></a>[module botbuilder.HeroCard](#apidoc.module.botbuilder.HeroCard)

#### <a name="apidoc.element.botbuilder.HeroCard.HeroCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>HeroCard (session)](#apidoc.element.botbuilder.HeroCard.HeroCard)
- description and source-code
```javascript
function HeroCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.hero';
    return _this;
}
```
- example usage
```shell
...
            isOldSchema = true;
            break;
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
...
```



# <a name="apidoc.module.botbuilder.HeroCard.prototype"></a>[module botbuilder.HeroCard.prototype](#apidoc.module.botbuilder.HeroCard.prototype)

#### <a name="apidoc.element.botbuilder.HeroCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.HeroCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.HeroCard.prototype.constructor)
- description and source-code
```javascript
function HeroCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.hero';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.IntentDialog"></a>[module botbuilder.IntentDialog](#apidoc.module.botbuilder.IntentDialog)

#### <a name="apidoc.element.botbuilder.IntentDialog.IntentDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>IntentDialog (options)](#apidoc.element.botbuilder.IntentDialog.IntentDialog)
- description and source-code
```javascript
function IntentDialog(options) {
    if (options === void 0) { options = {}; }
    var _this = _super.call(this) || this;
    _this.handlers = {};
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet(options);
    if (typeof options.recognizeMode !== "undefined") {
        _this.recognizeMode = options.recognizeMode;
    }
    else {
        _this.recognizeMode = RecognizeMode.onBeginIfRoot;
    }
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.IntentDialog.prototype"></a>[module botbuilder.IntentDialog.prototype](#apidoc.module.botbuilder.IntentDialog.prototype)

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.IntentDialog.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    var _this = this;
    var mode = this.recognizeMode;
    var isRoot = (session.sessionState.callstack.length == 1);
    var recognize = (mode == RecognizeMode.onBegin || (isRoot && mode == RecognizeMode.onBeginIfRoot));
    if (this.beginDialog) {
        try {
            logger.info(session, 'IntentDialog.begin()');
            this.beginDialog(session, args, function () {
                if (recognize) {
                    _this.replyReceived(session);
                }
            });
        }
        catch (e) {
            this.emitError(session, e);
        }
    }
    else if (recognize) {
        this.replyReceived(session);
    }
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>constructor (options)](#apidoc.element.botbuilder.IntentDialog.prototype.constructor)
- description and source-code
```javascript
function IntentDialog(options) {
    if (options === void 0) { options = {}; }
    var _this = _super.call(this) || this;
    _this.handlers = {};
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet(options);
    if (typeof options.recognizeMode !== "undefined") {
        _this.recognizeMode = options.recognizeMode;
    }
    else {
        _this.recognizeMode = RecognizeMode.onBeginIfRoot;
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.IntentDialog.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    var activeIntent = session.dialogData[consts.Data.Intent];
    if (activeIntent && this.handlers.hasOwnProperty(activeIntent)) {
        try {
            this.handlers[activeIntent](session, result);
        }
        catch (e) {
            this.emitError(session, e);
        }
    }
    else {
        _super.prototype.dialogResumed.call(this, session, result);
    }
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.emitError"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>emitError (session, err)](#apidoc.element.botbuilder.IntentDialog.prototype.emitError)
- description and source-code
```javascript
emitError = function (session, err) {
    var m = err.toString();
    err = err instanceof Error ? err : new Error(m);
    session.error(err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.invokeIntent"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>invokeIntent (session, recognizeResult)](#apidoc.element.botbuilder.IntentDialog.prototype.invokeIntent)
- description and source-code
```javascript
invokeIntent = function (session, recognizeResult) {
    var activeIntent;
    if (recognizeResult.intent && this.handlers.hasOwnProperty(recognizeResult.intent)) {
        logger.info(session, 'IntentDialog.matches(%s)', recognizeResult.intent);
        activeIntent = recognizeResult.intent;
    }
    else if (this.handlers.hasOwnProperty(consts.Intents.Default)) {
        logger.info(session, 'IntentDialog.onDefault()');
        activeIntent = consts.Intents.Default;
    }
    if (activeIntent) {
        try {
            session.dialogData[consts.Data.Intent] = activeIntent;
            this.handlers[activeIntent](session, recognizeResult);
        }
        catch (e) {
            this.emitError(session, e);
        }
    }
    else {
        logger.warn(session, 'IntentDialog - no intent handler found for %s', recognizeResult.intent);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.matches"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>matches (intent, dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.matches)
- description and source-code
```javascript
matches = function (intent, dialogId, dialogArgs) {
    var id;
    if (intent) {
        if (typeof intent === 'string') {
            id = intent;
        }
        else {
            id = intent.toString();
            this.recognizers.recognizer(new RegExpRecognizer_1.RegExpRecognizer(id, intent));
        }
    }
    if (this.handlers.hasOwnProperty(id)) {
        throw new Error("A handler for '" + id + "' already exists.");
    }
    if (Array.isArray(dialogId)) {
        this.handlers[id] = SimpleDialog_1.createWaterfall(dialogId);
    }
    else if (typeof dialogId === 'string') {
        this.handlers[id] = DialogAction_1.DialogAction.beginDialog(dialogId, dialogArgs);
    }
    else {
        this.handlers[id] = SimpleDialog_1.createWaterfall([dialogId]);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.matchesAny"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>matchesAny (intents, dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.matchesAny)
- description and source-code
```javascript
matchesAny = function (intents, dialogId, dialogArgs) {
    for (var i = 0; i < intents.length; i++) {
        this.matches(intents[i], dialogId, dialogArgs);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.onBegin"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.IntentDialog.prototype.onBegin)
- description and source-code
```javascript
onBegin = function (handler) {
    this.beginDialog = handler;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.onDefault"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.IntentDialog.prototype.onDefault)
- description and source-code
```javascript
onDefault = function (dialogId, dialogArgs) {
    if (Array.isArray(dialogId)) {
        this.handlers[consts.Intents.Default] = SimpleDialog_1.createWaterfall(dialogId);
    }
    else if (typeof dialogId === 'string') {
        this.handlers[consts.Intents.Default] = DialogAction_1.DialogAction.beginDialog(dialogId, dialogArgs);
    }
    else {
        this.handlers[consts.Intents.Default] = SimpleDialog_1.createWaterfall([dialogId]);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.IntentDialog.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    this.recognizers.recognize(context, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.recognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.IntentDialog.prototype.recognizer)
- description and source-code
```javascript
recognizer = function (plugin) {
    this.recognizers.recognizer(plugin);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentDialog.prototype.replyReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.IntentDialog.prototype.replyReceived)
- description and source-code
```javascript
replyReceived = function (session, recognizeResult) {
    var _this = this;
    if (!recognizeResult) {
        var locale = session.preferredLocale();
        var context = session.toRecognizeContext();
        context.dialogData = session.dialogData;
        context.activeDialog = true;
        this.recognize(context, function (err, result) {
            if (!err) {
                _this.invokeIntent(session, result);
            }
            else {
                _this.emitError(session, err);
            }
        });
    }
    else {
        this.invokeIntent(session, recognizeResult);
    }
}
```
- example usage
```shell
...
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
...
```



# <a name="apidoc.module.botbuilder.IntentRecognizerSet"></a>[module botbuilder.IntentRecognizerSet](#apidoc.module.botbuilder.IntentRecognizerSet)

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.IntentRecognizerSet"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>IntentRecognizerSet (options)](#apidoc.element.botbuilder.IntentRecognizerSet.IntentRecognizerSet)
- description and source-code
```javascript
function IntentRecognizerSet(options) {
    if (options === void 0) { options = {}; }
    this.options = options;
    if (typeof this.options.intentThreshold !== 'number') {
        this.options.intentThreshold = 0.1;
    }
    if (!this.options.hasOwnProperty('recognizeOrder')) {
        this.options.recognizeOrder = RecognizeOrder.parallel;
    }
    if (!this.options.recognizers) {
        this.options.recognizers = [];
    }
    if (!this.options.processLimit) {
        this.options.processLimit = 4;
    }
    if (!this.options.hasOwnProperty('stopIfExactMatch')) {
        this.options.stopIfExactMatch = true;
    }
    this.length = this.options.recognizers.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.IntentRecognizerSet.prototype"></a>[module botbuilder.IntentRecognizerSet.prototype](#apidoc.module.botbuilder.IntentRecognizerSet.prototype)

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.prototype.clone"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>clone (copyTo)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.clone)
- description and source-code
```javascript
clone = function (copyTo) {
    var obj = copyTo || new IntentRecognizerSet(utils.clone(this.options));
    obj.options.recognizers = this.options.recognizers.slice(0);
    return obj;
}
```
- example usage
```shell
...
        else if (map.hasOwnProperty('*')) {
            this.data.sourceEvent = map['*'];
        }
    }
    return this;
};
Message.prototype.toMessage = function () {
    return utils.clone(this.data);
};
Message.prototype.upgradeAttachment = function (a) {
    var isOldSchema = false;
    for (var prop in a) {
        switch (prop) {
            case 'actions':
            case 'fallbackText':
...
```

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognize (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, done) {
    if (this.options.recognizeOrder == RecognizeOrder.parallel) {
        this.recognizeInParallel(context, done);
    }
    else {
        this.recognizeInSeries(context, done);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInParallel"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizeInParallel (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInParallel)
- description and source-code
```javascript
recognizeInParallel = function (context, done) {
    var _this = this;
    var result = { score: 0.0, intent: null };
    async.eachLimit(this.options.recognizers, this.options.processLimit, function (recognizer, cb) {
        try {
            recognizer.recognize(context, function (err, r) {
                if (!err && r && r.score > result.score && r.score >= _this.options.intentThreshold) {
                    result = r;
                }
                cb(err);
            });
        }
        catch (e) {
            cb(e);
        }
    }, function (err) {
        if (!err) {
            done(null, result);
        }
        else {
            var msg = err.toString();
            done(err instanceof Error ? err : new Error(msg), null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInSeries"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizeInSeries (context, done)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizeInSeries)
- description and source-code
```javascript
recognizeInSeries = function (context, done) {
    var _this = this;
    var i = 0;
    var result = { score: 0.0, intent: null };
    async.whilst(function () {
        return (i < _this.options.recognizers.length && (result.score < 1.0 || !_this.options.stopIfExactMatch));
    }, function (cb) {
        try {
            var recognizer = _this.options.recognizers[i++];
            recognizer.recognize(context, function (err, r) {
                if (!err && r && r.score > result.score && r.score >= _this.options.intentThreshold) {
                    result = r;
                }
                cb(err);
            });
        }
        catch (e) {
            cb(e);
        }
    }, function (err) {
        if (!err) {
            done(null, result);
        }
        else {
            done(err instanceof Error ? err : new Error(err.toString()), null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.IntentRecognizerSet.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.IntentRecognizerSet.prototype.recognizer)
- description and source-code
```javascript
recognizer = function (plugin) {
    this.options.recognizers.push(plugin);
    this.length++;
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Keyboard"></a>[module botbuilder.Keyboard](#apidoc.module.botbuilder.Keyboard)

#### <a name="apidoc.element.botbuilder.Keyboard.Keyboard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Keyboard (session)](#apidoc.element.botbuilder.Keyboard.Keyboard)
- description and source-code
```javascript
function Keyboard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.keyboard',
        content: {}
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Keyboard.prototype"></a>[module botbuilder.Keyboard.prototype](#apidoc.module.botbuilder.Keyboard.prototype)

#### <a name="apidoc.element.botbuilder.Keyboard.prototype.buttons"></a>[function <span class="apidocSignatureSpan">botbuilder.Keyboard.prototype.</span>buttons (list)](#apidoc.element.botbuilder.Keyboard.prototype.buttons)
- description and source-code
```javascript
buttons = function (list) {
    this.data.content.buttons = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var action = list[i];
            this.data.content.buttons.push(action.toAction ? action.toAction() : action);
        }
    }
    return this;
}
```
- example usage
```shell
...
                    CardAction_1.CardAction.imBack(null, old.message, old.title) :
                    CardAction_1.CardAction.openUrl(null, old.url, old.title);
                if (old.image) {
                    btn.image(old.image);
                }
                list.push(btn);
            }
            card.buttons(list);
        }
        return card.toAttachment();
    }
    else {
        return a;
    }
};
...
```

#### <a name="apidoc.element.botbuilder.Keyboard.prototype.toAttachment"></a>[function <span class="apidocSignatureSpan">botbuilder.Keyboard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.Keyboard.prototype.toAttachment)
- description and source-code
```javascript
toAttachment = function () {
    return this.data;
}
```
- example usage
```shell
...
            this.addAttachment(list[i]);
        }
    }
    return this;
};
Message.prototype.addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
        a = this.upgradeAttachment(a);
        if (!this.data.attachments) {
            this.data.attachments = [a];
        }
        else {
            this.data.attachments.push(a);
        }
...
```



# <a name="apidoc.module.botbuilder.Library"></a>[module botbuilder.Library](#apidoc.module.botbuilder.Library)

#### <a name="apidoc.element.botbuilder.Library.Library"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Library (name)](#apidoc.element.botbuilder.Library.Library)
- description and source-code
```javascript
function Library(name) {
    var _this = _super.call(this) || this;
    _this.name = name;
    _this.dialogs = {};
    _this.libraries = {};
    _this.actions = new ActionSet_1.ActionSet();
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet();
    _this.triggersAdded = false;
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.EventEmitter"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.</span>EventEmitter ()](#apidoc.element.botbuilder.Library.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.addRouteResult"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.</span>addRouteResult (route, current)](#apidoc.element.botbuilder.Library.addRouteResult)
- description and source-code
```javascript
addRouteResult = function (route, current) {
    if (!current || current.length < 1 || route.score > current[0].score) {
        current = [route];
    }
    else if (route.score == current[0].score) {
        current.push(route);
    }
    return current;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.bestRouteResult"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.</span>bestRouteResult (routes, dialogStack, rootLibraryName)](#apidoc.element.botbuilder.Library.bestRouteResult)
- description and source-code
```javascript
bestRouteResult = function (routes, dialogStack, rootLibraryName) {
    var bestLibrary = rootLibraryName;
    if (dialogStack) {
        dialogStack.forEach(function (entry) {
            var parts = entry.id.split(':');
            for (var i = 0; i < routes.length; i++) {
                if (routes[i].libraryName == parts[0]) {
                    bestLibrary = parts[0];
                    break;
                }
            }
        });
    }
    var best;
    var bestPriority = 5;
    for (var i = 0; i < routes.length; i++) {
        var r = routes[i];
        if (r.score > 0.0) {
            var priority;
            switch (r.routeType) {
                default:
                    priority = 1;
                    break;
                case Library.RouteTypes.ActiveDialog:
                    priority = 2;
                    break;
                case Library.RouteTypes.StackAction:
                    priority = 3;
                    break;
                case Library.RouteTypes.GlobalAction:
                    priority = 4;
                    break;
            }
            if (priority < bestPriority) {
                best = r;
                bestPriority = priority;
            }
            else if (priority == bestPriority) {
                switch (priority) {
                    case 3:
                        if (r.routeData.dialogIndex > best.routeData.dialogIndex) {
                            best = r;
                        }
                        break;
                    case 4:
                        if (bestLibrary && best.libraryName !== bestLibrary && r.libraryName == bestLibrary) {
                            best = r;
                        }
                        break;
                }
            }
        }
    }
    return best;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.init"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.</span>init ()](#apidoc.element.botbuilder.Library.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.listenerCount"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.Library.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Library.prototype"></a>[module botbuilder.Library.prototype](#apidoc.module.botbuilder.Library.prototype)

#### <a name="apidoc.element.botbuilder.Library.prototype.beginDialogAction"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>beginDialogAction (name, id, options)](#apidoc.element.botbuilder.Library.prototype.beginDialogAction)
- description and source-code
```javascript
beginDialogAction = function (name, id, options) {
    this.actions.beginDialogAction(name, id, options);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.clone"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>clone (copyTo, newName)](#apidoc.element.botbuilder.Library.prototype.clone)
- description and source-code
```javascript
clone = function (copyTo, newName) {
    var obj = copyTo || new Library(newName || this.name);
    for (var id in this.dialogs) {
        obj.dialogs[id] = this.dialogs[id];
    }
    for (var name in this.libraries) {
        obj.libraries[name] = this.libraries[name];
    }
    this.actions.clone(obj.actions);
    this.recognizers.clone(obj.recognizers);
    obj._localePath = this._localePath;
    obj._onFindRoutes = this._onFindRoutes;
    obj._onSelectRoute = this._onSelectRoute;
    obj.triggersAdded = this.triggersAdded;
    return obj;
}
```
- example usage
```shell
...
        else if (map.hasOwnProperty('*')) {
            this.data.sourceEvent = map['*'];
        }
    }
    return this;
};
Message.prototype.toMessage = function () {
    return utils.clone(this.data);
};
Message.prototype.upgradeAttachment = function (a) {
    var isOldSchema = false;
    for (var prop in a) {
        switch (prop) {
            case 'actions':
            case 'fallbackText':
...
```

#### <a name="apidoc.element.botbuilder.Library.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>constructor (name)](#apidoc.element.botbuilder.Library.prototype.constructor)
- description and source-code
```javascript
function Library(name) {
    var _this = _super.call(this) || this;
    _this.name = name;
    _this.dialogs = {};
    _this.libraries = {};
    _this.actions = new ActionSet_1.ActionSet();
    _this.recognizers = new IntentRecognizerSet_1.IntentRecognizerSet();
    _this.triggersAdded = false;
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.defaultFindRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>defaultFindRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.defaultFindRoutes)
- description and source-code
```javascript
defaultFindRoutes = function (context, callback) {
    var _this = this;
    var results = Library.addRouteResult({ score: 0.0, libraryName: this.name });
    this.recognize(context, function (err, topIntent) {
        if (!err) {
            var ctx = utils.clone(context);
            ctx.intent = topIntent && topIntent.score > 0 ? topIntent : null;
            ctx.libraryName = _this.name;
            async.parallel([
                function (cb) {
                    _this.findActiveDialogRoutes(ctx, function (err, routes) {
                        if (!err && routes) {
                            routes.forEach(function (r) { return results = Library.addRouteResult(r, results); });
                        }
                        cb(err);
                    });
                },
                function (cb) {
                    _this.findStackActionRoutes(ctx, function (err, routes) {
                        if (!err && routes) {
                            routes.forEach(function (r) { return results = Library.addRouteResult(r, results); });
                        }
                        cb(err);
                    });
                },
                function (cb) {
                    _this.findGlobalActionRoutes(ctx, function (err, routes) {
                        if (!err && routes) {
                            routes.forEach(function (r) { return results = Library.addRouteResult(r, results); });
                        }
                        cb(err);
                    });
                }
            ], function (err) {
                if (!err) {
                    callback(null, results);
                }
                else {
                    callback(err, null);
                }
            });
        }
        else {
            callback(err, null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.defaultSelectRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>defaultSelectRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.defaultSelectRoute)
- description and source-code
```javascript
defaultSelectRoute = function (session, route) {
    switch (route.routeType || '') {
        case Library.RouteTypes.ActiveDialog:
            this.selectActiveDialogRoute(session, route);
            break;
        case Library.RouteTypes.StackAction:
            this.selectStackActionRoute(session, route);
            break;
        case Library.RouteTypes.GlobalAction:
            this.selectGlobalActionRoute(session, route);
            break;
        default:
            throw new Error('Invalid route type passed to Library.selectRoute().');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.dialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>dialog (id, dialog)](#apidoc.element.botbuilder.Library.prototype.dialog)
- description and source-code
```javascript
dialog = function (id, dialog) {
    var d;
    if (dialog) {
        if (id.indexOf(':') >= 0) {
            id = id.split(':')[1];
        }
        if (this.dialogs.hasOwnProperty(id)) {
            throw new Error("Dialog[" + id + "] already exists in library[" + this.name + "].");
        }
        if (Array.isArray(dialog)) {
            d = new SimpleDialog_1.SimpleDialog(SimpleDialog_1.createWaterfall(dialog));
        }
        else if (typeof dialog == 'function') {
            d = new SimpleDialog_1.SimpleDialog(SimpleDialog_1.createWaterfall([dialog]));
        }
        else {
            d = dialog;
        }
        this.dialogs[id] = d;
    }
    else if (this.dialogs.hasOwnProperty(id)) {
        d = this.dialogs[id];
    }
    return d;
}
```
- example usage
```shell
...

// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
...
```

#### <a name="apidoc.element.botbuilder.Library.prototype.endConversationAction"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>endConversationAction (name, msg, options)](#apidoc.element.botbuilder.Library.prototype.endConversationAction)
- description and source-code
```javascript
endConversationAction = function (name, msg, options) {
    this.actions.endConversationAction(name, msg, options);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.findActiveDialogRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findActiveDialogRoutes (context, callback, dialogStack)](#apidoc.element.botbuilder.Library.prototype.findActiveDialogRoutes)
- description and source-code
```javascript
findActiveDialogRoutes = function (context, callback, dialogStack) {
    var _this = this;
    if (!dialogStack) {
        dialogStack = context.dialogStack();
    }
    var results = Library.addRouteResult({ score: 0.0, libraryName: this.name });
    var entry = Session_1.Session.activeDialogStackEntry(dialogStack);
    var parts = entry ? entry.id.split(':') : null;
    if (parts && parts[0] == this.name) {
        var dialog = this.dialog(parts[1]);
        if (dialog) {
            var ctx = utils.clone(context);
            ctx.libraryName = this.name;
            ctx.dialogData = entry.state;
            ctx.activeDialog = true;
            dialog.recognize(ctx, function (err, result) {
                if (!err) {
                    if (result.score < 0.1) {
                        result.score = 0.1;
                    }
                    callback(null, Library.addRouteResult({
                        score: result.score,
                        libraryName: _this.name,
                        routeType: Library.RouteTypes.ActiveDialog,
                        routeData: result
                    }, results));
                }
                else {
                    callback(err, null);
                }
            });
        }
        else {
            logger.warn(ctx, "Active dialog '%s' not found in library.", entry.id);
            callback(null, results);
        }
    }
    else {
        callback(null, results);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.findDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findDialog (libName, dialogId)](#apidoc.element.botbuilder.Library.prototype.findDialog)
- description and source-code
```javascript
findDialog = function (libName, dialogId) {
    var d;
    var lib = this.library(libName);
    if (lib) {
        d = lib.dialog(dialogId);
    }
    return d;
}
```
- example usage
```shell
...
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
...
```

#### <a name="apidoc.element.botbuilder.Library.prototype.findGlobalActionRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findGlobalActionRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.findGlobalActionRoutes)
- description and source-code
```javascript
findGlobalActionRoutes = function (context, callback) {
    var results = Library.addRouteResult({ score: 0.0, libraryName: this.name });
    var ctx = utils.clone(context);
    ctx.libraryName = this.name;
    ctx.routeType = Library.RouteTypes.GlobalAction;
    this.actions.findActionRoutes(ctx, function (err, ra) {
        if (!err) {
            for (var i = 0; i < ra.length; i++) {
                var r = ra[i];
                results = Library.addRouteResult(r, results);
            }
            callback(null, results);
        }
        else {
            callback(err, null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.findRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findRoutes (context, callback)](#apidoc.element.botbuilder.Library.prototype.findRoutes)
- description and source-code
```javascript
findRoutes = function (context, callback) {
    var _this = this;
    if (!this.triggersAdded) {
        this.forEachDialog(function (dialog, id) { return dialog.addDialogTrigger(_this.actions, _this.name + ':' + id); });
        this.triggersAdded = true;
    }
    if (this._onFindRoutes) {
        this._onFindRoutes(context, callback);
    }
    else {
        this.defaultFindRoutes(context, callback);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.findStackActionRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>findStackActionRoutes (context, callback, dialogStack)](#apidoc.element.botbuilder.Library.prototype.findStackActionRoutes)
- description and source-code
```javascript
findStackActionRoutes = function (context, callback, dialogStack) {
    var _this = this;
    if (!dialogStack) {
        dialogStack = context.dialogStack();
    }
    var results = Library.addRouteResult({ score: 0.0, libraryName: this.name });
    var ctx = utils.clone(context);
    ctx.libraryName = this.name;
    ctx.routeType = Library.RouteTypes.StackAction;
    async.forEachOf(dialogStack || [], function (entry, index, next) {
        var parts = entry.id.split(':');
        if (parts[0] == _this.name) {
            var dialog = _this.dialog(parts[1]);
            if (dialog) {
                dialog.findActionRoutes(ctx, function (err, ra) {
                    if (!err) {
                        for (var i = 0; i < ra.length; i++) {
                            var r = ra[i];
                            if (r.routeData) {
                                r.routeData.dialogId = entry.id;
                                r.routeData.dialogIndex = index;
                            }
                            results = Library.addRouteResult(r, results);
                        }
                    }
                    next(err);
                });
            }
            else {
                logger.warn(ctx, "Dialog '%s' not found in library.", entry.id);
                next(null);
            }
        }
        else {
            next(null);
        }
    }, function (err) {
        if (!err) {
            callback(null, results);
        }
        else {
            callback(err, null);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.forEachDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>forEachDialog (callback)](#apidoc.element.botbuilder.Library.prototype.forEachDialog)
- description and source-code
```javascript
forEachDialog = function (callback) {
    for (var id in this.dialogs) {
        callback(this.dialog(id), id);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.forEachLibrary"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>forEachLibrary (callback)](#apidoc.element.botbuilder.Library.prototype.forEachLibrary)
- description and source-code
```javascript
forEachLibrary = function (callback) {
    for (var lib in this.libraries) {
        callback(this.libraries[lib]);
    }
}
```
- example usage
```shell
...
this.locales = {};
this.defaultLocale(defaultLocale || 'en');
var libsSeen = {};
var _that = this;
function addPaths(library) {
    if (!libsSeen.hasOwnProperty(library.name)) {
        libsSeen[library.name] = true;
        library.forEachLibrary(function (child) {
            addPaths(child);
        });
        var path = library.localePath();
        if (path) {
            _that.localePaths.push(path);
        }
    }
...
```

#### <a name="apidoc.element.botbuilder.Library.prototype.library"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>library (lib)](#apidoc.element.botbuilder.Library.prototype.library)
- description and source-code
```javascript
library = function (lib) {
    var l;
    if (typeof lib === 'string') {
        if (lib == this.name) {
            l = this;
        }
        else if (this.libraries.hasOwnProperty(lib)) {
            l = this.libraries[lib];
        }
        else {
            for (var name in this.libraries) {
                l = this.libraries[name].library(lib);
                if (l) {
                    break;
                }
            }
        }
    }
    else {
        l = this.libraries[lib.name] = lib;
    }
    return l;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.libraryList"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>libraryList (reverse)](#apidoc.element.botbuilder.Library.prototype.libraryList)
- description and source-code
```javascript
libraryList = function (reverse) {
    if (reverse === void 0) { reverse = false; }
    var list = [];
    var added = {};
    function addChildren(lib) {
        if (!added.hasOwnProperty(lib.name)) {
            added[lib.name] = true;
            if (!reverse) {
                list.push(lib);
            }
            lib.forEachLibrary(function (child) { return addChildren(child); });
            if (reverse) {
                list.push(lib);
            }
        }
    }
    addChildren(this);
    return list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.localePath"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>localePath (path)](#apidoc.element.botbuilder.Library.prototype.localePath)
- description and source-code
```javascript
localePath = function (path) {
    if (path) {
        this._localePath = path;
    }
    return this._localePath;
}
```
- example usage
```shell
...
    var _that = this;
    function addPaths(library) {
        if (!libsSeen.hasOwnProperty(library.name)) {
            libsSeen[library.name] = true;
            library.forEachLibrary(function (child) {
                addPaths(child);
            });
            var path = library.localePath();
            if (path) {
                _that.localePaths.push(path);
            }
        }
    }
    addPaths(root);
}
...
```

#### <a name="apidoc.element.botbuilder.Library.prototype.onFindRoutes"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>onFindRoutes (handler)](#apidoc.element.botbuilder.Library.prototype.onFindRoutes)
- description and source-code
```javascript
onFindRoutes = function (handler) {
    this._onFindRoutes = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.onSelectRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>onSelectRoute (handler)](#apidoc.element.botbuilder.Library.prototype.onSelectRoute)
- description and source-code
```javascript
onSelectRoute = function (handler) {
    this._onSelectRoute = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>recognize (context, callback)](#apidoc.element.botbuilder.Library.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, callback) {
    if (this.recognizers.length > 0 && context.libraryName !== this.name) {
        this.recognizers.recognize(context, callback);
    }
    else {
        callback(null, context.intent || { intent: 'None', score: 0.0 });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.recognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>recognizer (plugin)](#apidoc.element.botbuilder.Library.prototype.recognizer)
- description and source-code
```javascript
recognizer = function (plugin) {
    this.recognizers.recognizer(plugin);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.selectActiveDialogRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectActiveDialogRoute (session, route, newStack)](#apidoc.element.botbuilder.Library.prototype.selectActiveDialogRoute)
- description and source-code
```javascript
selectActiveDialogRoute = function (session, route, newStack) {
    if (!route || route.libraryName !== this.name || route.routeType !== Library.RouteTypes.ActiveDialog) {
        throw new Error('Invalid route type passed to Library.selectActiveDialogRoute().');
    }
    if (newStack) {
        session.dialogStack(newStack);
    }
    session.routeToActiveDialog(route.routeData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.selectGlobalActionRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectGlobalActionRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.selectGlobalActionRoute)
- description and source-code
```javascript
selectGlobalActionRoute = function (session, route) {
    if (!route || route.libraryName !== this.name || route.routeType !== Library.RouteTypes.GlobalAction) {
        throw new Error('Invalid route type passed to Library.selectGlobalActionRoute().');
    }
    this.actions.selectActionRoute(session, route);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.selectRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectRoute (session, route)](#apidoc.element.botbuilder.Library.prototype.selectRoute)
- description and source-code
```javascript
selectRoute = function (session, route) {
    if (this._onSelectRoute) {
        this._onSelectRoute(session, route);
    }
    else {
        this.defaultSelectRoute(session, route);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Library.prototype.selectStackActionRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.Library.prototype.</span>selectStackActionRoute (session, route, newStack)](#apidoc.element.botbuilder.Library.prototype.selectStackActionRoute)
- description and source-code
```javascript
selectStackActionRoute = function (session, route, newStack) {
    if (!route || route.libraryName !== this.name || route.routeType !== Library.RouteTypes.StackAction) {
        throw new Error('Invalid route type passed to Library.selectStackActionRoute().');
    }
    if (newStack) {
        session.dialogStack(newStack);
    }
    var routeData = route.routeData;
    var parts = routeData.dialogId.split(':');
    this.dialog(parts[1]).selectActionRoute(session, route);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.LuisDialog"></a>[module botbuilder.LuisDialog](#apidoc.module.botbuilder.LuisDialog)

#### <a name="apidoc.element.botbuilder.LuisDialog.LuisDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>LuisDialog (serviceUri)](#apidoc.element.botbuilder.LuisDialog.LuisDialog)
- description and source-code
```javascript
function LuisDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('LuisDialog class is deprecated. Use IntentDialog with a LuisRecognizer instead.');
    var recognizer = new LuisRecognizer_1.LuisRecognizer(serviceUri);
    _this.dialog = new IntentDialog_1.IntentDialog({ recognizers: [recognizer] });
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.LuisDialog.prototype"></a>[module botbuilder.LuisDialog.prototype](#apidoc.module.botbuilder.LuisDialog.prototype)

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.LuisDialog.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    this.dialog.begin(session, args);
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>constructor (serviceUri)](#apidoc.element.botbuilder.LuisDialog.prototype.constructor)
- description and source-code
```javascript
function LuisDialog(serviceUri) {
    var _this = _super.call(this) || this;
    console.warn('LuisDialog class is deprecated. Use IntentDialog with a LuisRecognizer instead.');
    var recognizer = new LuisRecognizer_1.LuisRecognizer(serviceUri);
    _this.dialog = new IntentDialog_1.IntentDialog({ recognizers: [recognizer] });
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.LuisDialog.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    this.dialog.dialogResumed(session, result);
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.on"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>on (intent, dialogId, dialogArgs)](#apidoc.element.botbuilder.LuisDialog.prototype.on)
- description and source-code
```javascript
on = function (intent, dialogId, dialogArgs) {
    this.dialog.matches(intent, dialogId, dialogArgs);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.onBegin"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>onBegin (handler)](#apidoc.element.botbuilder.LuisDialog.prototype.onBegin)
- description and source-code
```javascript
onBegin = function (handler) {
    this.dialog.onBegin(handler);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.onDefault"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>onDefault (dialogId, dialogArgs)](#apidoc.element.botbuilder.LuisDialog.prototype.onDefault)
- description and source-code
```javascript
onDefault = function (dialogId, dialogArgs) {
    this.dialog.onDefault(dialogId, dialogArgs);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.LuisDialog.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    this.dialog.recognize(context, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisDialog.prototype.replyReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisDialog.prototype.</span>replyReceived (session, recognizeResult)](#apidoc.element.botbuilder.LuisDialog.prototype.replyReceived)
- description and source-code
```javascript
replyReceived = function (session, recognizeResult) {
}
```
- example usage
```shell
...
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
...
```



# <a name="apidoc.module.botbuilder.LuisRecognizer"></a>[module botbuilder.LuisRecognizer](#apidoc.module.botbuilder.LuisRecognizer)

#### <a name="apidoc.element.botbuilder.LuisRecognizer.LuisRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>LuisRecognizer (models)](#apidoc.element.botbuilder.LuisRecognizer.LuisRecognizer)
- description and source-code
```javascript
function LuisRecognizer(models) {
    if (typeof models == 'string') {
        this.models = { '*': models };
    }
    else {
        this.models = (models || {});
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.LuisRecognizer.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisRecognizer.</span>recognize (utterance, modelUrl, callback)](#apidoc.element.botbuilder.LuisRecognizer.recognize)
- description and source-code
```javascript
recognize = function (utterance, modelUrl, callback) {
    try {
        var uri = modelUrl.trim();
        if (uri.lastIndexOf('&q=') != uri.length - 3) {
            uri += '&q=';
        }
        uri += encodeURIComponent(utterance || '');
        request.get(uri, function (err, res, body) {
            var result;
            try {
                if (!err) {
                    result = JSON.parse(body);
                    result.intents = result.intents || [];
                    result.entities = result.entities || [];
                    if (result.topScoringIntent && result.intents.length == 0) {
                        result.intents.push(result.topScoringIntent);
                    }
                    if (result.intents.length == 1 && typeof result.intents[0].score !== 'number') {
                        result.intents[0].score = 1.0;
                    }
                }
            }
            catch (e) {
                err = e;
            }
            try {
                if (!err) {
                    callback(null, result.intents, result.entities);
                }
                else {
                    var m = err.toString();
                    callback(err instanceof Error ? err : new Error(m));
                }
            }
            catch (e) {
                console.error(e.toString());
            }
        });
    }
    catch (err) {
        callback(err instanceof Error ? err : new Error(err.toString()));
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.LuisRecognizer.prototype"></a>[module botbuilder.LuisRecognizer.prototype](#apidoc.module.botbuilder.LuisRecognizer.prototype)

#### <a name="apidoc.element.botbuilder.LuisRecognizer.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.LuisRecognizer.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.LuisRecognizer.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    var result = { score: 0.0, intent: null };
    if (context && context.message && context.message.text) {
        var utterance = context.message.text;
        var locale = context.locale || '*';
        var model = this.models.hasOwnProperty(locale) ? this.models[locale] : this.models['*'];
        if (model) {
            LuisRecognizer.recognize(utterance, model, function (err, intents, entities) {
                if (!err) {
                    result.intents = intents;
                    result.entities = entities;
                    var top;
                    intents.forEach(function (intent) {
                        if (top) {
                            if (intent.score > top.score) {
                                top = intent;
                            }
                        }
                        else {
                            top = intent;
                        }
                    });
                    if (top) {
                        result.score = top.score;
                        result.intent = top.intent;
                        switch (top.intent.toLowerCase()) {
                            case 'builtin.intent.none':
                            case 'none':
                                result.score = 0.1;
                                break;
                        }
                    }
                    cb(null, result);
                }
                else {
                    cb(err, null);
                }
            });
        }
        else {
            cb(new Error("LUIS model not found for locale '" + locale + "'."), null);
        }
    }
    else {
        cb(null, result);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.MediaCard"></a>[module botbuilder.MediaCard](#apidoc.module.botbuilder.MediaCard)

#### <a name="apidoc.element.botbuilder.MediaCard.MediaCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>MediaCard (session)](#apidoc.element.botbuilder.MediaCard.MediaCard)
- description and source-code
```javascript
function MediaCard(session) {
    return _super.call(this, session) || this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.MediaCard.prototype"></a>[module botbuilder.MediaCard.prototype](#apidoc.module.botbuilder.MediaCard.prototype)

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.autoloop"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>autoloop (choice)](#apidoc.element.botbuilder.MediaCard.prototype.autoloop)
- description and source-code
```javascript
autoloop = function (choice) {
    this.data.content.autoloop = choice;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.autostart"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>autostart (choice)](#apidoc.element.botbuilder.MediaCard.prototype.autostart)
- description and source-code
```javascript
autostart = function (choice) {
    this.data.content.autostart = choice;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.MediaCard.prototype.constructor)
- description and source-code
```javascript
function MediaCard(session) {
    return _super.call(this, session) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.image"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>image (image)](#apidoc.element.botbuilder.MediaCard.prototype.image)
- description and source-code
```javascript
image = function (image) {
    if (image) {
        this.data.content.image = image.toImage ? image.toImage() : image;
    }
    return this;
}
```
- example usage
```shell
...
        var list = [];
        for (var i = 0; i < v2.actions.length; i++) {
            var old = v2.actions[i];
            var btn = old.message ?
                CardAction_1.CardAction.imBack(null, old.message, old.title) :
                CardAction_1.CardAction.openUrl(null, old.url, old.title);
            if (old.image) {
                btn.image(old.image);
            }
            list.push(btn);
        }
        card.buttons(list);
    }
    return card.toAttachment();
}
...
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.media"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>media (list)](#apidoc.element.botbuilder.MediaCard.prototype.media)
- description and source-code
```javascript
media = function (list) {
    this.data.content.media = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var media = list[i];
            this.data.content.media.push(media.toMedia ? media.toMedia() : media);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.shareable"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>shareable (choice)](#apidoc.element.botbuilder.MediaCard.prototype.shareable)
- description and source-code
```javascript
shareable = function (choice) {
    this.data.content.shareable = choice;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.subtitle"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.MediaCard.prototype.subtitle)
- description and source-code
```javascript
subtitle = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.subtitle = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.text"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>text (text)](#apidoc.element.botbuilder.MediaCard.prototype.text)
- description and source-code
```javascript
text = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.text = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.MediaCard.prototype.title"></a>[function <span class="apidocSignatureSpan">botbuilder.MediaCard.prototype.</span>title (text)](#apidoc.element.botbuilder.MediaCard.prototype.title)
- description and source-code
```javascript
title = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.title = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
        card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
    }
...
```



# <a name="apidoc.module.botbuilder.MemoryBotStorage"></a>[module botbuilder.MemoryBotStorage](#apidoc.module.botbuilder.MemoryBotStorage)

#### <a name="apidoc.element.botbuilder.MemoryBotStorage.MemoryBotStorage"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>MemoryBotStorage ()](#apidoc.element.botbuilder.MemoryBotStorage.MemoryBotStorage)
- description and source-code
```javascript
function MemoryBotStorage() {
    this.userStore = {};
    this.conversationStore = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.MemoryBotStorage.prototype"></a>[module botbuilder.MemoryBotStorage.prototype](#apidoc.module.botbuilder.MemoryBotStorage.prototype)

#### <a name="apidoc.element.botbuilder.MemoryBotStorage.prototype.deleteData"></a>[function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>deleteData (context)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.deleteData)
- description and source-code
```javascript
deleteData = function (context) {
    if (context.userId && this.userStore.hasOwnProperty(context.userId)) {
        if (context.conversationId) {
            if (this.conversationStore.hasOwnProperty(context.conversationId)) {
                delete this.conversationStore[context.conversationId];
            }
        }
        else {
            delete this.userStore[context.userId];
            for (var key in this.conversationStore) {
                if (key.indexOf(context.userId + ':') == 0) {
                    delete this.conversationStore[key];
                }
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MemoryBotStorage.prototype.getData"></a>[function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>getData (context, callback)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.getData)
- description and source-code
```javascript
getData = function (context, callback) {
    var data = {};
    if (context.userId) {
        if (context.persistUserData) {
            if (this.userStore.hasOwnProperty(context.userId)) {
                data.userData = JSON.parse(this.userStore[context.userId]);
            }
            else {
                data.userData = null;
            }
        }
        if (context.conversationId) {
            var key = context.userId + ':' + context.conversationId;
            if (this.conversationStore.hasOwnProperty(key)) {
                data.privateConversationData = JSON.parse(this.conversationStore[key]);
            }
            else {
                data.privateConversationData = null;
            }
        }
    }
    if (context.persistConversationData && context.conversationId) {
        if (this.conversationStore.hasOwnProperty(context.conversationId)) {
            data.conversationData = JSON.parse(this.conversationStore[context.conversationId]);
        }
        else {
            data.conversationData = null;
        }
    }
    callback(null, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.MemoryBotStorage.prototype.saveData"></a>[function <span class="apidocSignatureSpan">botbuilder.MemoryBotStorage.prototype.</span>saveData (context, data, callback)](#apidoc.element.botbuilder.MemoryBotStorage.prototype.saveData)
- description and source-code
```javascript
saveData = function (context, data, callback) {
    if (context.userId) {
        if (context.persistUserData) {
            this.userStore[context.userId] = JSON.stringify(data.userData || {});
        }
        if (context.conversationId) {
            var key = context.userId + ':' + context.conversationId;
            this.conversationStore[key] = JSON.stringify(data.privateConversationData || {});
        }
    }
    if (context.persistConversationData && context.conversationId) {
        this.conversationStore[context.conversationId] = JSON.stringify(data.conversationData || {});
    }
    callback(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Message"></a>[module botbuilder.Message](#apidoc.module.botbuilder.Message)

#### <a name="apidoc.element.botbuilder.Message.Message"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Message (session)](#apidoc.element.botbuilder.Message.Message)
- description and source-code
```javascript
function Message(session) {
    this.session = session;
    this.data = {};
    this.data.type = consts.messageType;
    this.data.agent = consts.agent;
    if (this.session) {
        var m = this.session.message;
        if (m.source) {
            this.data.source = m.source;
        }
        if (m.textLocale) {
            this.data.textLocale = m.textLocale;
        }
        if (m.address) {
            this.data.address = m.address;
        }
    }
}
```
- example usage
```shell
...
        }
        this.batchTimer = setTimeout(function () {
            _this.sendBatch();
        }, this.options.autoBatchDelay);
    }
};
Session.prototype.createMessage = function (localizationNamespace, text, args) {
    var message = new Message_1.Message(this)
        .text(this.vgettext(localizationNamespace, Message_1.Message.randomPrompt(text), args));
    return message.toMessage();
};
Session.prototype.prepareMessage = function (msg) {
    if (!msg.type) {
        msg.type = 'message';
    }
...
```

#### <a name="apidoc.element.botbuilder.Message.composePrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.</span>composePrompt (session, prompts, args)](#apidoc.element.botbuilder.Message.composePrompt)
- description and source-code
```javascript
composePrompt = function (session, prompts, args) {
    var connector = '';
    var prompt = '';
    for (var i = 0; i < prompts.length; i++) {
        var txt = Message.randomPrompt(prompts[i]);
        prompt += connector + (session ? session.gettext(txt) : txt);
        connector = ' ';
    }
    return args && args.length > 0 ? sprintf.vsprintf(prompt, args) : prompt;
}
```
- example usage
```shell
...
};
Message.prototype.compose = function (prompts) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (prompts) {
        this.data.text = Message.composePrompt(this.session, prompts, args);
    }
    return this;
};
Message.prototype.summary = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
...
```

#### <a name="apidoc.element.botbuilder.Message.randomPrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.</span>randomPrompt (prompts)](#apidoc.element.botbuilder.Message.randomPrompt)
- description and source-code
```javascript
randomPrompt = function (prompts) {
    if (Array.isArray(prompts)) {
        var i = Math.floor(Math.random() * prompts.length);
        return prompts[i];
    }
    else {
        return prompts;
    }
}
```
- example usage
```shell
...
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    this.data.text = text ? fmtText(this.session, text, args) : '';
    return this;
};
Message.prototype.ntext = function (msg, msg_plural, count) {
    var fmt = count == 1 ? Message.randomPrompt(msg) : Message.randomPrompt(msg_plural);
    if (this.session) {
        fmt = this.session.gettext(fmt);
    }
    this.data.text = sprintf.sprintf(fmt, count);
    return this;
};
Message.prototype.compose = function (prompts) {
...
```



# <a name="apidoc.module.botbuilder.Message.prototype"></a>[module botbuilder.Message.prototype](#apidoc.module.botbuilder.Message.prototype)

#### <a name="apidoc.element.botbuilder.Message.prototype.addAttachment"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>addAttachment (attachment)](#apidoc.element.botbuilder.Message.prototype.addAttachment)
- description and source-code
```javascript
addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
        a = this.upgradeAttachment(a);
        if (!this.data.attachments) {
            this.data.attachments = [a];
        }
        else {
            this.data.attachments.push(a);
        }
    }
    return this;
}
```
- example usage
```shell
...
    this.data.attachmentLayout = style;
    return this;
};
Message.prototype.attachments = function (list) {
    this.data.attachments = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            this.addAttachment(list[i]);
        }
    }
    return this;
};
Message.prototype.addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.addEntity"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>addEntity (obj)](#apidoc.element.botbuilder.Message.prototype.addEntity)
- description and source-code
```javascript
addEntity = function (obj) {
    if (obj) {
        if (!this.data.entities) {
            this.data.entities = [obj];
        }
        else {
            this.data.entities.push(obj);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.address"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>address (adr)](#apidoc.element.botbuilder.Message.prototype.address)
- description and source-code
```javascript
address = function (adr) {
    if (adr) {
        this.data.address = adr;
        this.data.source = adr.channelId;
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.attachmentLayout"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>attachmentLayout (style)](#apidoc.element.botbuilder.Message.prototype.attachmentLayout)
- description and source-code
```javascript
attachmentLayout = function (style) {
    this.data.attachmentLayout = style;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.attachments"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>attachments (list)](#apidoc.element.botbuilder.Message.prototype.attachments)
- description and source-code
```javascript
attachments = function (list) {
    this.data.attachments = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            this.addAttachment(list[i]);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.compose"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>compose (prompts)](#apidoc.element.botbuilder.Message.prototype.compose)
- description and source-code
```javascript
compose = function (prompts) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (prompts) {
        this.data.text = Message.composePrompt(this.session, prompts, args);
    }
    return this;
}
```
- example usage
```shell
...
    return this.ntext(msg, msg_plural, count);
};
Message.prototype.composePrompt = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    console.warn("Message.composePrompt() is deprecated. Use Message.compose() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.compose.apply(this, args);
};
Message.prototype.setChannelData = function (data) {
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.composePrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>composePrompt (session, prompts)](#apidoc.element.botbuilder.Message.prototype.composePrompt)
- description and source-code
```javascript
composePrompt = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    console.warn("Message.composePrompt() is deprecated. Use Message.compose() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.compose.apply(this, args);
}
```
- example usage
```shell
...
};
Message.prototype.compose = function (prompts) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (prompts) {
        this.data.text = Message.composePrompt(this.session, prompts, args);
    }
    return this;
};
Message.prototype.summary = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.entities"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>entities (list)](#apidoc.element.botbuilder.Message.prototype.entities)
- description and source-code
```javascript
entities = function (list) {
    this.data.entities = list || [];
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.ntext"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>ntext (msg, msg_plural, count)](#apidoc.element.botbuilder.Message.prototype.ntext)
- description and source-code
```javascript
ntext = function (msg, msg_plural, count) {
    var fmt = count == 1 ? Message.randomPrompt(msg) : Message.randomPrompt(msg_plural);
    if (this.session) {
        fmt = this.session.gettext(fmt);
    }
    this.data.text = sprintf.sprintf(fmt, count);
    return this;
}
```
- example usage
```shell
...
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.text.apply(this, args);
};
Message.prototype.setNText = function (session, msg, msg_plural, count) {
    console.warn("Message.setNText() is deprecated. Use Message.ntext() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    return this.ntext(msg, msg_plural, count);
};
Message.prototype.composePrompt = function (session, prompts) {
    var args = [];
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.setChannelData"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setChannelData (data)](#apidoc.element.botbuilder.Message.prototype.setChannelData)
- description and source-code
```javascript
setChannelData = function (data) {
    console.warn("Message.setChannelData() is deprecated. Use Message.sourceEvent() instead.");
    return this.sourceEvent({ '*': data });
}
```
- example usage
```shell
...
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.compose.apply(this, args);
};
Message.prototype.setChannelData = function (data) {
    console.warn("Message.setChannelData() is deprecated. Use Message.sourceEvent() instead.");
    return this.sourceEvent({ '*': data });
};
return Message;
}());
exports.Message = Message;
function fmtText(session, prompts, args) {
var fmt = Message.randomPrompt(prompts);
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.setLanguage"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setLanguage (local)](#apidoc.element.botbuilder.Message.prototype.setLanguage)
- description and source-code
```javascript
setLanguage = function (local) {
    console.warn("Message.setLanguage() is deprecated. Use Message.textLocal() instead.");
    return this.textLocale(local);
}
```
- example usage
```shell
...
        var txt = Message.randomPrompt(prompts[i]);
        prompt += connector + (session ? session.gettext(txt) : txt);
        connector = ' ';
    }
    return args && args.length > 0 ? sprintf.vsprintf(prompt, args) : prompt;
};
Message.prototype.setLanguage = function (local) {
    console.warn("Message.setLanguage() is deprecated. Use Message.textLocal() instead.");
    return this.textLocale(local);
};
Message.prototype.setText = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.setNText"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setNText (session, msg, msg_plural, count)](#apidoc.element.botbuilder.Message.prototype.setNText)
- description and source-code
```javascript
setNText = function (session, msg, msg_plural, count) {
    console.warn("Message.setNText() is deprecated. Use Message.ntext() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    return this.ntext(msg, msg_plural, count);
}
```
- example usage
```shell
...
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.text.apply(this, args);
};
Message.prototype.setNText = function (session, msg, msg_plural, count) {
    console.warn("Message.setNText() is deprecated. Use Message.ntext() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    return this.ntext(msg, msg_plural, count);
};
Message.prototype.composePrompt = function (session, prompts) {
    var args = [];
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.setText"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>setText (session, prompts)](#apidoc.element.botbuilder.Message.prototype.setText)
- description and source-code
```javascript
setText = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    console.warn("Message.setText() is deprecated. Use Message.text() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.text.apply(this, args);
}
```
- example usage
```shell
...
    return this.textLocale(local);
};
Message.prototype.setText = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    console.warn("Message.setText() is deprecated. Use Message.text() instead.");
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.text.apply(this, args);
};
Message.prototype.setNText = function (session, msg, msg_plural, count) {
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.sourceEvent"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>sourceEvent (map)](#apidoc.element.botbuilder.Message.prototype.sourceEvent)
- description and source-code
```javascript
sourceEvent = function (map) {
    if (map) {
        var channelId = this.data.address ? this.data.address.channelId : '*';
        if (map.hasOwnProperty(channelId)) {
            this.data.sourceEvent = map[channelId];
        }
        else if (map.hasOwnProperty('*')) {
            this.data.sourceEvent = map['*'];
        }
    }
    return this;
}
```
- example usage
```shell
...
    if (session && !this.session) {
        this.session = session;
    }
    args.unshift(prompts);
    return Message.prototype.compose.apply(this, args);
};
Message.prototype.setChannelData = function (data) {
    console.warn("Message.setChannelData() is deprecated. Use Message.sourceEvent() instead.");
    return this.sourceEvent({ '*': data });
};
return Message;
}());
exports.Message = Message;
function fmtText(session, prompts, args) {
var fmt = Message.randomPrompt(prompts);
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.summary"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>summary (text)](#apidoc.element.botbuilder.Message.prototype.summary)
- description and source-code
```javascript
summary = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    this.data.summary = text ? fmtText(this.session, text, args) : '';
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.text"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>text (text)](#apidoc.element.botbuilder.Message.prototype.text)
- description and source-code
```javascript
text = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    this.data.text = text ? fmtText(this.session, text, args) : '';
    return this;
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.textFormat"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>textFormat (style)](#apidoc.element.botbuilder.Message.prototype.textFormat)
- description and source-code
```javascript
textFormat = function (style) {
    this.data.textFormat = style;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.textLocale"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>textLocale (locale)](#apidoc.element.botbuilder.Message.prototype.textLocale)
- description and source-code
```javascript
textLocale = function (locale) {
    this.data.textLocale = locale;
    return this;
}
```
- example usage
```shell
...
        prompt += connector + (session ? session.gettext(txt) : txt);
        connector = ' ';
    }
    return args && args.length > 0 ? sprintf.vsprintf(prompt, args) : prompt;
};
Message.prototype.setLanguage = function (local) {
    console.warn("Message.setLanguage() is deprecated. Use Message.textLocal() instead.");
    return this.textLocale(local);
};
Message.prototype.setText = function (session, prompts) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    console.warn("Message.setText() is deprecated. Use Message.text() instead.");
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.timestamp"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>timestamp (time)](#apidoc.element.botbuilder.Message.prototype.timestamp)
- description and source-code
```javascript
timestamp = function (time) {
    this.data.timestamp = time || new Date().toISOString();
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Message.prototype.toMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>toMessage ()](#apidoc.element.botbuilder.Message.prototype.toMessage)
- description and source-code
```javascript
toMessage = function () {
    return utils.clone(this.data);
}
```
- example usage
```shell
...
this.msgSent = true;
if (message) {
    var m;
    if (typeof message == 'string' || Array.isArray(message)) {
        m = this.createMessage(localizationNamespace, message, args);
    }
    else if (message.toMessage) {
        m = message.toMessage();
    }
    else {
        m = message;
    }
    this.prepareMessage(m);
    this.batch.push(m);
    logger.info(this, 'session.send()');
...
```

#### <a name="apidoc.element.botbuilder.Message.prototype.upgradeAttachment"></a>[function <span class="apidocSignatureSpan">botbuilder.Message.prototype.</span>upgradeAttachment (a)](#apidoc.element.botbuilder.Message.prototype.upgradeAttachment)
- description and source-code
```javascript
upgradeAttachment = function (a) {
    var isOldSchema = false;
    for (var prop in a) {
        switch (prop) {
            case 'actions':
            case 'fallbackText':
            case 'title':
            case 'titleLink':
            case 'text':
            case 'thumbnailUrl':
                isOldSchema = true;
                break;
        }
    }
    if (isOldSchema) {
        console.warn('Using old attachment schema. Upgrade to new card schema.');
        var v2 = a;
        var card = new HeroCard_1.HeroCard();
        if (v2.title) {
            card.title(v2.title);
        }
        if (v2.text) {
            card.text(v2.text);
        }
        if (v2.thumbnailUrl) {
            card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
        }
        if (v2.titleLink) {
            card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
        }
        if (v2.actions) {
            var list = [];
            for (var i = 0; i < v2.actions.length; i++) {
                var old = v2.actions[i];
                var btn = old.message ?
                    CardAction_1.CardAction.imBack(null, old.message, old.title) :
                    CardAction_1.CardAction.openUrl(null, old.url, old.title);
                if (old.image) {
                    btn.image(old.image);
                }
                list.push(btn);
            }
            card.buttons(list);
        }
        return card.toAttachment();
    }
    else {
        return a;
    }
}
```
- example usage
```shell
...
        }
    }
    return this;
};
Message.prototype.addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
        a = this.upgradeAttachment(a);
        if (!this.data.attachments) {
            this.data.attachments = [a];
        }
        else {
            this.data.attachments.push(a);
        }
    }
...
```



# <a name="apidoc.module.botbuilder.Middleware"></a>[module botbuilder.Middleware](#apidoc.module.botbuilder.Middleware)

#### <a name="apidoc.element.botbuilder.Middleware.Middleware"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Middleware ()](#apidoc.element.botbuilder.Middleware.Middleware)
- description and source-code
```javascript
function Middleware() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Middleware.dialogVersion"></a>[function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>dialogVersion (options)](#apidoc.element.botbuilder.Middleware.dialogVersion)
- description and source-code
```javascript
dialogVersion = function (options) {
    return {
        botbuilder: function (session, next) {
            var cur = session.sessionState.version || 0.0;
            var curMajor = Math.floor(cur);
            var major = Math.floor(options.version);
            if (session.sessionState.callstack.length && curMajor !== major) {
                session.endConversation(options.message || "Sorry. The service was upgraded and we need to start over.");
            }
            else if (options.resetCommand && session.message.text && options.resetCommand.test(session.message.text)) {
                session.endConversation(options.message || "Sorry. The service was upgraded and we need to start over.");
            }
            else {
                session.sessionState.version = options.version;
                next();
            }
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Middleware.firstRun"></a>[function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>firstRun (options)](#apidoc.element.botbuilder.Middleware.firstRun)
- description and source-code
```javascript
firstRun = function (options) {
    return {
        botbuilder: function (session, next) {
            if (session.sessionState.callstack.length == 0) {
                var cur = session.userData[consts.Data.FirstRunVersion] || 0.0;
                var curMajor = Math.floor(cur);
                var major = Math.floor(options.version);
                if (major > curMajor) {
                    session.beginDialog(consts.DialogId.FirstRun, {
                        version: options.version,
                        dialogId: options.dialogId,
                        dialogArgs: options.dialogArgs
                    });
                }
                else if (options.version > cur && options.upgradeDialogId) {
                    session.beginDialog(consts.DialogId.FirstRun, {
                        version: options.version,
                        dialogId: options.upgradeDialogId,
                        dialogArgs: options.upgradeDialogArgs
                    });
                }
                else {
                    next();
                }
            }
            else {
                next();
            }
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Middleware.sendTyping"></a>[function <span class="apidocSignatureSpan">botbuilder.Middleware.</span>sendTyping ()](#apidoc.element.botbuilder.Middleware.sendTyping)
- description and source-code
```javascript
sendTyping = function () {
    return {
        botbuilder: function (session, next) {
            session.sendTyping();
            next();
        }
    };
}
```
- example usage
```shell
...
    return this;
};
Session.prototype.sendTyping = function () {
    this.msgSent = true;
    var m = { type: 'typing' };
    this.prepareMessage(m);
    this.batch.push(m);
    logger.info(this, 'session.sendTyping()');
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
...
```



# <a name="apidoc.module.botbuilder.Prompts"></a>[module botbuilder.Prompts](#apidoc.module.botbuilder.Prompts)

#### <a name="apidoc.element.botbuilder.Prompts.Prompts"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Prompts ()](#apidoc.element.botbuilder.Prompts.Prompts)
- description and source-code
```javascript
function Prompts() {
    return _super !== null && _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.attachment"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>attachment (session, prompt, options)](#apidoc.element.botbuilder.Prompts.attachment)
- description and source-code
```javascript
attachment = function (session, prompt, options) {
    Prompts.validateSession(session);
    var args = options || {};
    args.promptType = PromptType.attachment;
    args.prompt = prompt;
    beginPrompt(session, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.choice"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>choice (session, prompt, choices, options)](#apidoc.element.botbuilder.Prompts.choice)
- description and source-code
```javascript
choice = function (session, prompt, choices, options) {
    Prompts.validateSession(session);
    var args = options || {};
    args.promptType = PromptType.choice;
    args.prompt = prompt;
    args.listStyle = args.hasOwnProperty('listStyle') ? args.listStyle : ListStyle.auto;
    var c = EntityRecognizer_1.EntityRecognizer.expandChoices(choices);
    if (c.length == 0) {
        console.error("0 length choice for prompt:", prompt);
        throw "0 length choice list supplied";
    }
    args.enumValues = c;
    beginPrompt(session, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.configure"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>configure (options)](#apidoc.element.botbuilder.Prompts.configure)
- description and source-code
```javascript
configure = function (options) {
    if (options) {
        for (var key in options) {
            if (options.hasOwnProperty(key)) {
                Prompts.options[key] = options[key];
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.confirm"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>confirm (session, prompt, options)](#apidoc.element.botbuilder.Prompts.confirm)
- description and source-code
```javascript
confirm = function (session, prompt, options) {
    Prompts.validateSession(session);
    var locale = session.preferredLocale();
    var args = options || {};
    args.promptType = PromptType.confirm;
    args.prompt = prompt;
    args.enumValues = [
        session.localizer.gettext(locale, 'confirm_yes', consts.Library.system),
        session.localizer.gettext(locale, 'confirm_no', consts.Library.system)
    ];
    args.listStyle = args.hasOwnProperty('listStyle') ? args.listStyle : ListStyle.auto;
    beginPrompt(session, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.disambiguate"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>disambiguate (session, prompt, choices, options)](#apidoc.element.botbuilder.Prompts.disambiguate)
- description and source-code
```javascript
disambiguate = function (session, prompt, choices, options) {
    Prompts.validateSession(session);
    session.beginDialog(consts.DialogId.Disambiguate, {
        prompt: prompt,
        choices: choices,
        options: options
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.number"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>number (session, prompt, options)](#apidoc.element.botbuilder.Prompts.number)
- description and source-code
```javascript
number = function (session, prompt, options) {
    Prompts.validateSession(session);
    var args = options || {};
    args.promptType = PromptType.number;
    args.prompt = prompt;
    beginPrompt(session, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.text"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>text (session, prompt, options)](#apidoc.element.botbuilder.Prompts.text)
- description and source-code
```javascript
text = function (session, prompt, options) {
    Prompts.validateSession(session);
    var args = options || {};
    args.promptType = PromptType.text;
    args.prompt = prompt;
    beginPrompt(session, args);
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.Prompts.time"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>time (session, prompt, options)](#apidoc.element.botbuilder.Prompts.time)
- description and source-code
```javascript
time = function (session, prompt, options) {
    Prompts.validateSession(session);
    var args = options || {};
    args.promptType = PromptType.time;
    args.prompt = prompt;
    beginPrompt(session, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.validateSession"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.</span>validateSession (session)](#apidoc.element.botbuilder.Prompts.validateSession)
- description and source-code
```javascript
validateSession = function (session) {
    if (!session || typeof session != 'object') {
        throw 'Session should be provided as first parameter.';
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Prompts.prototype"></a>[module botbuilder.Prompts.prototype](#apidoc.module.botbuilder.Prompts.prototype)

#### <a name="apidoc.element.botbuilder.Prompts.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.Prompts.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    args = args || {};
    args.promptAfterAction = args.hasOwnProperty('promptAfterAction') ? args.promptAfterAction : Prompts.options.promptAfterAction
;
    args.retryCnt = 0;
    for (var key in args) {
        if (args.hasOwnProperty(key)) {
            session.dialogData[key] = args[key];
        }
    }
    this.sendPrompt(session, args);
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>constructor ()](#apidoc.element.botbuilder.Prompts.prototype.constructor)
- description and source-code
```javascript
function Prompts() {
    return _super !== null && _super.apply(this, arguments) || this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.createPrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>createPrompt (session, args, retry)](#apidoc.element.botbuilder.Prompts.prototype.createPrompt)
- description and source-code
```javascript
createPrompt = function (session, args, retry) {
    var msg = new Message_1.Message(session);
    var locale = session.preferredLocale();
    var localizationNamespace = args.localizationNamespace;
    var style = ListStyle.none;
    if (args.promptType == PromptType.choice || args.promptType == PromptType.confirm) {
        style = args.listStyle;
        if (style == ListStyle.auto) {
            if (Channel.supportsKeyboards(session, args.enumValues.length)) {
                style = ListStyle.button;
            }
            else if (!retry && args.promptType == PromptType.choice) {
                style = args.enumValues.length < 3 ? ListStyle.inline : ListStyle.list;
            }
            else {
                style = ListStyle.none;
            }
        }
    }
    var prompt;
    if (retry) {
        if (args.retryPrompt) {
            prompt = Message_1.Message.randomPrompt(args.retryPrompt);
        }
        else {
            var type = PromptType[args.promptType];
            prompt = Prompts.defaultRetryPrompt[type];
            localizationNamespace = consts.Library.system;
        }
    }
    else {
        prompt = Message_1.Message.randomPrompt(args.prompt);
    }
    var text = session.localizer.gettext(locale, prompt, localizationNamespace);
    var connector = '';
    var list;
    switch (style) {
        case ListStyle.button:
            var buttons = [];
            for (var i = 0; i < session.dialogData.enumValues.length; i++) {
                var option = session.dialogData.enumValues[i];
                buttons.push(CardAction_1.CardAction.imBack(session, option, option));
            }
            msg.text(text)
                .attachments([new Keyboard_1.Keyboard(session).buttons(buttons)]);
            break;
        case ListStyle.inline:
            list = ' (';
            args.enumValues.forEach(function (v, index) {
                var value = v.toString();
                list += connector + (index + 1) + '. ' + session.localizer.gettext(locale, value, consts.Library.system);
                if (index == args.enumValues.length - 2) {
                    connector = index == 0 ? session.localizer.gettext(locale, "list_or", consts.Library.system) : session.localizer
.gettext(locale, "list_or_more", consts.Library.system);
                }
                else {
                    connector = ', ';
                }
            });
            list += ')';
            msg.text(text + '%s', list);
            break;
        case ListStyle.list:
            list = '\n   ';
            args.enumValues.forEach(function (v, index) {
                var value = v.toString();
                list += connector + (index + 1) + '. ' + session.localizer.gettext(locale, value, args.localizationNamespace);
                connector = '\n   ';
            });
            msg.text(text + '%s', list);
            break;
        default:
            msg.text(text);
            break;
    }
    return msg;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.Prompts.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    var args = session.dialogData;
    if (args.promptAfterAction) {
        this.sendPrompt(session, args);
    }
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.Prompts.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    var args = context.dialogData;
    Prompts.options.recognizer.recognize({
        promptType: args.promptType,
        utterance: context.message.text,
        locale: context.message.textLocale,
        attachments: context.message.attachments,
        enumValues: args.enumValues,
        refDate: args.refDate
    }, function (result) {
        if (result.error) {
            cb(result.error, null);
        }
        else {
            cb(null, result);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.replyReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>replyReceived (session, result)](#apidoc.element.botbuilder.Prompts.prototype.replyReceived)
- description and source-code
```javascript
replyReceived = function (session, result) {
    var args = session.dialogData;
    if (result.error || result.resumed == Dialog_1.ResumeReason.completed) {
        result.promptType = args.promptType;
        session.endDialogWithResult(result);
    }
    else if (typeof args.maxRetries === 'number' && args.retryCnt >= args.maxRetries) {
        result.promptType = args.promptType;
        result.resumed = Dialog_1.ResumeReason.notCompleted;
        session.endDialogWithResult(result);
    }
    else {
        args.retryCnt++;
        this.sendPrompt(session, args, true);
    }
}
```
- example usage
```shell
...
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
...
```

#### <a name="apidoc.element.botbuilder.Prompts.prototype.sendPrompt"></a>[function <span class="apidocSignatureSpan">botbuilder.Prompts.prototype.</span>sendPrompt (session, args, retry)](#apidoc.element.botbuilder.Prompts.prototype.sendPrompt)
- description and source-code
```javascript
sendPrompt = function (session, args, retry) {
    if (retry === void 0) { retry = false; }
    logger.debug("prompts::sendPrompt called");
    var msg;
    if (retry && typeof args.retryPrompt === 'object' && !Array.isArray(args.retryPrompt)) {
        msg = args.retryPrompt;
    }
    else if (typeof args.prompt === 'object' && !Array.isArray(args.prompt)) {
        msg = args.prompt;
    }
    else {
        msg = this.createPrompt(session, args, retry);
    }
    session.send(msg);
    session.sendBatch();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ReceiptCard"></a>[module botbuilder.ReceiptCard](#apidoc.module.botbuilder.ReceiptCard)

#### <a name="apidoc.element.botbuilder.ReceiptCard.ReceiptCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptCard (session)](#apidoc.element.botbuilder.ReceiptCard.ReceiptCard)
- description and source-code
```javascript
function ReceiptCard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.card.receipt',
        content: {}
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ReceiptCard.prototype"></a>[module botbuilder.ReceiptCard.prototype](#apidoc.module.botbuilder.ReceiptCard.prototype)

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.buttons"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>buttons (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.buttons)
- description and source-code
```javascript
buttons = function (list) {
    this.data.content.buttons = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var action = list[i];
            this.data.content.buttons.push(action.toAction ? action.toAction() : action);
        }
    }
    return this;
}
```
- example usage
```shell
...
                    CardAction_1.CardAction.imBack(null, old.message, old.title) :
                    CardAction_1.CardAction.openUrl(null, old.url, old.title);
                if (old.image) {
                    btn.image(old.image);
                }
                list.push(btn);
            }
            card.buttons(list);
        }
        return card.toAttachment();
    }
    else {
        return a;
    }
};
...
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.facts"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>facts (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.facts)
- description and source-code
```javascript
facts = function (list) {
    this.data.content.facts = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var fact = list[i];
            this.data.content.facts.push(fact.toFact ? fact.toFact() : fact);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.items"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>items (list)](#apidoc.element.botbuilder.ReceiptCard.prototype.items)
- description and source-code
```javascript
items = function (list) {
    this.data.content.items = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var item = list[i];
            this.data.content.items.push(item.toItem ? item.toItem() : item);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.tap"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>tap (action)](#apidoc.element.botbuilder.ReceiptCard.prototype.tap)
- description and source-code
```javascript
tap = function (action) {
    if (action) {
        this.data.content.tap = action.toAction ? action.toAction() : action;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
...
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.tax"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>tax (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.tax)
- description and source-code
```javascript
tax = function (v) {
    this.data.content.tax = v || '';
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.title"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>title (text)](#apidoc.element.botbuilder.ReceiptCard.prototype.title)
- description and source-code
```javascript
title = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.title = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
        card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
    }
...
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.toAttachment"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.ReceiptCard.prototype.toAttachment)
- description and source-code
```javascript
toAttachment = function () {
    return this.data;
}
```
- example usage
```shell
...
            this.addAttachment(list[i]);
        }
    }
    return this;
};
Message.prototype.addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
        a = this.upgradeAttachment(a);
        if (!this.data.attachments) {
            this.data.attachments = [a];
        }
        else {
            this.data.attachments.push(a);
        }
...
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.total"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>total (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.total)
- description and source-code
```javascript
total = function (v) {
    this.data.content.total = v || '';
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptCard.prototype.vat"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptCard.prototype.</span>vat (v)](#apidoc.element.botbuilder.ReceiptCard.prototype.vat)
- description and source-code
```javascript
vat = function (v) {
    this.data.content.vat = v || '';
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ReceiptItem"></a>[module botbuilder.ReceiptItem](#apidoc.module.botbuilder.ReceiptItem)

#### <a name="apidoc.element.botbuilder.ReceiptItem.ReceiptItem"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ReceiptItem (session)](#apidoc.element.botbuilder.ReceiptItem.ReceiptItem)
- description and source-code
```javascript
function ReceiptItem(session) {
    this.session = session;
    this.data = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.create"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.</span>create (session, price, title)](#apidoc.element.botbuilder.ReceiptItem.create)
- description and source-code
```javascript
create = function (session, price, title) {
    return new ReceiptItem(session).price(price).title(title);
}
```
- example usage
```shell
...



"use strict";
var __extends = (this && this.__extends) || function (d, b) {
    for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p];
    function __() { this.constructor = d; }
    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());
};
var Dialog_1 = require("./dialogs/Dialog");
var Message_1 = require("./Message");
var consts = require("./consts");
var logger = require("./logger");
var sprintf = require("sprintf-js");
var events = require("events");
...
```



# <a name="apidoc.module.botbuilder.ReceiptItem.prototype"></a>[module botbuilder.ReceiptItem.prototype](#apidoc.module.botbuilder.ReceiptItem.prototype)

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.image"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>image (img)](#apidoc.element.botbuilder.ReceiptItem.prototype.image)
- description and source-code
```javascript
image = function (img) {
    if (img) {
        this.data.image = img.toImage ? img.toImage() : img;
    }
    return this;
}
```
- example usage
```shell
...
        var list = [];
        for (var i = 0; i < v2.actions.length; i++) {
            var old = v2.actions[i];
            var btn = old.message ?
                CardAction_1.CardAction.imBack(null, old.message, old.title) :
                CardAction_1.CardAction.openUrl(null, old.url, old.title);
            if (old.image) {
                btn.image(old.image);
            }
            list.push(btn);
        }
        card.buttons(list);
    }
    return card.toAttachment();
}
...
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.price"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>price (v)](#apidoc.element.botbuilder.ReceiptItem.prototype.price)
- description and source-code
```javascript
price = function (v) {
    this.data.price = v || '';
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.quantity"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>quantity (v)](#apidoc.element.botbuilder.ReceiptItem.prototype.quantity)
- description and source-code
```javascript
quantity = function (v) {
    this.data.quantity = v || '';
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.subtitle"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.subtitle)
- description and source-code
```javascript
subtitle = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.subtitle = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.tap"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>tap (action)](#apidoc.element.botbuilder.ReceiptItem.prototype.tap)
- description and source-code
```javascript
tap = function (action) {
    if (action) {
        this.data.tap = action.toAction ? action.toAction() : action;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
...
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.text"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>text (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.text)
- description and source-code
```javascript
text = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.text = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.title"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>title (text)](#apidoc.element.botbuilder.ReceiptItem.prototype.title)
- description and source-code
```javascript
title = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.title = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
        card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
    }
...
```

#### <a name="apidoc.element.botbuilder.ReceiptItem.prototype.toItem"></a>[function <span class="apidocSignatureSpan">botbuilder.ReceiptItem.prototype.</span>toItem ()](#apidoc.element.botbuilder.ReceiptItem.prototype.toItem)
- description and source-code
```javascript
toItem = function () {
    return this.data;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.RegExpRecognizer"></a>[module botbuilder.RegExpRecognizer](#apidoc.module.botbuilder.RegExpRecognizer)

#### <a name="apidoc.element.botbuilder.RegExpRecognizer.RegExpRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>RegExpRecognizer (intent, expressions)](#apidoc.element.botbuilder.RegExpRecognizer.RegExpRecognizer)
- description and source-code
```javascript
function RegExpRecognizer(intent, expressions) {
    this.intent = intent;
    if (expressions instanceof RegExp || typeof expressions.exec === 'function') {
        this.expressions = { '*': expressions };
    }
    else {
        this.expressions = (expressions || {});
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.RegExpRecognizer.prototype"></a>[module botbuilder.RegExpRecognizer.prototype](#apidoc.module.botbuilder.RegExpRecognizer.prototype)

#### <a name="apidoc.element.botbuilder.RegExpRecognizer.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.RegExpRecognizer.prototype.</span>recognize (context, cb)](#apidoc.element.botbuilder.RegExpRecognizer.prototype.recognize)
- description and source-code
```javascript
recognize = function (context, cb) {
    var result = { score: 0.0, intent: null };
    if (context && context.message && context.message.text) {
        var utterance = context.message.text;
        var locale = context.locale || '*';
        var exp = this.expressions.hasOwnProperty(locale) ? this.expressions[locale] : this.expressions['*'];
        if (exp) {
            var matches = exp.exec(context.message.text);
            if (matches && matches.length) {
                var matched = matches[0];
                result.score = matched.length / context.message.text.length;
                result.intent = this.intent;
                result.expression = exp;
                result.matched = matches;
            }
            cb(null, result);
        }
        else {
            cb(new Error("Expression not found for locale '" + locale + "'."), null);
        }
    }
    else {
        cb(null, result);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.Session"></a>[module botbuilder.Session](#apidoc.module.botbuilder.Session)

#### <a name="apidoc.element.botbuilder.Session.Session"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>Session (options)](#apidoc.element.botbuilder.Session.Session)
- description and source-code
```javascript
function Session(options) {
    var _this = _super.call(this) || this;
    _this.options = options;
    _this.msgSent = false;
    _this._isReset = false;
    _this.lastSendTime = new Date().getTime();
    _this.batch = [];
    _this.batchStarted = false;
    _this.sendingBatch = false;
    _this.inMiddleware = false;
    _this._locale = null;
    _this.localizer = null;
    _this.library = options.library;
    _this.localizer = options.localizer;
    if (typeof _this.options.autoBatchDelay !== 'number') {
        _this.options.autoBatchDelay = 250;
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.EventEmitter"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>EventEmitter ()](#apidoc.element.botbuilder.Session.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.activeDialogStackEntry"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>activeDialogStackEntry (stack)](#apidoc.element.botbuilder.Session.activeDialogStackEntry)
- description and source-code
```javascript
activeDialogStackEntry = function (stack) {
    return stack && stack.length > 0 ? stack[stack.length - 1] : null;
}
```
- example usage
```shell
...
    stack.push(entry);
    return entry;
};
Session.popDialogStackEntry = function (stack) {
    if (stack && stack.length > 0) {
        stack.pop();
    }
    return Session.activeDialogStackEntry(stack);
};
Session.pruneDialogStack = function (stack, start) {
    if (stack && stack.length > 0) {
        stack.splice(start);
    }
    return Session.activeDialogStackEntry(stack);
};
...
```

#### <a name="apidoc.element.botbuilder.Session.findDialogStackEntry"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>findDialogStackEntry (stack, dialogId, reverse)](#apidoc.element.botbuilder.Session.findDialogStackEntry)
- description and source-code
```javascript
findDialogStackEntry = function (stack, dialogId, reverse) {
    if (reverse === void 0) { reverse = false; }
    var step = reverse ? -1 : 1;
    var l = stack ? stack.length : 0;
    for (var i = step > 0 ? 0 : l - 1; i >= 0 && i < l; i += step) {
        if (stack[i].id === dialogId) {
            return i;
        }
    }
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.forEachDialogStackEntry"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>forEachDialogStackEntry (stack, reverse, fn)](#apidoc.element.botbuilder.Session.forEachDialogStackEntry)
- description and source-code
```javascript
forEachDialogStackEntry = function (stack, reverse, fn) {
    var step = reverse ? -1 : 1;
    var l = stack ? stack.length : 0;
    for (var i = step > 0 ? 0 : l - 1; i >= 0 && i < l; i += step) {
        fn(stack[i], i);
    }
}
```
- example usage
```shell
...
    if (stack && stack.length > 0) {
        stack.splice(start);
    }
    return Session.activeDialogStackEntry(stack);
};
Session.validateDialogStack = function (stack, root) {
    var valid = true;
    Session.forEachDialogStackEntry(stack, false, function (entry) {
        var pair = entry.id.split(':');
        if (!root.findDialog(pair[0], pair[1])) {
            valid = false;
        }
    });
    return valid;
};
...
```

#### <a name="apidoc.element.botbuilder.Session.init"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>init ()](#apidoc.element.botbuilder.Session.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.listenerCount"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.Session.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.popDialogStackEntry"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>popDialogStackEntry (stack)](#apidoc.element.botbuilder.Session.popDialogStackEntry)
- description and source-code
```javascript
popDialogStackEntry = function (stack) {
    if (stack && stack.length > 0) {
        stack.pop();
    }
    return Session.activeDialogStackEntry(stack);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.pruneDialogStack"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>pruneDialogStack (stack, start)](#apidoc.element.botbuilder.Session.pruneDialogStack)
- description and source-code
```javascript
pruneDialogStack = function (stack, start) {
    if (stack && stack.length > 0) {
        stack.splice(start);
    }
    return Session.activeDialogStackEntry(stack);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.pushDialogStackEntry"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>pushDialogStackEntry (stack, entry)](#apidoc.element.botbuilder.Session.pushDialogStackEntry)
- description and source-code
```javascript
pushDialogStackEntry = function (stack, entry) {
    if (!entry.state) {
        entry.state = {};
    }
    stack = stack || [];
    stack.push(entry);
    return entry;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.validateDialogStack"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.</span>validateDialogStack (stack, root)](#apidoc.element.botbuilder.Session.validateDialogStack)
- description and source-code
```javascript
validateDialogStack = function (stack, root) {
    var valid = true;
    Session.forEachDialogStackEntry(stack, false, function (entry) {
        var pair = entry.id.split(':');
        if (!root.findDialog(pair[0], pair[1])) {
            valid = false;
        }
    });
    return valid;
}
```
- example usage
```shell
...
            valid = false;
        }
    });
    return valid;
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
...
```



# <a name="apidoc.module.botbuilder.Session.prototype"></a>[module botbuilder.Session.prototype](#apidoc.module.botbuilder.Session.prototype)

#### <a name="apidoc.element.botbuilder.Session.prototype.beginDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>beginDialog (id, args)](#apidoc.element.botbuilder.Session.prototype.beginDialog)
- description and source-code
```javascript
beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
}
```
- example usage
```shell
...
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.cancelDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>cancelDialog (dialogId, replaceWithId, replaceWithArgs)](#apidoc.element.botbuilder.Session.prototype.cancelDialog)
- description and source-code
```javascript
cancelDialog = function (dialogId, replaceWithId, replaceWithArgs) {
    var childId = typeof dialogId === 'number' ? this.sessionState.callstack[dialogId].id : dialogId;
    var cur = this.deleteDialogs(dialogId);
    if (replaceWithId) {
        logger.info(this, 'session.cancelDialog(%s)', replaceWithId);
        var id = this.resolveDialogId(replaceWithId);
        var dialog = this.findDialog(id);
        this.pushDialog({ id: id, state: {} });
        this.startBatch();
        dialog.begin(this, replaceWithArgs);
    }
    else {
        logger.info(this, 'session.cancelDialog()');
        this.startBatch();
        if (cur) {
            var dialog = this.findDialog(cur.id);
            if (dialog) {
                dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.canceled, response: null, childId: childId });
            }
            else {
                this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
            }
        }
    }
    return this;
}
```
- example usage
```shell
...
    }
    return this;
};
Session.prototype.cancelDialog = function (dialogId, replaceWithId, replaceWithArgs) {
    var childId = typeof dialogId === 'number' ? this.sessionState.callstack[dialogId].id : dialogId;
    var cur = this.deleteDialogs(dialogId);
    if (replaceWithId) {
        logger.info(this, 'session.cancelDialog(%s)', replaceWithId);
        var id = this.resolveDialogId(replaceWithId);
        var dialog = this.findDialog(id);
        this.pushDialog({ id: id, state: {} });
        this.startBatch();
        dialog.begin(this, replaceWithArgs);
    }
    else {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.clearDialogStack"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>clearDialogStack ()](#apidoc.element.botbuilder.Session.prototype.clearDialogStack)
- description and source-code
```javascript
clearDialogStack = function () {
    this.sessionState.callstack = [];
    this.dialogData = null;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>constructor (options)](#apidoc.element.botbuilder.Session.prototype.constructor)
- description and source-code
```javascript
function Session(options) {
    var _this = _super.call(this) || this;
    _this.options = options;
    _this.msgSent = false;
    _this._isReset = false;
    _this.lastSendTime = new Date().getTime();
    _this.batch = [];
    _this.batchStarted = false;
    _this.sendingBatch = false;
    _this.inMiddleware = false;
    _this._locale = null;
    _this.localizer = null;
    _this.library = options.library;
    _this.localizer = options.localizer;
    if (typeof _this.options.autoBatchDelay !== 'number') {
        _this.options.autoBatchDelay = 250;
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.createMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>createMessage (localizationNamespace, text, args)](#apidoc.element.botbuilder.Session.prototype.createMessage)
- description and source-code
```javascript
createMessage = function (localizationNamespace, text, args) {
    var message = new Message_1.Message(this)
        .text(this.vgettext(localizationNamespace, Message_1.Message.randomPrompt(text), args));
    return message.toMessage();
}
```
- example usage
```shell
...
for (var _i = 2; _i < arguments.length; _i++) {
    args[_i - 2] = arguments[_i];
}
this.msgSent = true;
if (message) {
    var m;
    if (typeof message == 'string' || Array.isArray(message)) {
        m = this.createMessage(localizationNamespace, message, args);
    }
    else if (message.toMessage) {
        m = message.toMessage();
    }
    else {
        m = message;
    }
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.curDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>curDialog ()](#apidoc.element.botbuilder.Session.prototype.curDialog)
- description and source-code
```javascript
curDialog = function () {
    var cur;
    var ss = this.sessionState;
    if (ss.callstack.length > 0) {
        cur = ss.callstack[ss.callstack.length - 1];
    }
    return cur;
}
```
- example usage
```shell
...
    else {
        _this.inMiddleware = false;
        _this.sessionState.lastAccess = now;
        done();
    }
};
this.sessionState = sessionState || { callstack: [], lastAccess: now, version: 0.0 };
var cur = this.curDialog();
if (cur) {
    this.dialogData = cur.state;
}
this.inMiddleware = true;
this.message = (message || { text: '' });
if (!this.message.type) {
    this.message.type = consts.messageType;
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.curLibraryName"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>curLibraryName ()](#apidoc.element.botbuilder.Session.prototype.curLibraryName)
- description and source-code
```javascript
curLibraryName = function () {
    var cur = this.curDialog();
    return cur && !this.inMiddleware ? cur.id.split(':')[0] : this.library.name;
}
```
- example usage
```shell
...
    return this._locale;
};
Session.prototype.gettext = function (messageid) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    return this.vgettext(this.curLibraryName(), messageid, args);
};
Session.prototype.ngettext = function (messageid, messageid_plural, count) {
    var tmpl;
    if (this.localizer && this.message) {
        tmpl = this.localizer.ngettext(this.preferredLocale(), messageid, messageid_plural, count, this.curLibraryName());
    }
    else if (count == 1) {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.deleteDialogs"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>deleteDialogs (dialogId)](#apidoc.element.botbuilder.Session.prototype.deleteDialogs)
- description and source-code
```javascript
deleteDialogs = function (dialogId) {
    var ss = this.sessionState;
    var index = -1;
    if (typeof dialogId === 'string') {
        for (var i = ss.callstack.length - 1; i >= 0; i--) {
            if (ss.callstack[i].id == dialogId) {
                index = i;
                break;
            }
        }
    }
    else {
        index = dialogId;
    }
    if (index < 0 && index < ss.callstack.length) {
        throw new Error('Unable to cancel dialog. Dialog[' + dialogId + '] not found.');
    }
    ss.callstack.splice(index);
    var cur = this.curDialog();
    this.dialogData = cur ? cur.state : null;
    return cur;
}
```
- example usage
```shell
...
            }
        }
    }
    return this;
};
Session.prototype.cancelDialog = function (dialogId, replaceWithId, replaceWithArgs) {
    var childId = typeof dialogId === 'number' ? this.sessionState.callstack[dialogId].id : dialogId;
    var cur = this.deleteDialogs(dialogId);
    if (replaceWithId) {
        logger.info(this, 'session.cancelDialog(%s)', replaceWithId);
        var id = this.resolveDialogId(replaceWithId);
        var dialog = this.findDialog(id);
        this.pushDialog({ id: id, state: {} });
        this.startBatch();
        dialog.begin(this, replaceWithArgs);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.dialogStack"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>dialogStack (newStack)](#apidoc.element.botbuilder.Session.prototype.dialogStack)
- description and source-code
```javascript
dialogStack = function (newStack) {
    var stack;
    if (newStack) {
        stack = this.sessionState.callstack = newStack;
        this.dialogData = stack.length > 0 ? stack[stack.length - 1].state : null;
    }
    else {
        stack = this.sessionState.callstack || [];
        if (stack.length > 0) {
            stack[stack.length - 1].state = this.dialogData || {};
        }
    }
    return stack.slice(0);
}
```
- example usage
```shell
...
var _this = this;
return {
    message: this.message,
    userData: this.userData,
    conversationData: this.conversationData,
    privateConversationData: this.privateConversationData,
    localizer: this.localizer,
    dialogStack: function () { return _this.dialogStack(); },
    preferredLocale: function () { return _this.preferredLocale(); },
    gettext: function () {
        var args = [];
        for (var _i = 0; _i < arguments.length; _i++) {
            args[_i] = arguments[_i];
        }
        return Session.prototype.gettext.call(_this, args);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>dispatch (sessionState, message, done)](#apidoc.element.botbuilder.Session.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (sessionState, message, done) {
    var _this = this;
    var index = 0;
    var session = this;
    var now = new Date().getTime();
    var middleware = this.options.middleware || [];
    var next = function () {
        var handler = index < middleware.length ? middleware[index] : null;
        if (handler) {
            index++;
            handler(session, next);
        }
        else {
            _this.inMiddleware = false;
            _this.sessionState.lastAccess = now;
            done();
        }
    };
    this.sessionState = sessionState || { callstack: [], lastAccess: now, version: 0.0 };
    var cur = this.curDialog();
    if (cur) {
        this.dialogData = cur.state;
    }
    this.inMiddleware = true;
    this.message = (message || { text: '' });
    if (!this.message.type) {
        this.message.type = consts.messageType;
    }
    var locale = this.preferredLocale();
    this.localizer.load(locale, function (err) {
        if (err) {
            _this.error(err);
        }
        else {
            next();
        }
    });
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.endConversation"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endConversation (message)](#apidoc.element.botbuilder.Session.prototype.endConversation)
- description and source-code
```javascript
endConversation = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    var m;
    if (message) {
        if (typeof message == 'string' || Array.isArray(message)) {
            m = this.createMessage(this.curLibraryName(), message, args);
        }
        else if (message.toMessage) {
            m = message.toMessage();
        }
        else {
            m = message;
        }
        this.msgSent = true;
        this.prepareMessage(m);
        this.batch.push(m);
    }
    this.privateConversationData = {};
    logger.info(this, 'session.endConversation()');
    var ss = this.sessionState;
    ss.callstack = [];
    this.sendBatch();
    return this;
}
```
- example usage
```shell
...
        }
    });
    return this;
};
Session.prototype.error = function (err) {
    logger.info(this, 'session.error()');
    if (this.options.dialogErrorMessage) {
        this.endConversation(this.options.dialogErrorMessage);
    }
    else {
        var locale = this.preferredLocale();
        this.endConversation(this.localizer.gettext(locale, 'default_error', consts.Library.system));
    }
    var m = err.toString();
    err = err instanceof Error ? err : new Error(m);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.endDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endDialog (message)](#apidoc.element.botbuilder.Session.prototype.endDialog)
- description and source-code
```javascript
endDialog = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (typeof message === 'object' && (message.hasOwnProperty('response') || message.hasOwnProperty('resumed') || message.hasOwnProperty
('error'))) {
        console.warn('Returning results via Session.endDialog() is deprecated. Use Session.endDialogWithResult() instead.');
        return this.endDialogWithResult(message);
    }
    var cur = this.curDialog();
    if (cur) {
        var m;
        if (message) {
            if (typeof message == 'string' || Array.isArray(message)) {
                m = this.createMessage(this.curLibraryName(), message, args);
            }
            else if (message.toMessage) {
                m = message.toMessage();
            }
            else {
                m = message;
            }
            this.msgSent = true;
            this.prepareMessage(m);
            this.batch.push(m);
        }
        logger.info(this, 'session.endDialog()');
        var childId = cur.id;
        cur = this.popDialog();
        this.startBatch();
        if (cur) {
            var dialog = this.findDialog(cur.id);
            if (dialog) {
                dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
            }
            else {
                this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
            }
        }
    }
    return this;
}
```
- example usage
```shell
...
};
Session.prototype.endDialog = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (typeof message === 'object' && (message.hasOwnProperty('response') || message.hasOwnProperty('resumed') || message.hasOwnProperty
('error'))) {
        console.warn('Returning results via Session.endDialog() is deprecated. Use Session.endDialogWithResult() instead.');
        return this.endDialogWithResult(message);
    }
    var cur = this.curDialog();
    if (cur) {
        var m;
        if (message) {
            if (typeof message == 'string' || Array.isArray(message)) {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.endDialogWithResult"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>endDialogWithResult (result)](#apidoc.element.botbuilder.Session.prototype.endDialogWithResult)
- description and source-code
```javascript
endDialogWithResult = function (result) {
    var cur = this.curDialog();
    if (cur) {
        result = result || {};
        if (!result.hasOwnProperty('resumed')) {
            result.resumed = Dialog_1.ResumeReason.completed;
        }
        result.childId = cur.id;
        logger.info(this, 'session.endDialogWithResult()');
        cur = this.popDialog();
        this.startBatch();
        if (cur) {
            var dialog = this.findDialog(cur.id);
            if (dialog) {
                dialog.dialogResumed(this, result);
            }
            else {
                this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
            }
        }
    }
    return this;
}
```
- example usage
```shell
...
};
Session.prototype.endDialog = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (typeof message === 'object' && (message.hasOwnProperty('response') || message.hasOwnProperty('resumed') || message.hasOwnProperty
('error'))) {
        console.warn('Returning results via Session.endDialog() is deprecated. Use Session.endDialogWithResult() instead.');
        return this.endDialogWithResult(message);
    }
    var cur = this.curDialog();
    if (cur) {
        var m;
        if (message) {
            if (typeof message == 'string' || Array.isArray(message)) {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.error"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>error (err)](#apidoc.element.botbuilder.Session.prototype.error)
- description and source-code
```javascript
error = function (err) {
    logger.info(this, 'session.error()');
    if (this.options.dialogErrorMessage) {
        this.endConversation(this.options.dialogErrorMessage);
    }
    else {
        var locale = this.preferredLocale();
        this.endConversation(this.localizer.gettext(locale, 'default_error', consts.Library.system));
    }
    var m = err.toString();
    err = err instanceof Error ? err : new Error(m);
    this.emit('error', err);
    return this;
}
```
- example usage
```shell
...
    if (file.substring(file.length - 5).toLowerCase() == ".json") {
        logger.debug("localizer.load(%s) - Loading %s/%s", locale, dir, file);
        _this.parseFile(locale, dir, file)
            .then(function (count) {
            entryCount += count;
            cb();
        }, function (err) {
            logger.error("localizer.load(%s) - Error reading %s/%s: %s", locale, dir, file, err.toString());
            cb();
        });
    }
    else {
        cb();
    }
});
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.findDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>findDialog (id)](#apidoc.element.botbuilder.Session.prototype.findDialog)
- description and source-code
```javascript
findDialog = function (id) {
    var parts = id.split(':');
    return this.library.findDialog(parts[0] || this.library.name, parts[1]);
}
```
- example usage
```shell
...
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.getMessageReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>getMessageReceived ()](#apidoc.element.botbuilder.Session.prototype.getMessageReceived)
- description and source-code
```javascript
getMessageReceived = function () {
    console.warn("Session.getMessageReceived() is deprecated. Use Session.message.sourceEvent instead.");
    return this.message.sourceEvent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.gettext"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>gettext (messageid)](#apidoc.element.botbuilder.Session.prototype.gettext)
- description and source-code
```javascript
gettext = function (messageid) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    return this.vgettext(this.curLibraryName(), messageid, args);
}
```
- example usage
```shell
...
    }
    return text ? this.getValue(text) : null;
};
DefaultLocalizer.prototype.gettext = function (locale, msgid, ns) {
    return this.trygettext(locale, msgid, ns) || msgid;
};
DefaultLocalizer.prototype.ngettext = function (locale, msgid, msgid_plural, count, ns) {
    return count == 1 ? this.gettext(locale, msgid, ns) : this.gettext(locale, msgid_plural, ns);
};
DefaultLocalizer.prototype.getFallback = function (locale) {
    if (locale) {
        var split = locale.indexOf("-");
        if (split != -1) {
            return locale.substring(0, split);
        }
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.isReset"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>isReset ()](#apidoc.element.botbuilder.Session.prototype.isReset)
- description and source-code
```javascript
isReset = function () {
    return this._isReset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.messageSent"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>messageSent ()](#apidoc.element.botbuilder.Session.prototype.messageSent)
- description and source-code
```javascript
messageSent = function () {
    return this.msgSent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.ngettext"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>ngettext (messageid, messageid_plural, count)](#apidoc.element.botbuilder.Session.prototype.ngettext)
- description and source-code
```javascript
ngettext = function (messageid, messageid_plural, count) {
    var tmpl;
    if (this.localizer && this.message) {
        tmpl = this.localizer.ngettext(this.preferredLocale(), messageid, messageid_plural, count, this.curLibraryName());
    }
    else if (count == 1) {
        tmpl = messageid;
    }
    else {
        tmpl = messageid_plural;
    }
    return sprintf.sprintf(tmpl, count);
}
```
- example usage
```shell
...
        args[_i - 1] = arguments[_i];
    }
    return this.vgettext(this.curLibraryName(), messageid, args);
};
Session.prototype.ngettext = function (messageid, messageid_plural, count) {
    var tmpl;
    if (this.localizer && this.message) {
        tmpl = this.localizer.ngettext(this.preferredLocale(), messageid, messageid_plural, count, this.curLibraryName());
    }
    else if (count == 1) {
        tmpl = messageid;
    }
    else {
        tmpl = messageid_plural;
    }
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.popDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>popDialog ()](#apidoc.element.botbuilder.Session.prototype.popDialog)
- description and source-code
```javascript
popDialog = function () {
    var ss = this.sessionState;
    if (ss.callstack.length > 0) {
        ss.callstack.pop();
    }
    var cur = this.curDialog();
    this.dialogData = cur ? cur.state : null;
    return cur;
}
```
- example usage
```shell
...
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.popDialog();
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.endConversation = function (message) {
    var args = [];
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.preferredLocale"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>preferredLocale (locale, callback)](#apidoc.element.botbuilder.Session.prototype.preferredLocale)
- description and source-code
```javascript
preferredLocale = function (locale, callback) {
    if (locale) {
        this._locale = locale;
        if (this.userData) {
            this.userData[consts.Data.PreferredLocale] = locale;
        }
        if (this.localizer) {
            this.localizer.load(locale, callback);
        }
    }
    else if (!this._locale) {
        if (this.userData && this.userData[consts.Data.PreferredLocale]) {
            this._locale = this.userData[consts.Data.PreferredLocale];
        }
        else if (this.message && this.message.textLocale) {
            this._locale = this.message.textLocale;
        }
        else if (this.localizer) {
            this._locale = this.localizer.defaultLocale();
        }
    }
    return this._locale;
}
```
- example usage
```shell
...
        return {
message: this.message,
userData: this.userData,
conversationData: this.conversationData,
privateConversationData: this.privateConversationData,
localizer: this.localizer,
dialogStack: function () { return _this.dialogStack(); },
preferredLocale: function () { return _this.preferredLocale(); },
gettext: function () {
    var args = [];
    for (var _i = 0; _i < arguments.length; _i++) {
        args[_i] = arguments[_i];
    }
    return Session.prototype.gettext.call(_this, args);
},
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.prepareMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>prepareMessage (msg)](#apidoc.element.botbuilder.Session.prototype.prepareMessage)
- description and source-code
```javascript
prepareMessage = function (msg) {
    if (!msg.type) {
        msg.type = 'message';
    }
    if (!msg.address) {
        msg.address = this.message.address;
    }
    if (!msg.textLocale && this.message.textLocale) {
        msg.textLocale = this.message.textLocale;
    }
}
```
- example usage
```shell
...
        }
        else if (message.toMessage) {
            m = message.toMessage();
        }
        else {
            m = message;
        }
        this.prepareMessage(m);
        this.batch.push(m);
        logger.info(this, 'session.send()');
    }
    this.startBatch();
    return this;
};
Session.prototype.sendTyping = function () {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.pushDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>pushDialog (ds)](#apidoc.element.botbuilder.Session.prototype.pushDialog)
- description and source-code
```javascript
pushDialog = function (ds) {
    var ss = this.sessionState;
    var cur = this.curDialog();
    if (cur) {
        cur.state = this.dialogData || {};
    }
    ss.callstack.push(ds);
    this.dialogData = ds.state || {};
    return ds;
}
```
- example usage
```shell
...
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.replaceDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>replaceDialog (id, args)](#apidoc.element.botbuilder.Session.prototype.replaceDialog)
- description and source-code
```javascript
replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.popDialog();
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
}
```
- example usage
```shell
...
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.popDialog();
    this.pushDialog({ id: id, state: {} });
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.reset"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>reset (dialogId, dialogArgs)](#apidoc.element.botbuilder.Session.prototype.reset)
- description and source-code
```javascript
reset = function (dialogId, dialogArgs) {
    logger.info(this, 'session.reset()');
    this._isReset = true;
    this.sessionState.callstack = [];
    if (!dialogId) {
        dialogId = this.options.dialogId;
        dialogArgs = this.options.dialogArgs;
    }
    this.beginDialog(dialogId, dialogArgs);
    return this;
}
```
- example usage
```shell
...
                this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
            }
        }
    }
    return this;
};
Session.prototype.reset = function (dialogId, dialogArgs) {
    logger.info(this, 'session.reset()');
    this._isReset = true;
    this.sessionState.callstack = [];
    if (!dialogId) {
        dialogId = this.options.dialogId;
        dialogArgs = this.options.dialogArgs;
    }
    this.beginDialog(dialogId, dialogArgs);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.resolveDialogId"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>resolveDialogId (id)](#apidoc.element.botbuilder.Session.prototype.resolveDialogId)
- description and source-code
```javascript
resolveDialogId = function (id) {
    return id.indexOf(':') >= 0 ? id : this.curLibraryName() + ':' + id;
}
```
- example usage
```shell
...
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.routeToActiveDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>routeToActiveDialog (recognizeResult)](#apidoc.element.botbuilder.Session.prototype.routeToActiveDialog)
- description and source-code
```javascript
routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.save"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>save ()](#apidoc.element.botbuilder.Session.prototype.save)
- description and source-code
```javascript
save = function () {
    logger.info(this, 'session.save()');
    this.startBatch();
    return this;
}
```
- example usage
```shell
...
    }
    else {
        tmpl = messageid_plural;
    }
    return sprintf.sprintf(tmpl, count);
};
Session.prototype.save = function () {
    logger.info(this, 'session.save()');
    this.startBatch();
    return this;
};
Session.prototype.send = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.send"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>send (message)](#apidoc.element.botbuilder.Session.prototype.send)
- description and source-code
```javascript
send = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    args.unshift(this.curLibraryName(), message);
    return Session.prototype.sendLocalized.apply(this, args);
}
```
- example usage
```shell
...
// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
    console.log('%s listening to %s', server.name, server.url);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.sendBatch"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendBatch (callback)](#apidoc.element.botbuilder.Session.prototype.sendBatch)
- description and source-code
```javascript
sendBatch = function (callback) {
    var _this = this;
    logger.info(this, 'session.sendBatch() sending %d messages', this.batch.length);
    if (this.sendingBatch) {
        return;
    }
    if (this.batchTimer) {
        clearTimeout(this.batchTimer);
        this.batchTimer = null;
    }
    this.batchTimer = null;
    var batch = this.batch;
    this.batch = [];
    this.batchStarted = false;
    this.sendingBatch = true;
    var cur = this.curDialog();
    if (cur) {
        cur.state = this.dialogData;
    }
    this.options.onSave(function (err) {
        if (!err) {
            if (batch.length) {
                _this.options.onSend(batch, function (err) {
                    _this.sendingBatch = false;
                    if (_this.batchStarted) {
                        _this.startBatch();
                    }
                    if (callback) {
                        callback(err);
                    }
                });
            }
            else {
                _this.sendingBatch = false;
                if (_this.batchStarted) {
                    _this.startBatch();
                }
                if (callback) {
                    callback(err);
                }
            }
        }
        else {
            _this.sendingBatch = false;
            switch (err.code || '') {
                case consts.Errors.EBADMSG:
                case consts.Errors.EMSGSIZE:
                    _this.userData = {};
                    _this.batch = [];
                    _this.endConversation(_this.options.dialogErrorMessage || 'Oops. Something went wrong and we need to start over
.');
                    break;
            }
            if (callback) {
                callback(err);
            }
        }
    });
}
```
- example usage
```shell
...
};
Session.prototype.sendTyping = function () {
    this.msgSent = true;
    var m = { type: 'typing' };
    this.prepareMessage(m);
    this.batch.push(m);
    logger.info(this, 'session.sendTyping()');
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.sendLocalized"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendLocalized (localizationNamespace, message)](#apidoc.element.botbuilder.Session.prototype.sendLocalized)
- description and source-code
```javascript
sendLocalized = function (localizationNamespace, message) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    this.msgSent = true;
    if (message) {
        var m;
        if (typeof message == 'string' || Array.isArray(message)) {
            m = this.createMessage(localizationNamespace, message, args);
        }
        else if (message.toMessage) {
            m = message.toMessage();
        }
        else {
            m = message;
        }
        this.prepareMessage(m);
        this.batch.push(m);
        logger.info(this, 'session.send()');
    }
    this.startBatch();
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.sendTyping"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>sendTyping ()](#apidoc.element.botbuilder.Session.prototype.sendTyping)
- description and source-code
```javascript
sendTyping = function () {
    this.msgSent = true;
    var m = { type: 'typing' };
    this.prepareMessage(m);
    this.batch.push(m);
    logger.info(this, 'session.sendTyping()');
    this.sendBatch();
    return this;
}
```
- example usage
```shell
...
    return this;
};
Session.prototype.sendTyping = function () {
    this.msgSent = true;
    var m = { type: 'typing' };
    this.prepareMessage(m);
    this.batch.push(m);
    logger.info(this, 'session.sendTyping()');
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.startBatch"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>startBatch ()](#apidoc.element.botbuilder.Session.prototype.startBatch)
- description and source-code
```javascript
startBatch = function () {
    var _this = this;
    this.batchStarted = true;
    if (!this.sendingBatch) {
        if (this.batchTimer) {
            clearTimeout(this.batchTimer);
        }
        this.batchTimer = setTimeout(function () {
            _this.sendBatch();
        }, this.options.autoBatchDelay);
    }
}
```
- example usage
```shell
...
    else {
        tmpl = messageid_plural;
    }
    return sprintf.sprintf(tmpl, count);
};
Session.prototype.save = function () {
    logger.info(this, 'session.save()');
    this.startBatch();
    return this;
};
Session.prototype.send = function (message) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
...
```

#### <a name="apidoc.element.botbuilder.Session.prototype.toRecognizeContext"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>toRecognizeContext ()](#apidoc.element.botbuilder.Session.prototype.toRecognizeContext)
- description and source-code
```javascript
toRecognizeContext = function () {
    var _this = this;
    return {
        message: this.message,
        userData: this.userData,
        conversationData: this.conversationData,
        privateConversationData: this.privateConversationData,
        localizer: this.localizer,
        dialogStack: function () { return _this.dialogStack(); },
        preferredLocale: function () { return _this.preferredLocale(); },
        gettext: function () {
            var args = [];
            for (var _i = 0; _i < arguments.length; _i++) {
                args[_i] = arguments[_i];
            }
            return Session.prototype.gettext.call(_this, args);
        },
        ngettext: function () {
            var args = [];
            for (var _i = 0; _i < arguments.length; _i++) {
                args[_i] = arguments[_i];
            }
            return Session.prototype.ngettext.call(_this, args);
        },
        locale: this.preferredLocale()
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.validateCallstack"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>validateCallstack ()](#apidoc.element.botbuilder.Session.prototype.validateCallstack)
- description and source-code
```javascript
validateCallstack = function () {
    var ss = this.sessionState;
    for (var i = 0; i < ss.callstack.length; i++) {
        var id = ss.callstack[i].id;
        if (!this.findDialog(id)) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.Session.prototype.vgettext"></a>[function <span class="apidocSignatureSpan">botbuilder.Session.prototype.</span>vgettext (localizationNamespace, messageid, args)](#apidoc.element.botbuilder.Session.prototype.vgettext)
- description and source-code
```javascript
vgettext = function (localizationNamespace, messageid, args) {
    var tmpl;
    if (this.localizer && this.message) {
        tmpl = this.localizer.gettext(this.preferredLocale(), messageid, localizationNamespace);
    }
    else {
        tmpl = messageid;
    }
    return args && args.length > 0 ? sprintf.vsprintf(tmpl, args) : tmpl;
}
```
- example usage
```shell
...
    return this._locale;
};
Session.prototype.gettext = function (messageid) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    return this.vgettext(this.curLibraryName(), messageid, args);
};
Session.prototype.ngettext = function (messageid, messageid_plural, count) {
    var tmpl;
    if (this.localizer && this.message) {
        tmpl = this.localizer.ngettext(this.preferredLocale(), messageid, messageid_plural, count, this.curLibraryName());
    }
    else if (count == 1) {
...
```



# <a name="apidoc.module.botbuilder.SigninCard"></a>[module botbuilder.SigninCard](#apidoc.module.botbuilder.SigninCard)

#### <a name="apidoc.element.botbuilder.SigninCard.SigninCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SigninCard (session)](#apidoc.element.botbuilder.SigninCard.SigninCard)
- description and source-code
```javascript
function SigninCard(session) {
    this.session = session;
    this.data = {
        contentType: 'application/vnd.microsoft.card.signin',
        content: {}
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.SigninCard.prototype"></a>[module botbuilder.SigninCard.prototype](#apidoc.module.botbuilder.SigninCard.prototype)

#### <a name="apidoc.element.botbuilder.SigninCard.prototype.button"></a>[function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>button (title, url)](#apidoc.element.botbuilder.SigninCard.prototype.button)
- description and source-code
```javascript
button = function (title, url) {
    if (title && url) {
        this.data.content.buttons = [{
                type: 'signin',
                title: Message_1.fmtText(this.session, title),
                value: url
            }];
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.SigninCard.prototype.text"></a>[function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>text (prompts)](#apidoc.element.botbuilder.SigninCard.prototype.text)
- description and source-code
```javascript
text = function (prompts) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (prompts) {
        this.data.content.text = Message_1.fmtText(this.session, prompts, args);
    }
    return this;
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.SigninCard.prototype.toAttachment"></a>[function <span class="apidocSignatureSpan">botbuilder.SigninCard.prototype.</span>toAttachment ()](#apidoc.element.botbuilder.SigninCard.prototype.toAttachment)
- description and source-code
```javascript
toAttachment = function () {
    return this.data;
}
```
- example usage
```shell
...
            this.addAttachment(list[i]);
        }
    }
    return this;
};
Message.prototype.addAttachment = function (attachment) {
    if (attachment) {
        var a = attachment.toAttachment ? attachment.toAttachment() : attachment;
        a = this.upgradeAttachment(a);
        if (!this.data.attachments) {
            this.data.attachments = [a];
        }
        else {
            this.data.attachments.push(a);
        }
...
```



# <a name="apidoc.module.botbuilder.SimpleDialog"></a>[module botbuilder.SimpleDialog](#apidoc.module.botbuilder.SimpleDialog)

#### <a name="apidoc.element.botbuilder.SimpleDialog.SimpleDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SimpleDialog (fn)](#apidoc.element.botbuilder.SimpleDialog.SimpleDialog)
- description and source-code
```javascript
function SimpleDialog(fn) {
    var _this = _super.call(this) || this;
    _this.fn = fn;
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.SimpleDialog.prototype"></a>[module botbuilder.SimpleDialog.prototype](#apidoc.module.botbuilder.SimpleDialog.prototype)

#### <a name="apidoc.element.botbuilder.SimpleDialog.prototype.begin"></a>[function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>begin (session, args)](#apidoc.element.botbuilder.SimpleDialog.prototype.begin)
- description and source-code
```javascript
begin = function (session, args) {
    this.fn(session, args);
}
```
- example usage
```shell
...
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
    dialog.begin(this, args);
    return this;
};
Session.prototype.replaceDialog = function (id, args) {
    logger.info(this, 'session.replaceDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
...
```

#### <a name="apidoc.element.botbuilder.SimpleDialog.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>constructor (fn)](#apidoc.element.botbuilder.SimpleDialog.prototype.constructor)
- description and source-code
```javascript
function SimpleDialog(fn) {
    var _this = _super.call(this) || this;
    _this.fn = fn;
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.SimpleDialog.prototype.dialogResumed"></a>[function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>dialogResumed (session, result)](#apidoc.element.botbuilder.SimpleDialog.prototype.dialogResumed)
- description and source-code
```javascript
dialogResumed = function (session, result) {
    this.fn(session, result);
}
```
- example usage
```shell
...
    logger.info(this, 'session.endDialog()');
    var childId = cur.id;
    cur = this.popDialog();
    this.startBatch();
    if (cur) {
        var dialog = this.findDialog(cur.id);
        if (dialog) {
            dialog.dialogResumed(this, { resumed: Dialog_1.ResumeReason.completed, response: true, childId: childId });
        }
        else {
            this.error(new Error("Can't resume missing parent dialog '" + cur.id + "'."));
        }
    }
}
return this;
...
```

#### <a name="apidoc.element.botbuilder.SimpleDialog.prototype.replyReceived"></a>[function <span class="apidocSignatureSpan">botbuilder.SimpleDialog.prototype.</span>replyReceived (session)](#apidoc.element.botbuilder.SimpleDialog.prototype.replyReceived)
- description and source-code
```javascript
replyReceived = function (session) {
    this.fn(session);
}
```
- example usage
```shell
...
};
Session.prototype.routeToActiveDialog = function (recognizeResult) {
    var dialogStack = this.dialogStack();
    if (Session.validateDialogStack(dialogStack, this.library)) {
        var active = Session.activeDialogStackEntry(dialogStack);
        if (active) {
            var dialog = this.findDialog(active.id);
            dialog.replyReceived(this, recognizeResult);
        }
        else {
            this.beginDialog(this.options.dialogId, this.options.dialogArgs);
        }
    }
    else {
        this.error(new Error('Invalid Dialog Stack.'));
...
```



# <a name="apidoc.module.botbuilder.SimplePromptRecognizer"></a>[module botbuilder.SimplePromptRecognizer](#apidoc.module.botbuilder.SimplePromptRecognizer)

#### <a name="apidoc.element.botbuilder.SimplePromptRecognizer.SimplePromptRecognizer"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>SimplePromptRecognizer ()](#apidoc.element.botbuilder.SimplePromptRecognizer.SimplePromptRecognizer)
- description and source-code
```javascript
function SimplePromptRecognizer() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.SimplePromptRecognizer.prototype"></a>[module botbuilder.SimplePromptRecognizer.prototype](#apidoc.module.botbuilder.SimplePromptRecognizer.prototype)

#### <a name="apidoc.element.botbuilder.SimplePromptRecognizer.prototype.recognize"></a>[function <span class="apidocSignatureSpan">botbuilder.SimplePromptRecognizer.prototype.</span>recognize (args, callback, session)](#apidoc.element.botbuilder.SimplePromptRecognizer.prototype.recognize)
- description and source-code
```javascript
recognize = function (args, callback, session) {
    function findChoice(args, text) {
        var best = EntityRecognizer_1.EntityRecognizer.findBestMatch(args.enumValues, text);
        if (!best) {
            var n = EntityRecognizer_1.EntityRecognizer.parseNumber(text);
            if (!isNaN(n) && n > 0 && n <= args.enumValues.length) {
                best = { index: n - 1, entity: args.enumValues[n - 1], score: 1.0 };
            }
        }
        return best;
    }
    var score = 0.0;
    var response;
    var text = args.utterance.trim();
    switch (args.promptType) {
        default:
        case PromptType.text:
            score = 0.5;
            response = text;
            break;
        case PromptType.number:
            var n = EntityRecognizer_1.EntityRecognizer.parseNumber(text);
            if (!isNaN(n)) {
                var score = n.toString().length / text.length;
                response = n;
            }
            break;
        case PromptType.confirm:
            var b = EntityRecognizer_1.EntityRecognizer.parseBoolean(text);
            if (typeof b !== 'boolean') {
                var best = findChoice(args, text);
                if (best) {
                    b = (best.index === 0);
                }
            }
            if (typeof b == 'boolean') {
                score = 1.0;
                response = b;
            }
            break;
        case PromptType.time:
            var entity = EntityRecognizer_1.EntityRecognizer.recognizeTime(text, args.refDate ? new Date(args.refDate) : null);
            if (entity) {
                score = entity.entity.length / text.length;
                response = entity;
            }
            break;
        case PromptType.choice:
            var best = findChoice(args, text);
            if (best) {
                score = best.score;
                response = best;
            }
            break;
        case PromptType.attachment:
            if (args.attachments && args.attachments.length > 0) {
                score = 1.0;
                response = args.attachments;
            }
            break;
    }
    if (score > 0) {
        callback({ score: score, resumed: Dialog_1.ResumeReason.completed, promptType: args.promptType, response: response });
    }
    else {
        callback({ score: score, resumed: Dialog_1.ResumeReason.notCompleted, promptType: args.promptType });
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.TextBot"></a>[module botbuilder.TextBot](#apidoc.module.botbuilder.TextBot)

#### <a name="apidoc.element.botbuilder.TextBot.TextBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>TextBot (options)](#apidoc.element.botbuilder.TextBot.TextBot)
- description and source-code
```javascript
function TextBot(options) {
    if (options === void 0) { options = {}; }
    console.warn('TextBot class is deprecated. Use UniversalBot with a ConsoleConnector class.');
    var oBot = {};
    for (var key in options) {
        switch (key) {
            case 'defaultDialogId':
                oBot.defaultDialogId = options.defaultDialogId;
                break;
            case 'defaultDialogArgs':
                oBot.defaultDialogArgs = options.defaultDialogArgs;
                break;
            case 'groupWelcomeMessage':
                this.groupWelcomeMessage = options.groupWelcomeMessage;
                break;
            case 'userWelcomeMessage':
                this.userWelcomeMessage = options.userWelcomeMessage;
                break;
            case 'goodbyeMessage':
                this.goodbyeMessage = options.goodbyeMessage;
                break;
            case 'userStore':
            case 'sessionStore':
                console.error('TextBot custom stores no longer supported. Use UniversalBot with a custom IBotStorage implementation
 instead.');
                throw new Error('TextBot custom stores no longer supported.');
        }
    }
    this.connector = new ConsoleConnector_1.ConsoleConnector();
    this.bot = new UniversalBot_1.UniversalBot(this.connector, oBot);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.TextBot.prototype"></a>[module botbuilder.TextBot.prototype](#apidoc.module.botbuilder.TextBot.prototype)

#### <a name="apidoc.element.botbuilder.TextBot.prototype.add"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>add (id, dialog)](#apidoc.element.botbuilder.TextBot.prototype.add)
- description and source-code
```javascript
add = function (id, dialog) {
    this.bot.dialog(id, dialog);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.TextBot.prototype.beginDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>beginDialog (address, dialogId, dialogArgs)](#apidoc.element.botbuilder.TextBot.prototype.beginDialog)
- description and source-code
```javascript
beginDialog = function (address, dialogId, dialogArgs) {
    console.error("TextBot.beginDialog() is no longer supported. The schema for sending proactive messages has changed and you should
 update your code to use the new UniversalBot class.");
    throw new Error("TextBot.beginDialog() is no longer supported.");
}
```
- example usage
```shell
...
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
...
```

#### <a name="apidoc.element.botbuilder.TextBot.prototype.configure"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>configure (options)](#apidoc.element.botbuilder.TextBot.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
    console.error("TextBot.configure() is no longer supported. You should either pass all options into the constructor or update
 code to use the new UniversalBot class.");
    throw new Error("TextBot.configure() is no longer supported.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.TextBot.prototype.listenStdin"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>listenStdin ()](#apidoc.element.botbuilder.TextBot.prototype.listenStdin)
- description and source-code
```javascript
listenStdin = function () {
    return this.connector.listen();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.TextBot.prototype.on"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>on (event, listener)](#apidoc.element.botbuilder.TextBot.prototype.on)
- description and source-code
```javascript
on = function (event, listener) {
    this.bot.on(event, listener);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.TextBot.prototype.processMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.TextBot.prototype.</span>processMessage (message, callback)](#apidoc.element.botbuilder.TextBot.prototype.processMessage)
- description and source-code
```javascript
processMessage = function (message, callback) {
    console.error("TextBot.processMessage() is no longer supported. The schema for messages has changed and you should update your
 code to use the new UniversalBot class.");
    throw new Error("TextBot.processMessage() is no longer supported.");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ThumbnailCard"></a>[module botbuilder.ThumbnailCard](#apidoc.module.botbuilder.ThumbnailCard)

#### <a name="apidoc.element.botbuilder.ThumbnailCard.ThumbnailCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>ThumbnailCard (session)](#apidoc.element.botbuilder.ThumbnailCard.ThumbnailCard)
- description and source-code
```javascript
function ThumbnailCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.thumbnail';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.ThumbnailCard.prototype"></a>[module botbuilder.ThumbnailCard.prototype](#apidoc.module.botbuilder.ThumbnailCard.prototype)

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.ThumbnailCard.prototype.constructor)
- description and source-code
```javascript
function ThumbnailCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.thumbnail';
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.images"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>images (list)](#apidoc.element.botbuilder.ThumbnailCard.prototype.images)
- description and source-code
```javascript
images = function (list) {
    this.data.content.images = [];
    if (list) {
        for (var i = 0; i < list.length; i++) {
            var image = list[i];
            this.data.content.images.push(image.toImage ? image.toImage() : image);
        }
    }
    return this;
}
```
- example usage
```shell
...
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
...
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.subtitle"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>subtitle (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.subtitle)
- description and source-code
```javascript
subtitle = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.subtitle = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.tap"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>tap (action)](#apidoc.element.botbuilder.ThumbnailCard.prototype.tap)
- description and source-code
```javascript
tap = function (action) {
    if (action) {
        this.data.content.tap = action.toAction ? action.toAction() : action;
    }
    return this;
}
```
- example usage
```shell
...
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
if (v2.actions) {
    var list = [];
    for (var i = 0; i < v2.actions.length; i++) {
        var old = v2.actions[i];
        var btn = old.message ?
            CardAction_1.CardAction.imBack(null, old.message, old.title) :
...
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.text"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>text (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.text)
- description and source-code
```javascript
text = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.text = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
console.warn('Using old attachment schema. Upgrade to new card schema.');
var v2 = a;
var card = new HeroCard_1.HeroCard();
if (v2.title) {
    card.title(v2.title);
}
if (v2.text) {
    card.text(v2.text);
}
if (v2.thumbnailUrl) {
    card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
}
if (v2.titleLink) {
    card.tap(CardAction_1.CardAction.openUrl(null, v2.titleLink));
}
...
```

#### <a name="apidoc.element.botbuilder.ThumbnailCard.prototype.title"></a>[function <span class="apidocSignatureSpan">botbuilder.ThumbnailCard.prototype.</span>title (text)](#apidoc.element.botbuilder.ThumbnailCard.prototype.title)
- description and source-code
```javascript
title = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.title = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
...
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
    }
    if (v2.thumbnailUrl) {
        card.images([new CardImage_1.CardImage().url(v2.thumbnailUrl)]);
    }
...
```



# <a name="apidoc.module.botbuilder.UniversalBot"></a>[module botbuilder.UniversalBot](#apidoc.module.botbuilder.UniversalBot)

#### <a name="apidoc.element.botbuilder.UniversalBot.UniversalBot"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>UniversalBot (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot.UniversalBot)
- description and source-code
```javascript
function UniversalBot(connector, defaultDialog, libraryName) {
    var _this = _super.call(this, libraryName || consts.Library.default) || this;
    _this.settings = {
        processLimit: 4,
        persistUserData: true,
        persistConversationData: false
    };
    _this.connectors = {};
    _this.mwReceive = [];
    _this.mwSend = [];
    _this.mwSession = [];
    _this.localePath('./locale/');
    _this.library(Library_1.systemLib);
    if (defaultDialog) {
        if (typeof defaultDialog === 'function' || Array.isArray(defaultDialog)) {
            _this.dialog('/', defaultDialog);
        }
        else {
            var settings = defaultDialog;
            for (var name in settings) {
                if (settings.hasOwnProperty(name)) {
                    _this.set(name, settings[name]);
                }
            }
        }
    }
    if (connector) {
        _this.connector(consts.defaultConnector, connector);
    }
    return _this;
}
```
- example usage
```shell
...
var builder = require('botbuilder');

// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
...
```

#### <a name="apidoc.element.botbuilder.UniversalBot.EventEmitter"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>EventEmitter ()](#apidoc.element.botbuilder.UniversalBot.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.addRouteResult"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>addRouteResult (route, current)](#apidoc.element.botbuilder.UniversalBot.addRouteResult)
- description and source-code
```javascript
addRouteResult = function (route, current) {
    if (!current || current.length < 1 || route.score > current[0].score) {
        current = [route];
    }
    else if (route.score == current[0].score) {
        current.push(route);
    }
    return current;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.bestRouteResult"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>bestRouteResult (routes, dialogStack, rootLibraryName)](#apidoc.element.botbuilder.UniversalBot.bestRouteResult)
- description and source-code
```javascript
bestRouteResult = function (routes, dialogStack, rootLibraryName) {
    var bestLibrary = rootLibraryName;
    if (dialogStack) {
        dialogStack.forEach(function (entry) {
            var parts = entry.id.split(':');
            for (var i = 0; i < routes.length; i++) {
                if (routes[i].libraryName == parts[0]) {
                    bestLibrary = parts[0];
                    break;
                }
            }
        });
    }
    var best;
    var bestPriority = 5;
    for (var i = 0; i < routes.length; i++) {
        var r = routes[i];
        if (r.score > 0.0) {
            var priority;
            switch (r.routeType) {
                default:
                    priority = 1;
                    break;
                case Library.RouteTypes.ActiveDialog:
                    priority = 2;
                    break;
                case Library.RouteTypes.StackAction:
                    priority = 3;
                    break;
                case Library.RouteTypes.GlobalAction:
                    priority = 4;
                    break;
            }
            if (priority < bestPriority) {
                best = r;
                bestPriority = priority;
            }
            else if (priority == bestPriority) {
                switch (priority) {
                    case 3:
                        if (r.routeData.dialogIndex > best.routeData.dialogIndex) {
                            best = r;
                        }
                        break;
                    case 4:
                        if (bestLibrary && best.libraryName !== bestLibrary && r.libraryName == bestLibrary) {
                            best = r;
                        }
                        break;
                }
            }
        }
    }
    return best;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.init"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>init ()](#apidoc.element.botbuilder.UniversalBot.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.listenerCount"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.</span>listenerCount (emitter, type)](#apidoc.element.botbuilder.UniversalBot.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.UniversalBot.prototype"></a>[module botbuilder.UniversalBot.prototype](#apidoc.module.botbuilder.UniversalBot.prototype)

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.beginDialog"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>beginDialog (address, dialogId, dialogArgs, done)](#apidoc.element.botbuilder.UniversalBot.prototype.beginDialog)
- description and source-code
```javascript
beginDialog = function (address, dialogId, dialogArgs, done) {
    var _this = this;
    this.lookupUser(address, function (user) {
        var msg = {
            type: consts.messageType,
            agent: consts.agent,
            source: address.channelId,
            sourceEvent: {},
            address: utils.clone(address),
            text: '',
            user: user
        };
        _this.ensureConversation(msg.address, function (adr) {
            msg.address = adr;
            var conversationId = msg.address.conversation ? msg.address.conversation.id : null;
            var storageCtx = {
                userId: msg.user.id,
                conversationId: conversationId,
                address: msg.address,
                persistUserData: _this.settings.persistUserData,
                persistConversationData: _this.settings.persistConversationData
            };
            _this.dispatch(storageCtx, msg, dialogId, dialogArgs, _this.errorLogger(done), true);
        }, _this.errorLogger(done));
    }, this.errorLogger(done));
}
```
- example usage
```shell
...
    this.sendBatch();
    return this;
};
Session.prototype.messageSent = function () {
    return this.msgSent;
};
Session.prototype.beginDialog = function (id, args) {
    logger.info(this, 'session.beginDialog(%s)', id);
    var id = this.resolveDialogId(id);
    var dialog = this.findDialog(id);
    if (!dialog) {
        throw new Error('Dialog[' + id + '] not found.');
    }
    this.pushDialog({ id: id, state: {} });
    this.startBatch();
...
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.clone"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>clone (copyTo, newName)](#apidoc.element.botbuilder.UniversalBot.prototype.clone)
- description and source-code
```javascript
clone = function (copyTo, newName) {
    var obj = copyTo || new UniversalBot(null, null, newName || this.name);
    for (var name in this.settings) {
        if (this.settings.hasOwnProperty(name)) {
            this.set(name, this.settings[name]);
        }
    }
    for (var channel in this.connectors) {
        obj.connector(channel, this.connectors[channel]);
    }
    obj.mwReceive = this.mwReceive.slice(0);
    obj.mwSession = this.mwSession.slice(0);
    obj.mwSend = this.mwSend.slice(0);
    return _super.prototype.clone.call(this, obj);
}
```
- example usage
```shell
...
        else if (map.hasOwnProperty('*')) {
            this.data.sourceEvent = map['*'];
        }
    }
    return this;
};
Message.prototype.toMessage = function () {
    return utils.clone(this.data);
};
Message.prototype.upgradeAttachment = function (a) {
    var isOldSchema = false;
    for (var prop in a) {
        switch (prop) {
            case 'actions':
            case 'fallbackText':
...
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.connector"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>connector (channelId, connector)](#apidoc.element.botbuilder.UniversalBot.prototype.connector)
- description and source-code
```javascript
connector = function (channelId, connector) {
    var _this = this;
    var c;
    if (connector) {
        this.connectors[channelId || consts.defaultConnector] = c = connector;
        c.onEvent(function (events, cb) { return _this.receive(events, cb); });
        var asStorage = connector;
        if (!this.settings.storage &&
            typeof asStorage.getData === 'function' &&
            typeof asStorage.saveData === 'function') {
            this.settings.storage = asStorage;
        }
    }
    else if (this.connectors.hasOwnProperty(channelId)) {
        c = this.connectors[channelId];
    }
    else if (this.connectors.hasOwnProperty(consts.defaultConnector)) {
        c = this.connectors[consts.defaultConnector];
    }
    return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>constructor (connector, defaultDialog, libraryName)](#apidoc.element.botbuilder.UniversalBot.prototype.constructor)
- description and source-code
```javascript
function UniversalBot(connector, defaultDialog, libraryName) {
    var _this = _super.call(this, libraryName || consts.Library.default) || this;
    _this.settings = {
        processLimit: 4,
        persistUserData: true,
        persistConversationData: false
    };
    _this.connectors = {};
    _this.mwReceive = [];
    _this.mwSend = [];
    _this.mwSession = [];
    _this.localePath('./locale/');
    _this.library(Library_1.systemLib);
    if (defaultDialog) {
        if (typeof defaultDialog === 'function' || Array.isArray(defaultDialog)) {
            _this.dialog('/', defaultDialog);
        }
        else {
            var settings = defaultDialog;
            for (var name in settings) {
                if (settings.hasOwnProperty(name)) {
                    _this.set(name, settings[name]);
                }
            }
        }
    }
    if (connector) {
        _this.connector(consts.defaultConnector, connector);
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.createSession"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>createSession (storageCtx, message, dialogId, dialogArgs, done, newStack)](#apidoc.element.botbuilder.UniversalBot.prototype.createSession)
- description and source-code
```javascript
createSession = function (storageCtx, message, dialogId, dialogArgs, done, newStack) {
    var _this = this;
    if (newStack === void 0) { newStack = false; }
    var loadedData;
    this.getStorageData(storageCtx, function (data) {
        if (!_this.localizer) {
            var defaultLocale = _this.settings.localizerSettings ? _this.settings.localizerSettings.defaultLocale : null;
            _this.localizer = new DefaultLocalizer_1.DefaultLocalizer(_this, defaultLocale);
        }
        var session = new Session_1.Session({
            localizer: _this.localizer,
            autoBatchDelay: _this.settings.autoBatchDelay,
            library: _this,
            middleware: _this.mwSession,
            dialogId: dialogId,
            dialogArgs: dialogArgs,
            dialogErrorMessage: _this.settings.dialogErrorMessage,
            onSave: function (cb) {
                var finish = _this.errorLogger(cb);
                loadedData.userData = utils.clone(session.userData);
                loadedData.conversationData = utils.clone(session.conversationData);
                loadedData.privateConversationData = utils.clone(session.privateConversationData);
                loadedData.privateConversationData[consts.Data.SessionState] = session.sessionState;
                _this.saveStorageData(storageCtx, loadedData, finish, finish);
            },
            onSend: function (messages, cb) {
                _this.send(messages, cb);
            }
        });
        session.on('error', function (err) { return _this.emitError(err); });
        var sessionState;
        session.userData = data.userData || {};
        session.conversationData = data.conversationData || {};
        session.privateConversationData = data.privateConversationData || {};
        if (session.privateConversationData.hasOwnProperty(consts.Data.SessionState)) {
            sessionState = newStack ? null : session.privateConversationData[consts.Data.SessionState];
            delete session.privateConversationData[consts.Data.SessionState];
        }
        loadedData = data;
        session.dispatch(sessionState, message, function () { return done(null, session); });
    }, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>dispatch (storageCtx, message, dialogId, dialogArgs, done, newStack)](#apidoc.element.botbuilder.UniversalBot.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (storageCtx, message, dialogId, dialogArgs, done, newStack) {
    var _this = this;
    if (newStack === void 0) { newStack = false; }
    this.createSession(storageCtx, message, dialogId, dialogArgs, function (err, session) {
        if (!err) {
            _this.emit('routing', session);
            _this.routeMessage(session, done);
        }
        else {
            done(err);
        }
    }, newStack);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.emitError"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>emitError (err)](#apidoc.element.botbuilder.UniversalBot.prototype.emitError)
- description and source-code
```javascript
emitError = function (err) {
    var m = err.toString();
    var e = err instanceof Error ? err : new Error(m);
    if (this.listenerCount('error') > 0) {
        this.emit('error', e);
    }
    else {
        console.error(e.stack);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.ensureConversation"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>ensureConversation (address, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.ensureConversation)
- description and source-code
```javascript
ensureConversation = function (address, done, error) {
    var _this = this;
    this.tryCatch(function () {
        if (!address.conversation) {
            var connector = _this.connector(address.channelId);
            if (!connector) {
                throw new Error("Invalid channelId='" + address.channelId + "'");
            }
            connector.startConversation(address, function (err, adr) {
                if (!err) {
                    _this.tryCatch(function () { return done(adr); }, error);
                }
                else if (error) {
                    error(err);
                }
            });
        }
        else {
            _this.tryCatch(function () { return done(address); }, error);
        }
    }, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.errorLogger"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>errorLogger (done)](#apidoc.element.botbuilder.UniversalBot.prototype.errorLogger)
- description and source-code
```javascript
errorLogger = function (done) {
    var _this = this;
    return function (err) {
        if (err) {
            _this.emitError(err);
        }
        if (done) {
            done(err);
            done = null;
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.eventMiddleware"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>eventMiddleware (event, middleware, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.eventMiddleware)
- description and source-code
```javascript
eventMiddleware = function (event, middleware, done, error) {
    var i = -1;
    var _that = this;
    function next() {
        if (++i < middleware.length) {
            _that.tryCatch(function () {
                middleware[i](event, next);
            }, function () { return next(); });
        }
        else {
            _that.tryCatch(function () { return done(); }, error);
        }
    }
    next();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.get"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>get (name)](#apidoc.element.botbuilder.UniversalBot.prototype.get)
- description and source-code
```javascript
get = function (name) {
    return this.settings[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.getStorage"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>getStorage ()](#apidoc.element.botbuilder.UniversalBot.prototype.getStorage)
- description and source-code
```javascript
getStorage = function () {
    if (!this.settings.storage) {
        this.settings.storage = new BotStorage_1.MemoryBotStorage();
    }
    return this.settings.storage;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.getStorageData"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>getStorageData (storageCtx, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.getStorageData)
- description and source-code
```javascript
getStorageData = function (storageCtx, done, error) {
    var _this = this;
    this.tryCatch(function () {
        _this.emit('getStorageData', storageCtx);
        var storage = _this.getStorage();
        storage.getData(storageCtx, function (err, data) {
            if (!err) {
                _this.tryCatch(function () { return done(data || {}); }, error);
            }
            else if (error) {
                error(err);
            }
        });
    }, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.isInConversation"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>isInConversation (address, cb)](#apidoc.element.botbuilder.UniversalBot.prototype.isInConversation)
- description and source-code
```javascript
isInConversation = function (address, cb) {
    var _this = this;
    this.lookupUser(address, function (user) {
        var conversationId = address.conversation ? address.conversation.id : null;
        var storageCtx = {
            userId: user.id,
            conversationId: conversationId,
            address: address,
            persistUserData: false,
            persistConversationData: false
        };
        _this.getStorageData(storageCtx, function (data) {
            var lastAccess;
            if (data && data.privateConversationData && data.privateConversationData.hasOwnProperty(consts.Data.SessionState)) {
                var ss = data.privateConversationData[consts.Data.SessionState];
                if (ss && ss.lastAccess) {
                    lastAccess = new Date(ss.lastAccess);
                }
            }
            cb(null, lastAccess);
        }, _this.errorLogger(cb));
    }, this.errorLogger(cb));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.isMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>isMessage (message)](#apidoc.element.botbuilder.UniversalBot.prototype.isMessage)
- description and source-code
```javascript
isMessage = function (message) {
    return (message && message.type && message.type.toLowerCase() == consts.messageType);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.loadSession"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>loadSession (address, done)](#apidoc.element.botbuilder.UniversalBot.prototype.loadSession)
- description and source-code
```javascript
loadSession = function (address, done) {
    var _this = this;
    this.lookupUser(address, function (user) {
        var msg = {
            type: consts.messageType,
            agent: consts.agent,
            source: address.channelId,
            sourceEvent: {},
            address: utils.clone(address),
            text: '',
            user: user
        };
        _this.ensureConversation(msg.address, function (adr) {
            msg.address = adr;
            var conversationId = msg.address.conversation ? msg.address.conversation.id : null;
            var storageCtx = {
                userId: msg.user.id,
                conversationId: conversationId,
                address: msg.address,
                persistUserData: _this.settings.persistUserData,
                persistConversationData: _this.settings.persistConversationData
            };
            _this.createSession(storageCtx, msg, _this.settings.defaultDialogId || '/', _this.settings.defaultDialogArgs, done);
        }, _this.errorLogger(done));
    }, this.errorLogger(done));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.lookupUser"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>lookupUser (address, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.lookupUser)
- description and source-code
```javascript
lookupUser = function (address, done, error) {
    var _this = this;
    this.tryCatch(function () {
        _this.emit('lookupUser', address);
        if (_this.settings.lookupUser) {
            _this.settings.lookupUser(address, function (err, user) {
                if (!err) {
                    _this.tryCatch(function () { return done(user || address.user); }, error);
                }
                else if (error) {
                    error(err);
                }
            });
        }
        else {
            _this.tryCatch(function () { return done(address.user); }, error);
        }
    }, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.onDisambiguateRoute"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>onDisambiguateRoute (handler)](#apidoc.element.botbuilder.UniversalBot.prototype.onDisambiguateRoute)
- description and source-code
```javascript
onDisambiguateRoute = function (handler) {
    this._onDisambiguateRoute = handler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.receive"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>receive (events, done)](#apidoc.element.botbuilder.UniversalBot.prototype.receive)
- description and source-code
```javascript
receive = function (events, done) {
    var _this = this;
    var list = Array.isArray(events) ? events : [events];
    async.eachLimit(list, this.settings.processLimit, function (message, cb) {
        message.agent = consts.agent;
        message.type = message.type || consts.messageType;
        _this.lookupUser(message.address, function (user) {
            if (user) {
                message.user = user;
            }
            _this.emit('receive', message);
            _this.eventMiddleware(message, _this.mwReceive, function () {
                if (_this.isMessage(message)) {
                    _this.emit('incoming', message);
                    var userId = message.user.id;
                    var conversationId = message.address.conversation ? message.address.conversation.id : null;
                    var storageCtx = {
                        userId: userId,
                        conversationId: conversationId,
                        address: message.address,
                        persistUserData: _this.settings.persistUserData,
                        persistConversationData: _this.settings.persistConversationData
                    };
                    _this.dispatch(storageCtx, message, _this.settings.defaultDialogId || '/', _this.settings.defaultDialogArgs,
cb);
                }
                else {
                    _this.emit(message.type, message);
                    cb(null);
                }
            }, cb);
        }, cb);
    }, this.errorLogger(done));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.routeMessage"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>routeMessage (session, done)](#apidoc.element.botbuilder.UniversalBot.prototype.routeMessage)
- description and source-code
```javascript
routeMessage = function (session, done) {
    var _this = this;
    var context = session.toRecognizeContext();
    this.recognize(context, function (err, topIntent) {
        if (session.message.entities) {
            session.message.entities.forEach(function (entity) {
                if (entity.type === consts.intentEntityType &&
                    entity.score > topIntent.score) {
                    topIntent = entity;
                }
            });
        }
        context.intent = topIntent;
        context.libraryName = _this.name;
        var results = Library_1.Library.addRouteResult({ score: 0.0, libraryName: _this.name });
        async.each(_this.libraryList(), function (lib, cb) {
            lib.findRoutes(context, function (err, routes) {
                if (!err && routes) {
                    routes.forEach(function (r) { return results = Library_1.Library.addRouteResult(r, results); });
                }
                cb(err);
            });
        }, function (err) {
            if (!err) {
                var disambiguateRoute = function (session, routes) {
                    var route = Library_1.Library.bestRouteResult(results, session.dialogStack(), _this.name);
                    if (route) {
                        _this.library(route.libraryName).selectRoute(session, route);
                    }
                    else {
                        session.routeToActiveDialog();
                    }
                };
                if (_this._onDisambiguateRoute) {
                    disambiguateRoute = _this._onDisambiguateRoute;
                }
                disambiguateRoute(session, results);
                done(null);
            }
            else {
                session.error(err);
                done(err);
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.saveStorageData"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>saveStorageData (storageCtx, data, done, error)](#apidoc.element.botbuilder.UniversalBot.prototype.saveStorageData)
- description and source-code
```javascript
saveStorageData = function (storageCtx, data, done, error) {
    var _this = this;
    this.tryCatch(function () {
        _this.emit('saveStorageData', storageCtx);
        var storage = _this.getStorage();
        storage.saveData(storageCtx, data, function (err) {
            if (!err) {
                if (done) {
                    _this.tryCatch(function () { return done(); }, error);
                }
            }
            else if (error) {
                error(err);
            }
        });
    }, error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.send"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>send (messages, done)](#apidoc.element.botbuilder.UniversalBot.prototype.send)
- description and source-code
```javascript
send = function (messages, done) {
    var _this = this;
    var list;
    if (Array.isArray(messages)) {
        list = messages;
    }
    else if (messages.toMessage) {
        list = [messages.toMessage()];
    }
    else {
        list = [messages];
    }
    async.eachLimit(list, this.settings.processLimit, function (message, cb) {
        _this.ensureConversation(message.address, function (adr) {
            message.address = adr;
            _this.emit('send', message);
            _this.eventMiddleware(message, _this.mwSend, function () {
                _this.emit('outgoing', message);
                cb(null);
            }, cb);
        }, cb);
    }, this.errorLogger(function (err) {
        if (!err) {
            _this.tryCatch(function () {
                var channelId = list[0].address.channelId;
                var connector = _this.connector(channelId);
                if (!connector) {
                    throw new Error("Invalid channelId='" + channelId + "'");
                }
                connector.send(list, _this.errorLogger(done));
            }, _this.errorLogger(done));
        }
        else if (done) {
            done(null);
        }
    }));
}
```
- example usage
```shell
...
// Create bot and add dialogs
var connector = new builder.ChatConnector({
    appId: "YourAppId",
    appPassword: "YourAppSecret"
});
var bot = new builder.UniversalBot(connector);
bot.dialog('/', function (session) {
    session.send('Hello World');
});

// Setup Restify Server
var server = restify.createServer();
server.post('/api/messages', connector.listen());
server.listen(process.env.port || 3978, function () {
    console.log('%s listening to %s', server.name, server.url);
...
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.set"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>set (name, value)](#apidoc.element.botbuilder.UniversalBot.prototype.set)
- description and source-code
```javascript
set = function (name, value) {
    this.settings[name] = value;
    if (value && name === 'localizerSettings') {
        var settings = value;
        if (settings.botLocalePath) {
            this.localePath(settings.botLocalePath);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.tryCatch"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>tryCatch (fn, error)](#apidoc.element.botbuilder.UniversalBot.prototype.tryCatch)
- description and source-code
```javascript
tryCatch = function (fn, error) {
    try {
        fn();
    }
    catch (e) {
        try {
            if (error) {
                error(e);
            }
        }
        catch (e2) {
            this.emitError(e2);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.UniversalBot.prototype.use"></a>[function <span class="apidocSignatureSpan">botbuilder.UniversalBot.prototype.</span>use ()](#apidoc.element.botbuilder.UniversalBot.prototype.use)
- description and source-code
```javascript
use = function () {
    var _this = this;
    var args = [];
    for (var _i = 0; _i < arguments.length; _i++) {
        args[_i] = arguments[_i];
    }
    args.forEach(function (mw) {
        var added = 0;
        if (mw.receive) {
            Array.prototype.push.apply(_this.mwReceive, Array.isArray(mw.receive) ? mw.receive : [mw.receive]);
            added++;
        }
        if (mw.send) {
            Array.prototype.push.apply(_this.mwSend, Array.isArray(mw.send) ? mw.send : [mw.send]);
            added++;
        }
        if (mw.botbuilder) {
            Array.prototype.push.apply(_this.mwSession, Array.isArray(mw.botbuilder) ? mw.botbuilder : [mw.botbuilder]);
            added++;
        }
        if (added < 1) {
            console.warn('UniversalBot.use: no compatible middleware hook found to install.');
        }
    });
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.VideoCard"></a>[module botbuilder.VideoCard](#apidoc.module.botbuilder.VideoCard)

#### <a name="apidoc.element.botbuilder.VideoCard.VideoCard"></a>[function <span class="apidocSignatureSpan">botbuilder.</span>VideoCard (session)](#apidoc.element.botbuilder.VideoCard.VideoCard)
- description and source-code
```javascript
function VideoCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.video';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.VideoCard.prototype"></a>[module botbuilder.VideoCard.prototype](#apidoc.module.botbuilder.VideoCard.prototype)

#### <a name="apidoc.element.botbuilder.VideoCard.prototype.aspect"></a>[function <span class="apidocSignatureSpan">botbuilder.VideoCard.prototype.</span>aspect (text)](#apidoc.element.botbuilder.VideoCard.prototype.aspect)
- description and source-code
```javascript
aspect = function (text) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    if (text) {
        this.data.content.aspect = Message_1.fmtText(this.session, text, args);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.VideoCard.prototype.constructor"></a>[function <span class="apidocSignatureSpan">botbuilder.VideoCard.prototype.</span>constructor (session)](#apidoc.element.botbuilder.VideoCard.prototype.constructor)
- description and source-code
```javascript
function VideoCard(session) {
    var _this = _super.call(this, session) || this;
    _this.data.contentType = 'application/vnd.microsoft.card.video';
    return _this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.botbuilder.logger"></a>[module botbuilder.logger](#apidoc.module.botbuilder.logger)

#### <a name="apidoc.element.botbuilder.logger.debug"></a>[function <span class="apidocSignatureSpan">botbuilder.logger.</span>debug (fmt)](#apidoc.element.botbuilder.logger.debug)
- description and source-code
```javascript
function debug(fmt) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    debugLog(false, fmt, args);
}
```
- example usage
```shell
...
    }
    else {
        return this._defaultLocale;
    }
};
DefaultLocalizer.prototype.load = function (locale, done) {
    var _this = this;
    logger.debug("localizer.load(%s)", locale);
    locale = locale ? locale : this._defaultLocale;
    var fbDefault = this.getFallback(this._defaultLocale);
    var fbLocale = this.getFallback(locale);
    var locales = ['en'];
    if (fbDefault !== 'en') {
        locales.push(fbDefault);
    }
...
```

#### <a name="apidoc.element.botbuilder.logger.error"></a>[function <span class="apidocSignatureSpan">botbuilder.logger.</span>error (fmt)](#apidoc.element.botbuilder.logger.error)
- description and source-code
```javascript
function error(fmt) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    var msg = args.length > 0 ? sprintf.vsprintf(fmt, args) : fmt;
    console.error('ERROR: ' + msg);
}
```
- example usage
```shell
...
    if (file.substring(file.length - 5).toLowerCase() == ".json") {
        logger.debug("localizer.load(%s) - Loading %s/%s", locale, dir, file);
        _this.parseFile(locale, dir, file)
            .then(function (count) {
            entryCount += count;
            cb();
        }, function (err) {
            logger.error("localizer.load(%s) - Error reading %s/%s: %s", locale, dir, file, err.toString());
            cb();
        });
    }
    else {
        cb();
    }
});
...
```

#### <a name="apidoc.element.botbuilder.logger.info"></a>[function <span class="apidocSignatureSpan">botbuilder.logger.</span>info (addressable, fmt)](#apidoc.element.botbuilder.logger.info)
- description and source-code
```javascript
function info(addressable, fmt) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    var channelId = Channel.getChannelId(addressable);
    if (channelId === Channel.channels.emulator || debugLoggingEnabled) {
        var prefix = getPrefix(addressable);
        var msg = args.length > 0 ? sprintf.vsprintf(fmt, args) : fmt;
        console.info(prefix + msg);
    }
}
```
- example usage
```shell
...
        else {
            next();
        }
    });
    return this;
};
Session.prototype.error = function (err) {
    logger.info(this, 'session.error()');
    if (this.options.dialogErrorMessage) {
        this.endConversation(this.options.dialogErrorMessage);
    }
    else {
        var locale = this.preferredLocale();
        this.endConversation(this.localizer.gettext(locale, 'default_error', consts.Library.system));
    }
...
```

#### <a name="apidoc.element.botbuilder.logger.trace"></a>[function <span class="apidocSignatureSpan">botbuilder.logger.</span>trace (fmt)](#apidoc.element.botbuilder.logger.trace)
- description and source-code
```javascript
function trace(fmt) {
    var args = [];
    for (var _i = 1; _i < arguments.length; _i++) {
        args[_i - 1] = arguments[_i];
    }
    debugLog(true, fmt, args);
}
```
- example usage
```shell
...
exports.trace = trace;
function debugLog(trace, fmt, args) {
if (!debugLoggingEnabled) {
    return;
}
var msg = args.length > 0 ? sprintf.vsprintf(fmt, args) : fmt;
if (trace) {
    console.trace(msg);
}
else {
    console.log(msg);
}
}
function getPrefix(addressable) {
var prefix = '';
...
```

#### <a name="apidoc.element.botbuilder.logger.warn"></a>[function <span class="apidocSignatureSpan">botbuilder.logger.</span>warn (addressable, fmt)](#apidoc.element.botbuilder.logger.warn)
- description and source-code
```javascript
function warn(addressable, fmt) {
    var args = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        args[_i - 2] = arguments[_i];
    }
    var prefix = getPrefix(addressable);
    var msg = args.length > 0 ? sprintf.vsprintf(fmt, args) : fmt;
    console.warn(prefix + 'WARN: ' + msg);
}
```
- example usage
```shell
...
        case 'text':
        case 'thumbnailUrl':
            isOldSchema = true;
            break;
    }
}
if (isOldSchema) {
    console.warn('Using old attachment schema. Upgrade to new card schema.');
    var v2 = a;
    var card = new HeroCard_1.HeroCard();
    if (v2.title) {
        card.title(v2.title);
    }
    if (v2.text) {
        card.text(v2.text);
...
```



# <a name="apidoc.module.botbuilder.utils"></a>[module botbuilder.utils](#apidoc.module.botbuilder.utils)

#### <a name="apidoc.element.botbuilder.utils.clone"></a>[function <span class="apidocSignatureSpan">botbuilder.utils.</span>clone (obj)](#apidoc.element.botbuilder.utils.clone)
- description and source-code
```javascript
function clone(obj) {
    var cpy = {};
    if (obj) {
        for (var key in obj) {
            if (obj.hasOwnProperty(key)) {
                cpy[key] = obj[key];
            }
        }
    }
    return cpy;
}
```
- example usage
```shell
...
        else if (map.hasOwnProperty('*')) {
            this.data.sourceEvent = map['*'];
        }
    }
    return this;
};
Message.prototype.toMessage = function () {
    return utils.clone(this.data);
};
Message.prototype.upgradeAttachment = function (a) {
    var isOldSchema = false;
    for (var prop in a) {
        switch (prop) {
            case 'actions':
            case 'fallbackText':
...
```

#### <a name="apidoc.element.botbuilder.utils.copyFieldsTo"></a>[function <span class="apidocSignatureSpan">botbuilder.utils.</span>copyFieldsTo (frm, to, fields)](#apidoc.element.botbuilder.utils.copyFieldsTo)
- description and source-code
```javascript
function copyFieldsTo(frm, to, fields) {
    if (frm && to) {
        fields.split('|').forEach(function (f) {
            if (frm.hasOwnProperty(f)) {
                if (typeof to[f] === 'function') {
                    to[f](frm[f]);
                }
                else {
                    to[f] = frm[f];
                }
            }
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.utils.copyTo"></a>[function <span class="apidocSignatureSpan">botbuilder.utils.</span>copyTo (frm, to)](#apidoc.element.botbuilder.utils.copyTo)
- description and source-code
```javascript
function copyTo(frm, to) {
    if (frm) {
        for (var key in frm) {
            if (frm.hasOwnProperty(key)) {
                if (typeof to[key] === 'function') {
                    to[key](frm[key]);
                }
                else {
                    to[key] = frm[key];
                }
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.utils.moveFieldsTo"></a>[function <span class="apidocSignatureSpan">botbuilder.utils.</span>moveFieldsTo (frm, to, fields)](#apidoc.element.botbuilder.utils.moveFieldsTo)
- description and source-code
```javascript
function moveFieldsTo(frm, to, fields) {
    if (frm && to) {
        for (var f in fields) {
            if (frm.hasOwnProperty(f)) {
                if (typeof to[f] === 'function') {
                    to[fields[f]](frm[f]);
                }
                else {
                    to[fields[f]] = frm[f];
                }
                delete frm[f];
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.botbuilder.utils.toDate8601"></a>[function <span class="apidocSignatureSpan">botbuilder.utils.</span>toDate8601 (date)](#apidoc.element.botbuilder.utils.toDate8601)
- description and source-code
```javascript
function toDate8601(date) {
    return sprintf.sprintf('%04d-%02d-%02d', date.getUTCFullYear(), date.getUTCMonth() + 1, date.getUTCDate());
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
