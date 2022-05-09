# Event Listing Item Clicked

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Event Listing Item Clicked",
    "listingItemClicked": {
        "listing": [
            {
                "event": {
                    "fakeProductId": "<fakeProductId>",
                    "status": "<status>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|listingItemClicked.listing[n].event.fakeProductId|string|Helper node used by AA Product String Builder to set product to location. This field gets a static value of "event".  With updates to the AA PS extension, this will soon go away.|event|event||||||
|listingItemClicked.listing[n].event.status|string|The status of an event.|Cancelled, Sold Out, Postponed, Rescheduled|||||||




