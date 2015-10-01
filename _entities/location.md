---
layout: entity
title: Location
url: /schema/location/

breadcrumb: Location
collection: entities
---

A physical location where the event or grouping of events occurs.
   
##Attributes
    
   | Attribute name | Description                                                                 | Controlled vocabulary |
   | -------------- | --------------------------------------------------------------------------- | --------------------- |
   | LocationID     | A unique identifier for the event location, e.g., URI or URL                |                       |
   | Name           | Name of the place where the event occurs                                    |                       |
   | Type           | Type of place where the event occurs, e.g., Theatre, Gallery, Outdoors      |                       |
   | Address        | Address of the event location, including city, region and country if needed |                       |
   | Geocode        | The geocode coordinates of the location, for mapping                        |                       |                                                                                                       
                                                                                                            



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
