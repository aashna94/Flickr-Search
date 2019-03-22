# Flickr-Search
A small project that uses Flickr API to search images based on the keyword.


## Pre-requisite

- Clone the repo and run Flickr-Search-Project.xcodeproj
- No 3rd party Libraries Used.
- Create a Flickr API key and replace in line number 124 **flickrKey** with your own key in Flickr.swift 

## Requirements

* Deployment target of your App is >= iOS 10.0
* XCode 9.3 or later
* Swift 4.0

## Flickr API Documentation

Images are retrieved by hitting the [Flickr API](https://www.flickr.com/services/api/flickr.photos.search.html).

- **Search Path:**

```
https://api.flickr.com/services/rest/?method=flickr.photos.search&api_key=YOUR_FLICKR_API_KEY&per_page=25&format=json&nojsoncallback=1&safe_search=1&text=KEYWORD
```
Increase the per_page count to download more photos.

- Response includes an array of photo objects, each represented as:

``` swift
{
    "id": "23451156376",
    "owner": "28017113@N08",
    "secret": "8983a8ebc7",
    "server": "578",
    "farm": 1,
    "title": "Merry Christmas!",
    "ispublic": 1,
    "isfriend": 0,
    "isfamily": 0
}
```

