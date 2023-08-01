# 1. Search tracks
Base url: https://free-mp3-download.net/search.php?s={query}

#### Request params
| URL Parameter | Description  |
| ------------- | ------------ |
| query         | Search query |

### Sample request
Request URL: https://free-mp3-download.net/search.php?s=dvrst
Response: 
<details> 
  <summary>JSON Response </summary>
  
  ``` json
 {
  "data": [
    {
      "id": 1413655312,
      "readable": true,
      "title": "Close Eyes",
      "title_short": "Close Eyes",
      "title_version": "",
      "link": "https:\\/\\/www.deezer.com\\/track\\/1413655312",
      "duration": 132,
      "rank": 800372,
      "explicit_lyrics": true,
      "explicit_content_lyrics": 1,
      "explicit_content_cover": 2,
      "preview": "https:\\/\\/cdns-preview-c.dzcdn.net\\/stream\\/c-cb3ceb59e926c5270fc7be69fe1822ea-3.mp3",
      "md5_image": "927d033421b24eb3ba981d8551cdcbde",
      "artist": {
        "id": 88333752,
        "name": "DVRST",
        "link": "https:\\/\\/www.deezer.com\\/artist\\/88333752",
        "picture": "https:\\/\\/api.deezer.com\\/artist\\/88333752\\/image",
        "picture_small": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/artist\\/ab88269cc6a389ac11afa6ac935e6c53\\/56x56-000000-80-0-0.jpg",
        "picture_medium": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/artist\\/ab88269cc6a389ac11afa6ac935e6c53\\/250x250-000000-80-0-0.jpg",
        "picture_big": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/artist\\/ab88269cc6a389ac11afa6ac935e6c53\\/500x500-000000-80-0-0.jpg",
        "picture_xl": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/artist\\/ab88269cc6a389ac11afa6ac935e6c53\\/1000x1000-000000-80-0-0.jpg",
        "tracklist": "https:\\/\\/api.deezer.com\\/artist\\/88333752\\/top?limit=50",
        "type": "artist"
      },
      "album": {
        "id": 239513192,
        "title": "Close Eyes",
        "cover": "https:\\/\\/api.deezer.com\\/album\\/239513192\\/image",
        "cover_small": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/cover\\/927d033421b24eb3ba981d8551cdcbde\\/56x56-000000-80-0-0.jpg",
        "cover_medium": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/cover\\/927d033421b24eb3ba981d8551cdcbde\\/250x250-000000-80-0-0.jpg",
        "cover_big": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/cover\\/927d033421b24eb3ba981d8551cdcbde\\/500x500-000000-80-0-0.jpg",
        "cover_xl": "https:\\/\\/e-cdns-images.dzcdn.net\\/images\\/cover\\/927d033421b24eb3ba981d8551cdcbde\\/1000x1000-000000-80-0-0.jpg",
        "md5_image": "927d033421b24eb3ba981d8551cdcbde",
        "tracklist": "https:\\/\\/api.deezer.com\\/album\\/239513192\\/tracks",
        "type": "album"
      },
      "type": "track"
    },
```

</details>
