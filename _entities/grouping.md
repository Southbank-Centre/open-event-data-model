---
layout: entity
title: Grouping
url: /schema/grouping/

breadcrumb: Grouping
collection: entities
---

An organisationally-determined collection of events. The grouping can be called a number of different things (Type=). More than one grouping can be associated with an event in a hierarchical manner or independently.
   
##Attributes
    
| Attribute name | Description                                                                          | Controlled vocabulary                                                                                      |
|----------------|--------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| GroupingID     | A unique identifier for the series, e.g., URI or URL                                 |                                                                                                                 |
| Name           | Name of the grouping                                                                 |                                                                                                                 |
| Description    | Description of the grouping, if distinct from the event description                  |                                                                                                                 |
| Type           | Type of grouping, e.g., Festival, Production, Run, Season                            | This vocabulary should be open and organisation specific. A common vocabulary may emerge organically over time. |
| Edition        | Identifier for recurrent grouping. This could be a year, number or name.             |                                                                                                                 |
| Image          | Image or logo that serves as branding for series or as an icon for it                |                                                                                                                 |
| StartDate      | The start date for the grouping                                                      | ISO 8601: YYYY-MM-DD                                                                                            |
| EndDate        | The end date for the grouping                                                        | ISO 8601: YYYY-MM-DD                                                                                            |
| URL            | Persistent URL for grouping (may be the same as GroupingID if the URL is used there) |                                                                                                                 |



##JSON Example

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
