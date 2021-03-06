<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [HttpAdapter][1]
    -   [download][2]
    -   [upload][3]
    -   [update][4]

## HttpAdapter

Off-chain data adapter for HTTP(s).

Optionally accepts an `options` object that can have two attributes:

-   `uploader`: A function responsible for uploading the data.
    It should return a Promise of the resulting URL.

-   `updater`: A function responsible for updating data at
    a given URL. It should return a Promise of the resulting URL.

**Parameters**

-   `options` **{uploader: UploaderType?, updater: UpdaterType?}** 

### download

Retrieves data from a url via https.

**Parameters**

-   `url` **[string][5]** 

Returns **[Object][6]** Parsed data.

### upload

Stores data somewhere where they can be accessed via HTTP.

Only available when options.uploader was provided during
initialization.

**Parameters**

-   `data` **[Object][6]** 

Returns **[string][5]** Resulting url such as `https://example.com/data`.

### update

Modifies data somewhere where they can be accessed via HTTP.

Only available when options.updater was provided during
initialization.

**Parameters**

-   `url` **[string][5]** 
-   `data` **[Object][6]** 

Returns **[string][5]** Resulting url such as `https://example.com/data`.

[1]: #httpadapter

[2]: #download

[3]: #upload

[4]: #update

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object
