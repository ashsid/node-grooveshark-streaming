# node-grooveshark-streaming

A node.js module for getting a music streaming url from Grooveshark without any API authentication.

[![Build Status](https://travis-ci.org/xissy/node-grooveshark-streaming.png?branch=master)](https://travis-ci.org/xissy/node-grooveshark-streaming)

## Features

- Searches grooveshark song info by a track title and an artist name.
- Gets grooveshark streaming url by a song id from grooveshark song info.

## Installation

Via [npm](https://npmjs.org):

```
  $ npm install grooveshark-streaming
```
  

## Quick Start

### Load in the module

```
  var GS = require('grooveshark-streaming');
```

### Exported Objects

- Tinysong
- Grooveshark

### Searching a grooveshark song info and getting its streaming url

```javascript
  GS.Tinysong.getSongInfo('Love of My Life', 'Queen', function(err, songInfo) {
    ...
    GS.Grooveshark.getStreamingUrl(songInfo.SongID, function(err, streamUrl) {
      ...
    });
  });
```

## License

Released under the MIT License

Copyright (c) 2013 Taeho Kim <xissysnd@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
