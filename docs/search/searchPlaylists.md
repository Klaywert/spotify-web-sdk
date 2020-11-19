---
id: searchPlaylists
title: searchPlaylists
---

Use this function to get the informations about playlists in Spotify's catalog that matches a search query keyword.

## Parameters

Parameters | Type   | Obligatoriness | Value
-----------|--------|----------------|-------
query      | string | Required       | Query keyword of the search
market     | string | Optional       | A code that identifies a country
limit      | number | Optional       | A field that represents the maximum number of results that will be returned
offset     | number | Optional       | The index of the first result to be returned

## Return

This function returns a Page of PlaylistSimplified objects (`Page<PlaylistSimplified>`) that matches the query keyword. You can get the informations about each one of the playlists returned in the query.

## Use Example

```javascript
import * as spotify from 'spotify-web-sdk';
spotify.searchPlaylists('hits');
```