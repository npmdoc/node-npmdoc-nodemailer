# api documentation for  [nodemailer (v3.1.8)](https://nodemailer.com/)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nodemailer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nodemailer)
#### Easy as cake e-mail sending from your Node.js applications

[![NPM](https://nodei.co/npm/nodemailer.png?downloads=true)](https://www.npmjs.com/package/nodemailer)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodemailer/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nodemailer_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodemailer/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-nodemailer/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Andris Reinman"
    },
    "bugs": {
        "url": "https://github.com/nodemailer/nodemailer/issues"
    },
    "dependencies": {},
    "description": "Easy as cake e-mail sending from your Node.js applications",
    "devDependencies": {
        "bunyan": "^1.8.9",
        "chai": "^3.5.0",
        "eslint-config-nodemailer": "^1.0.0",
        "grunt": "^1.0.1",
        "grunt-cli": "^1.2.0",
        "grunt-eslint": "^19.0.0",
        "grunt-mocha-test": "^0.13.2",
        "libbase64": "^0.1.0",
        "libmime": "^3.1.0",
        "libqp": "^1.1.0",
        "mocha": "^3.2.0",
        "proxy": "^0.2.4",
        "proxy-test-server": "^1.0.0",
        "sinon": "^2.1.0",
        "smtp-server": "^2.0.3"
    },
    "directories": {},
    "dist": {
        "shasum": "febfaccb4bd273678473a309c6cb4b4a2f3c48e3",
        "tarball": "https://registry.npmjs.org/nodemailer/-/nodemailer-3.1.8.tgz"
    },
    "engines": {
        "node": ">=6.0.0"
    },
    "gitHead": "9b4f90ac6a93e154b90884ae2ddb07c091eb872e",
    "homepage": "https://nodemailer.com/",
    "keywords": [
        "Nodemailer"
    ],
    "license": "EUPL-1.1",
    "main": "lib/nodemailer.js",
    "maintainers": [
        {
            "name": "andris",
            "email": "andris@node.ee"
        }
    ],
    "name": "nodemailer",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nodemailer/nodemailer.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "3.1.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nodemailer](#apidoc.module.nodemailer)
1.  [function <span class="apidocSignatureSpan">nodemailer.</span>createTransport (transporter, defaults)](#apidoc.element.nodemailer.createTransport)
1.  [function <span class="apidocSignatureSpan">nodemailer.</span>fetch (url, options)](#apidoc.element.nodemailer.fetch)
1.  object <span class="apidocSignatureSpan">nodemailer.</span>base64
1.  object <span class="apidocSignatureSpan">nodemailer.</span>mime_funcs
1.  object <span class="apidocSignatureSpan">nodemailer.</span>qp
1.  object <span class="apidocSignatureSpan">nodemailer.</span>shared

#### [module nodemailer.base64](#apidoc.module.nodemailer.base64)
1.  [function <span class="apidocSignatureSpan">nodemailer.base64.</span>Encoder (options)](#apidoc.element.nodemailer.base64.Encoder)
1.  [function <span class="apidocSignatureSpan">nodemailer.base64.</span>encode (buffer)](#apidoc.element.nodemailer.base64.encode)
1.  [function <span class="apidocSignatureSpan">nodemailer.base64.</span>wrap (str, lineLength)](#apidoc.element.nodemailer.base64.wrap)

#### [module nodemailer.fetch](#apidoc.module.nodemailer.fetch)
1.  [function <span class="apidocSignatureSpan">nodemailer.</span>fetch (url, options)](#apidoc.element.nodemailer.fetch.fetch)
1.  [function <span class="apidocSignatureSpan">nodemailer.fetch.</span>Cookies (options)](#apidoc.element.nodemailer.fetch.Cookies)

#### [module nodemailer.mime_funcs](#apidoc.module.nodemailer.mime_funcs)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>buildHeaderParam (key, data, maxLength)](#apidoc.element.nodemailer.mime_funcs.buildHeaderParam)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>buildHeaderValue (structured)](#apidoc.element.nodemailer.mime_funcs.buildHeaderValue)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>detectExtension (mimeType)](#apidoc.element.nodemailer.mime_funcs.detectExtension)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>detectMimeType (extension)](#apidoc.element.nodemailer.mime_funcs.detectMimeType)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeURICharComponent (0)](#apidoc.element.nodemailer.mime_funcs.encodeURICharComponent)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeWord (data, mimeWordEncoding, maxLength)](#apidoc.element.nodemailer.mime_funcs.encodeWord)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeWords (value, mimeWordEncoding, maxLength)](#apidoc.element.nodemailer.mime_funcs.encodeWords)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>foldLines (str, lineLength, afterSpace)](#apidoc.element.nodemailer.mime_funcs.foldLines)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>hasLongerLines (str, lineLength)](#apidoc.element.nodemailer.mime_funcs.hasLongerLines)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>isPlainText (value)](#apidoc.element.nodemailer.mime_funcs.isPlainText)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>parseHeaderValue (str)](#apidoc.element.nodemailer.mime_funcs.parseHeaderValue)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>safeEncodeURIComponent (str)](#apidoc.element.nodemailer.mime_funcs.safeEncodeURIComponent)
1.  [function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>splitMimeEncodedString (str, maxlen)](#apidoc.element.nodemailer.mime_funcs.splitMimeEncodedString)

#### [module nodemailer.qp](#apidoc.module.nodemailer.qp)
1.  [function <span class="apidocSignatureSpan">nodemailer.qp.</span>Encoder (options)](#apidoc.element.nodemailer.qp.Encoder)
1.  [function <span class="apidocSignatureSpan">nodemailer.qp.</span>encode (buffer)](#apidoc.element.nodemailer.qp.encode)
1.  [function <span class="apidocSignatureSpan">nodemailer.qp.</span>wrap (str, lineLength)](#apidoc.element.nodemailer.qp.wrap)

#### [module nodemailer.shared](#apidoc.module.nodemailer.shared)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>_logFunc (logger, level, defaults, data, message, ...args)](#apidoc.element.nodemailer.shared._logFunc)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>assign ()](#apidoc.element.nodemailer.shared.assign)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>callbackPromise (resolve, reject)](#apidoc.element.nodemailer.shared.callbackPromise)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>encodeXText (!/[^\x21-\x2A\x2C-\x3C\x3E-\x7E]/.test(str)](#apidoc.element.nodemailer.shared.encodeXText)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>getLogger (options, defaults)](#apidoc.element.nodemailer.shared.getLogger)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>parseConnectionUrl (str, true)](#apidoc.element.nodemailer.shared.parseConnectionUrl)
1.  [function <span class="apidocSignatureSpan">nodemailer.shared.</span>resolveContent (data, key, callback)](#apidoc.element.nodemailer.shared.resolveContent)



# <a name="apidoc.module.nodemailer"></a>[module nodemailer](#apidoc.module.nodemailer)

#### <a name="apidoc.element.nodemailer.createTransport"></a>[function <span class="apidocSignatureSpan">nodemailer.</span>createTransport (transporter, defaults)](#apidoc.element.nodemailer.createTransport)
- description and source-code
```javascript
createTransport = function (transporter, defaults) {
    let urlConfig;
    let options;
    let mailer;

    if (
        // provided transporter is a configuration object, not transporter plugin
        (typeof transporter === 'object' && typeof transporter.send !== 'function') ||
        // provided transporter looks like a connection url
        (typeof transporter === 'string' && /^(smtps?|direct):/i.test(transporter))
    ) {

        if ((urlConfig = typeof transporter === 'string' ? transporter : transporter.url)) {
            // parse a configuration URL into configuration options
            options = shared.parseConnectionUrl(urlConfig);
        } else {
            options = transporter;
        }

        if (options.pool) {
            transporter = new SMTPPool(options);
        } else if (options.sendmail) {
            transporter = new SendmailTransport(options);
        } else if (options.streamTransport) {
            transporter = new StreamTransport(options);
        } else if (options.jsonTransport) {
            transporter = new JSONTransport(options);
        } else if (options.SES) {
            transporter = new SESTransport(options);
        } else {
            transporter = new SMTPTransport(options);
        }
    }

    mailer = new Mailer(transporter, options, defaults);

    return mailer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.fetch"></a>[function <span class="apidocSignatureSpan">nodemailer.</span>fetch (url, options)](#apidoc.element.nodemailer.fetch)
- description and source-code
```javascript
fetch = function (url, options) {
    return fetch(url, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodemailer.base64"></a>[module nodemailer.base64](#apidoc.module.nodemailer.base64)

#### <a name="apidoc.element.nodemailer.base64.Encoder"></a>[function <span class="apidocSignatureSpan">nodemailer.base64.</span>Encoder (options)](#apidoc.element.nodemailer.base64.Encoder)
- description and source-code
```javascript
class Encoder extends Transform {
    constructor(options) {
        super();
        // init Transform
        this.options = options || {};

        if (this.options.lineLength !== false) {
            this.options.lineLength = this.options.lineLength || 76;
        }

        this._curLine = '';
        this._remainingBytes = false;

        this.inputBytes = 0;
        this.outputBytes = 0;
    }

    _transform(chunk, encoding, done) {
        let b64;

        if (encoding !== 'buffer') {
            chunk = new Buffer(chunk, encoding);
        }

        if (!chunk || !chunk.length) {
            return done();
        }

        this.inputBytes += chunk.length;

        if (this._remainingBytes && this._remainingBytes.length) {
            chunk = Buffer.concat([this._remainingBytes, chunk]);
            this._remainingBytes = false;
        }

        if (chunk.length % 3) {
            this._remainingBytes = chunk.slice(chunk.length - chunk.length % 3);
            chunk = chunk.slice(0, chunk.length - chunk.length % 3);
        } else {
            this._remainingBytes = false;
        }

        b64 = this._curLine + encode(chunk);

        if (this.options.lineLength) {
            b64 = wrap(b64, this.options.lineLength);
            b64 = b64.replace(/(^|\n)([^\n]*)$/, (match, lineBreak, lastLine) => {
                this._curLine = lastLine;
                return lineBreak;
            });
        }

        if (b64) {
            this.outputBytes += b64.length;
            this.push(b64);
        }

        done();
    }

    _flush(done) {
        if (this._remainingBytes && this._remainingBytes.length) {
            this._curLine += encode(this._remainingBytes);
        }

        if (this._curLine) {
            this._curLine = wrap(this._curLine, this.options.lineLength);
            this.outputBytes += this._curLine.length;
            this.push(this._curLine, 'ascii');
            this._curLine = '';
        }
        done();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.base64.encode"></a>[function <span class="apidocSignatureSpan">nodemailer.base64.</span>encode (buffer)](#apidoc.element.nodemailer.base64.encode)
- description and source-code
```javascript
function encode(buffer) {
    if (typeof buffer === 'string') {
        buffer = new Buffer(buffer, 'utf-8');
    }

    return buffer.toString('base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.base64.wrap"></a>[function <span class="apidocSignatureSpan">nodemailer.base64.</span>wrap (str, lineLength)](#apidoc.element.nodemailer.base64.wrap)
- description and source-code
```javascript
function wrap(str, lineLength) {
    str = (str || '').toString();
    lineLength = lineLength || 76;

    if (str.length <= lineLength) {
        return str;
    }

    let result = [];
    let pos = 0;
    let chunkLength = lineLength * 1024;
    while (pos < str.length) {
        let wrappedLines = str.substr(pos, chunkLength).replace(new RegExp('.{' + lineLength + '}', 'g'), '$&\r\n').trim();
        result.push(wrappedLines);
        pos += chunkLength;
    }

    return result.join('\r\n').trim();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodemailer.fetch"></a>[module nodemailer.fetch](#apidoc.module.nodemailer.fetch)

#### <a name="apidoc.element.nodemailer.fetch.fetch"></a>[function <span class="apidocSignatureSpan">nodemailer.</span>fetch (url, options)](#apidoc.element.nodemailer.fetch.fetch)
- description and source-code
```javascript
fetch = function (url, options) {
    return fetch(url, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.fetch.Cookies"></a>[function <span class="apidocSignatureSpan">nodemailer.fetch.</span>Cookies (options)](#apidoc.element.nodemailer.fetch.Cookies)
- description and source-code
```javascript
class Cookies {
    constructor(options) {
        this.options = options || {};
        this.cookies = [];
    }

<span class="apidocCodeCommentSpan">    /**
     * Stores a cookie string to the cookie storage
     *
     * @param {String} cookieStr Value from the 'Set-Cookie:' header
     * @param {String} url Current URL
     */
</span>    set(cookieStr, url) {
        let urlparts = urllib.parse(url || '');
        let cookie = this.parse(cookieStr);
        let domain;

        if (cookie.domain) {
            domain = cookie.domain.replace(/^\./, '');

            // do not allow cross origin cookies
            if (
                // can't be valid if the requested domain is shorter than current hostname
                urlparts.hostname.length < domain.length ||

                // prefix domains with dot to be sure that partial matches are not used
                ('.' + urlparts.hostname).substr(-domain.length + 1) !== ('.' + domain)) {
                cookie.domain = urlparts.hostname;
            }
        } else {
            cookie.domain = urlparts.hostname;
        }

        if (!cookie.path) {
            cookie.path = this.getPath(urlparts.pathname);
        }

        // if no expire date, then use sessionTimeout value
        if (!cookie.expires) {
            cookie.expires = new Date(Date.now() + (Number(this.options.sessionTimeout || SESSION_TIMEOUT) || SESSION_TIMEOUT) *
1000);
        }

        return this.add(cookie);
    }

    /**
     * Returns cookie string for the 'Cookie:' header.
     *
     * @param {String} url URL to check for
     * @returns {String} Cookie header or empty string if no matches were found
     */
    get(url) {
        return this.list(url).map(cookie =>
            cookie.name + '=' + cookie.value).join('; ');
    }

    /**
     * Lists all valied cookie objects for the specified URL
     *
     * @param {String} url URL to check for
     * @returns {Array} An array of cookie objects
     */
    list(url) {
        let result = [];
        let i;
        let cookie;

        for (i = this.cookies.length - 1; i >= 0; i--) {
            cookie = this.cookies[i];

            if (this.isExpired(cookie)) {
                this.cookies.splice(i, i);
                continue;
            }

            if (this.match(cookie, url)) {
                result.unshift(cookie);
            }
        }

        return result;
    }

    /**
     * Parses cookie string from the 'Set-Cookie:' header
     *
     * @param {String} cookieStr String from the 'Set-Cookie:' header
     * @returns {Object} Cookie object
     */
    parse(cookieStr) {
        let cookie = {};

        (cookieStr || '').toString().split(';').forEach(cookiePart => {
            let valueParts = cookiePart.split('=');
            let key = valueParts.shift().trim().toLowerCase();
            let value = valueParts.join('=').trim();
            let domain;

            if (!key) {
                // skip empty parts
                return;
            }

            switch (key) {

                case 'expires':
                    value = new Date(value);
                    // ignore date if can not parse it
                    if (value.toString() !== 'Invalid Date') {
                        cookie.expires = value;
                    }
                    break;

                case 'path':
                    cookie.path = value;
                    break;

                case 'domain':
                    domain = value.toLowerCase();
                    if (domain.length && domain.charAt(0) !== '.') {
                        domain = '.' + domain; // ensure preceeding dot for user set domains
                    }
                    cookie.domain = domain;
                    break;

                case 'max-age':
                    cookie.expires = new Date(Date.now() + (Number(value) || 0) * 1000);
                    break;

                case 'secure':
                    cookie.secure = true;
                    break;

                case 'httponly':
                    cookie.httponly = true;
                    break; ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodemailer.mime_funcs"></a>[module nodemailer.mime_funcs](#apidoc.module.nodemailer.mime_funcs)

#### <a name="apidoc.element.nodemailer.mime_funcs.buildHeaderParam"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>buildHeaderParam (key, data, maxLength)](#apidoc.element.nodemailer.mime_funcs.buildHeaderParam)
- description and source-code
```javascript
buildHeaderParam(key, data, maxLength) {
    let list = [];
    let encodedStr = typeof data === 'string' ? data : (data || '').toString();
    let encodedStrArr;
    let chr, ord;
    let line;
    let startPos = 0;
    let i, len;

    maxLength = maxLength || 50;

    // process ascii only text
    if (this.isPlainText(data)) {

        // check if conversion is even needed
        if (encodedStr.length <= maxLength) {
            return [{
                key,
                value: encodedStr
            }];
        }

        encodedStr = encodedStr.replace(new RegExp('.{' + maxLength + '}', 'g'), str => {
            list.push({
                line: str
            });
            return '';
        });

        if (encodedStr) {
            list.push({
                line: encodedStr
            });
        }

    } else {

        if (/[\uD800-\uDBFF]/.test(encodedStr)) {
            // string containts surrogate pairs, so normalize it to an array of bytes
            encodedStrArr = [];
            for (i = 0, len = encodedStr.length; i < len; i++) {
                chr = encodedStr.charAt(i);
                ord = chr.charCodeAt(0);
                if (ord >= 0xD800 && ord <= 0xDBFF && i < len - 1) {
                    chr += encodedStr.charAt(i + 1);
                    encodedStrArr.push(chr);
                    i++;
                } else {
                    encodedStrArr.push(chr);
                }
            }
            encodedStr = encodedStrArr;
        }

        // first line includes the charset and language info and needs to be encoded
        // even if it does not contain any unicode characters
        line = 'utf-8\'\'';
        let encoded = true;
        startPos = 0;

        // process text with unicode or special chars
        for (i = 0, len = encodedStr.length; i < len; i++) {

            chr = encodedStr[i];

            if (encoded) {
                chr = this.safeEncodeURIComponent(chr);
            } else {
                // try to urlencode current char
                chr = chr === ' ' ? chr : this.safeEncodeURIComponent(chr);
                // By default it is not required to encode a line, the need
                // only appears when the string contains unicode or special chars
                // in this case we start processing the line over and encode all chars
                if (chr !== encodedStr[i]) {
                    // Check if it is even possible to add the encoded char to the line
                    // If not, there is no reason to use this line, just push it to the list
                    // and start a new line with the char that needs encoding
                    if ((this.safeEncodeURIComponent(line) + chr).length >= maxLength) {
                        list.push({
                            line,
                            encoded
                        });
                        line = '';
                        startPos = i - 1;
                    } else {
                        encoded = true;
                        i = startPos;
                        line = '';
                        continue;
                    }
                }
            }

            // if the line is already too long, push it to the list and start a new one
            if ((line + chr).length >= maxLength) {
                list.push({
                    line,
                    encoded
                });
                line = chr = encodedStr[i] === ' ' ? ' ' : this.safeEncodeURIComponent(encodedStr[i]);
                if (chr === encodedStr[i]) {
                    encoded = false;
                    startPos = i - 1;
                } else {
                    encoded = true;
                }
            } else {
                line += chr;
            }
        }

        if (line) {
            list.push({
                line,
                encoded
            });
        }
    }

    return list.map((item, i) => ({
        // encoded lines: {name}*{part}*
        // unencoded lines: {name}*{part}
        // if any line needs to be encode ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.buildHeaderValue"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>buildHeaderValue (structured)](#apidoc.element.nodemailer.mime_funcs.buildHeaderValue)
- description and source-code
```javascript
buildHeaderValue(structured) {
    let paramsArray = [];

    Object.keys(structured.params || {}).forEach(param => {
        // filename might include unicode characters so it is a special case
        // other values probably do not
        let value = structured.params[param];
        if (!this.isPlainText(value) || value.length >= 75) {
            this.buildHeaderParam(param, value, 50).forEach(encodedParam => {
                if (!/[\s"\\;:\/=\(\),<>@\[\]\?]|^[\-']|'$/.test(encodedParam.value) || encodedParam.key.substr(-1) === '*') {
                    paramsArray.push(encodedParam.key + '=' + encodedParam.value);
                } else {
                    paramsArray.push(encodedParam.key + '=' + JSON.stringify(encodedParam.value));
                }
            });
        } else if (/[\s'"\\;:\/=\(\),<>@\[\]\?]|^\-/.test(value)) {
            paramsArray.push(param + '=' + JSON.stringify(value));
        } else {
            paramsArray.push(param + '=' + value);
        }
    });

    return structured.value + (paramsArray.length ? '; ' + paramsArray.join('; ') : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.detectExtension"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>detectExtension (mimeType)](#apidoc.element.nodemailer.mime_funcs.detectExtension)
- description and source-code
```javascript
mimeType => mimeTypes.detectExtension(mimeType)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.detectMimeType"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>detectMimeType (extension)](#apidoc.element.nodemailer.mime_funcs.detectMimeType)
- description and source-code
```javascript
extension => mimeTypes.detectMimeType(extension)
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.encodeURICharComponent"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeURICharComponent (0)](#apidoc.element.nodemailer.mime_funcs.encodeURICharComponent)
- description and source-code
```javascript
chr => {
    let res = '';
    let ord = chr.charCodeAt(0).toString(16).toUpperCase();

    if (ord.length % 2) {
        ord = '0' + ord;
    }

    if (ord.length > 2) {
        for (let i = 0, len = ord.length / 2; i < len; i++) {
            res += '%' + ord.substr(i, 2);
        }
    } else {
        res += '%' + ord;
    }

    return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.encodeWord"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeWord (data, mimeWordEncoding, maxLength)](#apidoc.element.nodemailer.mime_funcs.encodeWord)
- description and source-code
```javascript
encodeWord(data, mimeWordEncoding, maxLength) {
    mimeWordEncoding = (mimeWordEncoding || 'Q').toString().toUpperCase().trim().charAt(0);
    maxLength = maxLength || 0;

    let encodedStr;
    let toCharset = 'UTF-8';

    if (maxLength && maxLength > 7 + toCharset.length) {
        maxLength -= (7 + toCharset.length);
    }

    if (mimeWordEncoding === 'Q') {
        // https://tools.ietf.org/html/rfc2047#section-5 rule (3)
        encodedStr = qp.encode(data).replace(/[^a-z0-9!*+\-\/=]/ig, chr => {
            let ord = chr.charCodeAt(0).toString(16).toUpperCase();
            if (chr === ' ') {
                return '_';
            } else {
                return '=' + (ord.length === 1 ? '0' + ord : ord);
            }
        });
    } else if (mimeWordEncoding === 'B') {
        encodedStr = typeof data === 'string' ? data : base64.encode(data);
        maxLength = maxLength ? Math.max(3, (maxLength - maxLength % 4) / 4 * 3) : 0;
    }

    if (maxLength && (mimeWordEncoding !== 'B' ? encodedStr : base64.encode(data)).length > maxLength) {
        if (mimeWordEncoding === 'Q') {
            encodedStr = this.splitMimeEncodedString(encodedStr, maxLength).join('?= =?' + toCharset + '?' + mimeWordEncoding + '?');
        } else {
            // RFC2047 6.3 (2) states that encoded-word must include an integral number of characters, so no chopping unicode sequences
            let parts = [];
            let lpart = '';
            for (let i = 0, len = encodedStr.length; i < len; i++) {
                let chr = encodedStr.charAt(i);
                // check if we can add this character to the existing string
                // without breaking byte length limit
                if (Buffer.byteLength(lpart + chr) <= maxLength || i === 0) {
                    lpart += chr;
                } else {
                    // we hit the length limit, so push the existing string and start over
                    parts.push(base64.encode(lpart));
                    lpart = chr;
                }
            }
            if (lpart) {
                parts.push(base64.encode(lpart));
            }

            if (parts.length > 1) {
                encodedStr = parts.join('?= =?' + toCharset + '?' + mimeWordEncoding + '?');
            } else {
                encodedStr = parts.join('');
            }
        }
    } else if (mimeWordEncoding === 'B') {
        encodedStr = base64.encode(data);
    }

    return '=?' + toCharset + '?' + mimeWordEncoding + '?' + encodedStr + (encodedStr.substr(-2) === '?=' ? '' : '?=');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.encodeWords"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>encodeWords (value, mimeWordEncoding, maxLength)](#apidoc.element.nodemailer.mime_funcs.encodeWords)
- description and source-code
```javascript
encodeWords(value, mimeWordEncoding, maxLength) {
    maxLength = maxLength || 0;

    let encodedValue;

    // find first word with a non-printable ascii in it
    let firstMatch = value.match(/(?:^|\s)([^\s]*[\u0080-\uFFFF])/);
    if (!firstMatch) {
        return value;
    }

    // find the last word with a non-printable ascii in it
    let lastMatch = value.match(/([\u0080-\uFFFF][^\s]*)[^\u0080-\uFFFF]*$/);
    if (!lastMatch) {
        // should not happen
        return value;
    }

    let startIndex = firstMatch.index + (firstMatch[0].match(/[^\s]/) || {
        index: 0
    }).index;
    let endIndex = lastMatch.index + (lastMatch[1] || '').length;

    encodedValue =
        (startIndex ? value.substr(0, startIndex) : '') + this.encodeWord(value.substring(startIndex, endIndex), mimeWordEncoding
 || 'Q', maxLength) +
        (endIndex < value.length ? value.substr(endIndex) : '');

    return encodedValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.foldLines"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>foldLines (str, lineLength, afterSpace)](#apidoc.element.nodemailer.mime_funcs.foldLines)
- description and source-code
```javascript
foldLines(str, lineLength, afterSpace) {
    str = (str || '').toString();
    lineLength = lineLength || 76;

    let pos = 0,
        len = str.length,
        result = '',
        line, match;

    while (pos < len) {
        line = str.substr(pos, lineLength);
        if (line.length < lineLength) {
            result += line;
            break;
        }
        if ((match = line.match(/^[^\n\r]*(\r?\n|\r)/))) {
            line = match[0];
            result += line;
            pos += line.length;
            continue;
        } else if ((match = line.match(/(\s+)[^\s]*$/)) && match[0].length - (afterSpace ? (match[1] || '').length : 0) < line.length
) {
            line = line.substr(0, line.length - (match[0].length - (afterSpace ? (match[1] || '').length : 0)));
        } else if ((match = str.substr(pos + line.length).match(/^[^\s]+(\s*)/))) {
            line = line + match[0].substr(0, match[0].length - (!afterSpace ? (match[1] || '').length : 0));
        }

        result += line;
        pos += line.length;
        if (pos < len) {
            result += '\r\n';
        }
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.hasLongerLines"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>hasLongerLines (str, lineLength)](#apidoc.element.nodemailer.mime_funcs.hasLongerLines)
- description and source-code
```javascript
hasLongerLines(str, lineLength) {
    if (str.length > 128 * 1024) {
        // do not test strings longer than 128kB
        return true;
    }
    return new RegExp('^.{' + (lineLength + 1) + ',}', 'm').test(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.isPlainText"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>isPlainText (value)](#apidoc.element.nodemailer.mime_funcs.isPlainText)
- description and source-code
```javascript
isPlainText(value) {
    if (typeof value !== 'string' || /[\x00-\x08\x0b\x0c\x0e-\x1f\u0080-\uFFFF]/.test(value)) {
        return false;
    } else {
        return true;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.parseHeaderValue"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>parseHeaderValue (str)](#apidoc.element.nodemailer.mime_funcs.parseHeaderValue)
- description and source-code
```javascript
parseHeaderValue(str) {
    let response = {
        value: false,
        params: {}
    };
    let key = false;
    let value = '';
    let type = 'value';
    let quote = false;
    let escaped = false;
    let chr;

    for (let i = 0, len = str.length; i < len; i++) {
        chr = str.charAt(i);
        if (type === 'key') {
            if (chr === '=') {
                key = value.trim().toLowerCase();
                type = 'value';
                value = '';
                continue;
            }
            value += chr;
        } else {
            if (escaped) {
                value += chr;
            } else if (chr === '\\') {
                escaped = true;
                continue;
            } else if (quote && chr === quote) {
                quote = false;
            } else if (!quote && chr === '"') {
                quote = chr;
            } else if (!quote && chr === ';') {
                if (key === false) {
                    response.value = value.trim();
                } else {
                    response.params[key] = value.trim();
                }
                type = 'key';
                value = '';
            } else {
                value += chr;
            }
            escaped = false;

        }
    }

    if (type === 'value') {
        if (key === false) {
            response.value = value.trim();
        } else {
            response.params[key] = value.trim();
        }
    } else if (value.trim()) {
        response.params[value.trim().toLowerCase()] = '';
    }

    // handle parameter value continuations
    // https://tools.ietf.org/html/rfc2231#section-3

    // preprocess values
    Object.keys(response.params).forEach(key => {
        let actualKey, nr, match, value;
        if ((match = key.match(/(\*(\d+)|\*(\d+)\*|\*)$/))) {
            actualKey = key.substr(0, match.index);
            nr = Number(match[2] || match[3]) || 0;

            if (!response.params[actualKey] || typeof response.params[actualKey] !== 'object') {
                response.params[actualKey] = {
                    charset: false,
                    values: []
                };
            }

            value = response.params[key];

            if (nr === 0 && match[0].substr(-1) === '*' && (match = value.match(/^([^']*)'[^']*'(.*)$/))) {
                response.params[actualKey].charset = match[1] || 'iso-8859-1';
                value = match[2];
            }

            response.params[actualKey].values[nr] = value;

            // remove the old reference
            delete response.params[key];
        }
    });

    // concatenate split rfc2231 strings and convert encoded strings to mime encoded words
    Object.keys(response.params).forEach(key => {
        let value;
        if (response.params[key] && Array.isArray(response.params[key].values)) {
            value = response.params[key].values.map(val => val || '').join('');

            if (response.params[key].charset) {
                // convert "%AB" to "=?charset?Q?=AB?="
                response.params[key] = '=?' +
                    response.params[key].charset +
                    '?Q?' +
                    value.
                // fix invalidly encoded chars
                replace(/[=\?_\s]/g,
                    s => {
                        let c = s.charCodeAt(0).toString(16);
                        if (s === ' ') {
                            return '_';
                        } else {
                            return '%' + (c.length < 2 ? '0' : '') + c;
                        }
                    }
                ).
                // change from urlencoding to percent encoding
                replace(/%/g, '=') +
                    '?=';
            } else {
                response.params[key] = value;
            }
        }
    });

    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.safeEncodeURIComponent"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>safeEncodeURIComponent (str)](#apidoc.element.nodemailer.mime_funcs.safeEncodeURIComponent)
- description and source-code
```javascript
safeEncodeURIComponent(str) {
    str = (str || '').toString();

    try {
        // might throw if we try to encode invalid sequences, eg. partial emoji
        str = encodeURIComponent(str);
    } catch (E) {
        // should never run
        return str.replace(/[^\x00-\x1F *'()<>@,;:\\"\[\]?=\u007F-\uFFFF]+/g, '');
    }

    // ensure chars that are not handled by encodeURICompent are converted as well
    return str.replace(/[\x00-\x1F *'()<>@,;:\\"\[\]?=\u007F-\uFFFF]/g, chr => this.encodeURICharComponent(chr));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.mime_funcs.splitMimeEncodedString"></a>[function <span class="apidocSignatureSpan">nodemailer.mime_funcs.</span>splitMimeEncodedString (str, maxlen)](#apidoc.element.nodemailer.mime_funcs.splitMimeEncodedString)
- description and source-code
```javascript
(str, maxlen) => {
    let curLine, match, chr, done,
        lines = [];

    // require at least 12 symbols to fit possible 4 octet UTF-8 sequences
    maxlen = Math.max(maxlen || 0, 12);

    while (str.length) {
        curLine = str.substr(0, maxlen);

        // move incomplete escaped char back to main
        if ((match = curLine.match(/\=[0-9A-F]?$/i))) {
            curLine = curLine.substr(0, match.index);
        }

        done = false;
        while (!done) {
            done = true;
            // check if not middle of a unicode char sequence
            if ((match = str.substr(curLine.length).match(/^\=([0-9A-F]{2})/i))) {
                chr = parseInt(match[1], 16);
                // invalid sequence, move one char back anc recheck
                if (chr < 0xC2 && chr > 0x7F) {
                    curLine = curLine.substr(0, curLine.length - 3);
                    done = false;
                }
            }
        }

        if (curLine.length) {
            lines.push(curLine);
        }
        str = str.substr(curLine.length);
    }

    return lines;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodemailer.qp"></a>[module nodemailer.qp](#apidoc.module.nodemailer.qp)

#### <a name="apidoc.element.nodemailer.qp.Encoder"></a>[function <span class="apidocSignatureSpan">nodemailer.qp.</span>Encoder (options)](#apidoc.element.nodemailer.qp.Encoder)
- description and source-code
```javascript
class Encoder extends Transform {
    constructor(options) {
        super();

        // init Transform
        this.options = options || {};

        if (this.options.lineLength !== false) {
            this.options.lineLength = this.options.lineLength || 76;
        }

        this._curLine = '';

        this.inputBytes = 0;
        this.outputBytes = 0;
    }

    _transform(chunk, encoding, done) {
        let qp;

        if (encoding !== 'buffer') {
            chunk = new Buffer(chunk, encoding);
        }

        if (!chunk || !chunk.length) {
            return done();
        }

        this.inputBytes += chunk.length;

        if (this.options.lineLength) {
            qp = this._curLine + encode(chunk);
            qp = wrap(qp, this.options.lineLength);
            qp = qp.replace(/(^|\n)([^\n]*)$/, (match, lineBreak, lastLine) => {
                this._curLine = lastLine;
                return lineBreak;
            });

            if (qp) {
                this.outputBytes += qp.length;
                this.push(qp);
            }

        } else {
            qp = encode(chunk);
            this.outputBytes += qp.length;
            this.push(qp, 'ascii');
        }

        done();
    }

    _flush(done) {
        if (this._curLine) {
            this.outputBytes += this._curLine.length;
            this.push(this._curLine, 'ascii');
        }
        done();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.qp.encode"></a>[function <span class="apidocSignatureSpan">nodemailer.qp.</span>encode (buffer)](#apidoc.element.nodemailer.qp.encode)
- description and source-code
```javascript
function encode(buffer) {
    if (typeof buffer === 'string') {
        buffer = new Buffer(buffer, 'utf-8');
    }

    // usable characters that do not need encoding
    let ranges = [
        // https://tools.ietf.org/html/rfc2045#section-6.7
        [0x09], // <TAB>
        [0x0A], // <LF>
        [0x0D], // <CR>
        [0x20, 0x3C], // <SP>!"#$%&'()*+,-./0123456789:;
        [0x3E, 0x7E] // >?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_'abcdefghijklmnopqrstuvwxyz{|}
    ];
    let result = '';
    let ord;

    for (let i = 0, len = buffer.length; i < len; i++) {
        ord = buffer[i];
        // if the char is in allowed range, then keep as is, unless it is a WS in the end of a line
        if (checkRanges(ord, ranges) && !((ord === 0x20 || ord === 0x09) && (i === len - 1 || buffer[i + 1] === 0x0a || buffer[i
 + 1] === 0x0d))) {
            result += String.fromCharCode(ord);
            continue;
        }
        result += '=' + (ord < 0x10 ? '0' : '') + ord.toString(16).toUpperCase();
    }

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.qp.wrap"></a>[function <span class="apidocSignatureSpan">nodemailer.qp.</span>wrap (str, lineLength)](#apidoc.element.nodemailer.qp.wrap)
- description and source-code
```javascript
function wrap(str, lineLength) {
    str = (str || '').toString();
    lineLength = lineLength || 76;

    if (str.length <= lineLength) {
        return str;
    }

    let pos = 0;
    let len = str.length;
    let match, code, line;
    let lineMargin = Math.floor(lineLength / 3);
    let result = '';

    // insert soft linebreaks where needed
    while (pos < len) {
        line = str.substr(pos, lineLength);
        if ((match = line.match(/\r\n/))) {
            line = line.substr(0, match.index + match[0].length);
            result += line;
            pos += line.length;
            continue;
        }

        if (line.substr(-1) === '\n') {
            // nothing to change here
            result += line;
            pos += line.length;
            continue;
        } else if ((match = line.substr(-lineMargin).match(/\n.*?$/))) {
            // truncate to nearest line break
            line = line.substr(0, line.length - (match[0].length - 1));
            result += line;
            pos += line.length;
            continue;
        } else if (line.length > lineLength - lineMargin && (match = line.substr(-lineMargin).match(/[ \t\.,!\?][^ \t\.,!\?]*$/))) {
            // truncate to nearest space
            line = line.substr(0, line.length - (match[0].length - 1));
        } else if (line.match(/\=[\da-f]{0,2}$/i)) {

            // push incomplete encoding sequences to the next line
            if ((match = line.match(/\=[\da-f]{0,1}$/i))) {
                line = line.substr(0, line.length - match[0].length);
            }

            // ensure that utf-8 sequences are not split
            while (line.length > 3 && line.length < len - pos && !line.match(/^(?:=[\da-f]{2}){1,4}$/i) && (match = line.match(/\=[\da-f]{2}$/ig))) {
                code = parseInt(match[0].substr(1, 2), 16);
                if (code < 128) {
                    break;
                }

                line = line.substr(0, line.length - 3);

                if (code >= 0xC0) {
                    break;
                }
            }
        }

        if (pos + line.length < len && line.substr(-1) !== '\n') {
            if (line.length === lineLength && line.match(/\=[\da-f]{2}$/i)) {
                line = line.substr(0, line.length - 3);
            } else if (line.length === lineLength) {
                line = line.substr(0, line.length - 1);
            }
            pos += line.length;
            line += '=\r\n';
        } else {
            pos += line.length;
        }

        result += line;
    }

    return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodemailer.shared"></a>[module nodemailer.shared](#apidoc.module.nodemailer.shared)

#### <a name="apidoc.element.nodemailer.shared._logFunc"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>_logFunc (logger, level, defaults, data, message, ...args)](#apidoc.element.nodemailer.shared._logFunc)
- description and source-code
```javascript
(logger, level, defaults, data, message, ...args) => {
    let entry = {};

    Object.keys(defaults || {}).forEach(key => {
        if (key !== 'level') {
            entry[key] = defaults[key];
        }
    });

    Object.keys(data || {}).forEach(key => {
        if (key !== 'level') {
            entry[key] = data[key];
        }
    });

    logger[level](entry, message, ...args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.assign"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>assign ()](#apidoc.element.nodemailer.shared.assign)
- description and source-code
```javascript
assign = function () {
    let args = Array.from(arguments);
    let target = args.shift() || {};

    args.forEach(source => {
        Object.keys(source || {}).forEach(key => {
            if (['tls', 'auth'].includes(key) && source[key] && typeof source[key] === 'object') {
                // tls and auth are special keys that need to be enumerated separately
                // other objects are passed as is
                if (!target[key]) {
                    // ensure that target has this key
                    target[key] = {};
                }
                Object.keys(source[key]).forEach(subKey => {
                    target[key][subKey] = source[key][subKey];
                });
            } else {
                target[key] = source[key];
            }
        });
    });
    return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.callbackPromise"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>callbackPromise (resolve, reject)](#apidoc.element.nodemailer.shared.callbackPromise)
- description and source-code
```javascript
(resolve, reject) => function () {
    let args = Array.from(arguments);
    let err = args.shift();
    if (err) {
        reject(err);
    } else {
        resolve(...args);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.encodeXText"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>encodeXText (!/[^\x21-\x2A\x2C-\x3C\x3E-\x7E]/.test(str)](#apidoc.element.nodemailer.shared.encodeXText)
- description and source-code
```javascript
str => {
    // ! 0x21
    // + 0x2B
    // = 0x3D
    // ~ 0x7E
    if (!/[^\x21-\x2A\x2C-\x3C\x3E-\x7E]/.test(str)) {
        return str;
    }
    let buf = Buffer.from(str);
    let result = '';
    for (let i = 0, len = buf.length; i < len; i++) {
        let c = buf[i];
        if (c < 0x21 || c > 0x7e || c === 0x2b || c === 0x3d) {
            result += '+' + (c < 0x10 ? '0' : '') + c.toString(16).toUpperCase();
        } else {
            result += String.fromCharCode(c);
        }
    }
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.getLogger"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>getLogger (options, defaults)](#apidoc.element.nodemailer.shared.getLogger)
- description and source-code
```javascript
(options, defaults) => {
    options = options || {};

    let response = {};
    let levels = ['trace', 'debug', 'info', 'warn', 'error', 'fatal'];

    if (!options.logger) {
        // use vanity logger
        levels.forEach(level => {
            response[level] = () => false;
        });
        return response;
    }

    let logger = options.logger;

    if (options.logger === true) {
        // create console logger
        logger = createDefaultLogger(levels);
    }

    levels.forEach(level => {
        response[level] = (data, message, ...args) => {
            module.exports._logFunc(logger, level, defaults, data, message, ...args);
        };
    });

    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.parseConnectionUrl"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>parseConnectionUrl (str, true)](#apidoc.element.nodemailer.shared.parseConnectionUrl)
- description and source-code
```javascript
str => {
    str = str || '';
    let options = {};

    [urllib.parse(str, true)].forEach(url => {
        let auth;

        switch (url.protocol) {
            case 'smtp:':
                options.secure = false;
                break;
            case 'smtps:':
                options.secure = true;
                break;
            case 'direct:':
                options.direct = true;
                break;
        }

        if (!isNaN(url.port) && Number(url.port)) {
            options.port = Number(url.port);
        }

        if (url.hostname) {
            options.host = url.hostname;
        }

        if (url.auth) {
            auth = url.auth.split(':');

            if (!options.auth) {
                options.auth = {};
            }

            options.auth.user = auth.shift();
            options.auth.pass = auth.join(':');
        }

        Object.keys(url.query || {}).forEach(key => {
            let obj = options;
            let lKey = key;
            let value = url.query[key];

            if (!isNaN(value)) {
                value = Number(value);
            }

            switch (value) {
                case 'true':
                    value = true;
                    break;
                case 'false':
                    value = false;
                    break;
            }

            // tls is nested object
            if (key.indexOf('tls.') === 0) {
                lKey = key.substr(4);
                if (!options.tls) {
                    options.tls = {};
                }
                obj = options.tls;
            } else if (key.indexOf('.') >= 0) {
                // ignore nested properties besides tls
                return;
            }

            if (!(lKey in obj)) {
                obj[lKey] = value;
            }
        });
    });

    return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodemailer.shared.resolveContent"></a>[function <span class="apidocSignatureSpan">nodemailer.shared.</span>resolveContent (data, key, callback)](#apidoc.element.nodemailer.shared.resolveContent)
- description and source-code
```javascript
(data, key, callback) => {
    let promise;

    if (!callback && typeof Promise === 'function') {
        promise = new Promise((resolve, reject) => {
            callback = module.exports.callbackPromise(resolve, reject);
        });
    }

    let content = data && data[key] && data[key].content || data[key];
    let contentStream;
    let encoding = (typeof data[key] === 'object' && data[key].encoding || 'utf8')
        .toString()
        .toLowerCase()
        .replace(/[-_\s]/g, '');

    if (!content) {
        return callback(null, content);
    }

    if (typeof content === 'object') {
        if (typeof content.pipe === 'function') {
            return resolveStream(content, (err, value) => {
                if (err) {
                    return callback(err);
                }
                // we can't stream twice the same content, so we need
                // to replace the stream object with the streaming result
                data[key] = value;
                callback(null, value);
            });
        } else if (/^https?:\/\//i.test(content.path || content.href)) {
            contentStream = fetch(content.path || content.href);
            return resolveStream(contentStream, callback);
        } else if (/^data:/i.test(content.path || content.href)) {
            let parts = (content.path || content.href).match(/^data:((?:[^;]*;)*(?:[^,]*)),(.*)$/i);
            if (!parts) {
                return callback(null, new Buffer(0));
            }
            return callback(null, /\bbase64$/i.test(parts[1]) ? new Buffer(parts[2], 'base64') : new Buffer(decodeURIComponent(parts
[2])));
        } else if (content.path) {
            return resolveStream(fs.createReadStream(content.path), callback);
        }
    }

    if (typeof data[key].content === 'string' && !['utf8', 'usascii', 'ascii'].includes(encoding)) {
        content = new Buffer(data[key].content, encoding);
    }

    // default action, return as is
    setImmediate(() => callback(null, content));

    return promise;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
