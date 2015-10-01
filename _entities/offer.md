---
layout: entity
title: Offer
url: /schema/offer/

breadcrumb: Offer
collection: entities
---

A specific thing that is offered in relation to the event or grouping of events. This may be include: tickets, merchandise and food/drink
   
##Attributes
    
   | Attribute name | Description                                                      | Controlled vocabulary |
   | -------------- | ---------------------------------------------------------------- | --------------------- |
   | OfferID        | A unique identifier for the offer, e.g., URI or URL              |                       |
   | Name           | Name of the offer                                                |                       |
   | Type           | Type of thing on offer, e.g., ticket, day pass, entry, book, DVD |                       |
   | Description    | Description of the offer                                         |                       |
   | Price          | The price of the offer                                           |                       |
   | Availability   | The number of things on offer                                    |                       |
   | OfferStartDate | When the offer starts                                            | SO 8601: YYYY-MM-DD   |
   | OfferEndDate   | When the offer ends                                              | SO 8601: YYYY-MM-DD   |
   | OfferStartTime | Time offer starts                                                | ISO 8601: [hh]:[mm]   |
   | OfferEndTime   | Time offer ends                                                  | ISO 8601: [hh]:[mm]   |
   | URL            | URL for the offer (ecommerce)                                    |                       |                                                                                                    



##Example

{% highlight json  %}
{
        "Grouping": 
        {
            "GroupingID": "http://www.southbankcentre.co.uk/whatson/festivals-series/david-byrnes-meltdown-2015",
            "Name": "Meltdown",
            "Description": "This festival brings legendary artists to Southbank Centre for a very special week of one-off performances.",
            "Type": "Festival",
            "Edition": "2015",
            "Image": "http://www.southbankcentre.co.uk/images/meltdown-image.jpg",
            "StartDate": "2015-08-17",
            "EndDate": "2015-08-30",
            "URL": "http://www.southbankcentre.co.uk/whatson/festivals-series/david-byrnes-meltdown-2015"
        }
}
{% endhighlight %}
