# WebSocket - Pascal and C# implementations #

Project contains implementation of clients and servers using WebSocket protocol.



**SECOND VERSION OF BAUGLIR WEBSOCKET - [HyBi 7-17](http://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-07) AND [RFC](http://tools.ietf.org/html/rfc6455) WEBSOCKET SPECIFICATION**

**Current version: 2.0.4 (2012-01-30)** [#Changelog](#Changelog.md)

For Hixi versions of specification (75, 76) use Bauglir WebSocket 1.1.0.

_If you are using Bauglir WebSocket in production, please let me know (Bronislav.Klucka@bauglir.com)_

**If you are getting garbage from Chrome19: T problem is caused by x-deflate-frame extension in WebSocket implementation in Chrome see
http://code.google.com/p/bauglir-websocket/issues/detail?id=37#c1 to refuse it from server**

## Implementations ##
  * Pascal client and server implementation (source code documented). Support for non-secure and secure (SSL) connection.
  * C# .NET client and server implementation (source code documented). Support for non-secure and secure (SSL) connection.

**[Implementation notes](http://code.google.com/p/bauglir-websocket/wiki/programming_notes)**

<a href='Hidden comment: 
==Binaries==
Work on library in progress.

There is Wiki page with [http://code.google.com/p/bauglir-websocket/wiki/Libraries interface description]
'></a>


## Demos ##

[Check out the demos on YouTube!](http://www.youtube.com/user/BronislavKlucka#p/c/3A7E9CAAA6B4CB73) (Excuse my English...)

  * Pascal
    * Delphi client and server demos (Windows) - based directly on Pascal sources
    * Lazarus client and server demos (Linux (Kubuntu)) - based directly on Pascal sources
  * C# .NET
    * C# .NET client and server demos (Windows & Linux) - based directly on C# sources
  * HTML5 web pages for WebSocket compatible browsers (client) for testing server (e.g. Pascal demo).

<a href='Hidden comment: 
* source code and projects compiled for Windows XP and Linux (Kubuntu) - based directly on Pascal sources
* source code and projects compiled for Windows XP and Linux (Kubuntu) - based on libraries (dll, so)
* PHP server implementing request/response communication with HTML5 web page for testing
* PHP server implementing broadcasts to all connected clients with HTML5 web page for testing
'></a>





## Support ##

Supported HyBi versions: [7-17](http://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-07)

Supported RFC versions: [RFC6455](http://tools.ietf.org/html/rfc6455)

Supported browsers:
  * FireFox 11
    * Aurora 11.0a2 (2012-01-11)  supports binary data and close reason and code
  * Chrome 16 and up

Browser issues
  * Chrome
    * current stable release (16) and up should follow RFC
  * Firefox
    * does not support SSL with non-authorized keys

## Notes ##

  1. Documentation on [WebNt.eu WebSocket](http://www.webnt.eu) is in progress. See source code for documentation, it's fully documented.
  1. If you are still using 1st version, you should check [its introduction page](http://code.google.com/p/bauglir-websocket/wiki/Version001)


## Changelog ##

---

  * + = added
  * - = removed
  * @ = bugfix
  * : = changes

---


### 2012-01-30 - Version 2.0.4 ###
  * @ [Delphi XE does not work](http://code.google.com/p/bauglir-websocket/issues/detail?id=34)
  * @ [Pascal - Events are missing on very frequent traffic](http://code.google.com/p/bauglir-websocket/issues/detail?id=27)
  * @ [Pascal - Closing connection issues](http://code.google.com/p/bauglir-websocket/issues/detail?id=28)
  * : [Change default client version to 13](http://code.google.com/p/bauglir-websocket/issues/detail?id=31)
  * + [Pascal - Make CanReceiveOrSend public](http://code.google.com/p/bauglir-websocket/issues/detail?id=29)
  * + [Pascal - Make SendData public](http://code.google.com/p/bauglir-websocket/issues/detail?id=30)
  * + [Add Handshake property](http://code.google.com/p/bauglir-websocket/issues/detail?id=33)
  * + [Add CloseAllConnections method](http://code.google.com/p/bauglir-websocket/issues/detail?id=32)


### 2012-01-11 - Version 2.0.3 ###
  * + support for [The WebSocket Protocol RFC](http://tools.ietf.org/html/rfc6455)
  * : [Close codes](http://code.google.com/p/bauglir-websocket/issues/detail?id=24)
  * + [Full data processing mode (concanating fragmented messages)](http://code.google.com/p/bauglir-websocket/issues/detail?id=25)


### 2011-10-14 - Version 2.0.2 ###
  * + support for HyBi 13 up


### 2011-09-04 - Version 2.0.1 ###
Initial C# .NET version 2 with support for HyBi 10 version of WebSocket specification

  * @ [Pascal Demo - TTestWebSocketClientConnection constructor](http://code.google.com/p/bauglir-websocket/issues/detail?id=11)
  * @ [Pascal Library - improve headers manipulation](http://code.google.com/p/bauglir-websocket/issues/detail?id=12)
  * @ [Pascal Lazarus Server demo](http://code.google.com/p/bauglir-websocket/issues/detail?id=19)
  * @ [Pascal Library - Closing connection while reading](http://code.google.com/p/bauglir-websocket/issues/detail?id=20)
  * + [C# - Create WebSocket HyBi implementation for version 2](http://code.google.com/p/bauglir-websocket/issues/detail?id=13)
  * + [Pascal Library - Add extension support](http://code.google.com/p/bauglir-websocket/issues/detail?id=16)
  * + [Pascal Library - Do not check Host agins server bindings](http://code.google.com/p/bauglir-websocket/issues/detail?id=18)




### 2011-08-29 - Version 2.0.0 ###
Initial Pascal version 2 with support for HyBi 10 version of WebSocket specification

### 2011-04-24 - Version 1.1.0 ###
  * + [Enhancement Issue 4 (wss (SSL) support for pascal)](http://code.google.com/p/bauglir-websocket/issues/detail?id=4)
  * + [Enhancement Issue 5 (automatic UTF-8 conversion to desktop charset for pascal - AutoUTF8)](http://code.google.com/p/bauglir-websocket/issues/detail?id=5)
  * : [Enhancement Issue 6 (renaming BauglirInLibrary variable since it is confusing)](http://code.google.com/p/bauglir-websocket/issues/detail?id=6)
  * : [Enhancement Issue 8 (clean up duplication in code)](http://code.google.com/p/bauglir-websocket/issues/detail?id=8)
  * : library interface changed to support SSL and, AutoUTF8


### 2011-04-15 - Version 1.0.1 ###
  * + Added C# implemetation (based on WebSocket library)
  * + [Enhancement Issue 2 (libraries for Windows and Linux)](http://code.google.com/p/bauglir-websocket/issues/detail?id=2)
  * + [Enhancement Issue 1 (events)](http://code.google.com/p/bauglir-websocket/issues/detail?id=1)
  * : StoreData property is `false` after object construction

### 2011-03-29 - Initial version 1.0.0 ###

## Todo ##
Todo list can be found in Issues as accepted enhancements