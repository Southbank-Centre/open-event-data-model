---
layout: entity
title: Event
url: /schema/event/

breadcrumb: Event
collection: entities
---

A specific activity that occurs at a place at a given time. This is the base entity of the model. Events can be grouped in any number of ways. They inherit the attributes of the grouping, unless they are specifically changed in the event attribute.
   
##Attributes
    
| Attribute name | Description                                                                                                                                | Controlled vocabulary |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- |
| EventID        | A unique identifier for the event, e.g., URI or URL                                                                                        |                       |
| Name           | Name of the event. This should be the standard, canonical name. The data client can add alternative names on their end.                    |                       |
| Description    | Description of the event. This is the base description. Versions of this for different media or contexts can be added by the data consumer |                       |
| ArtForm        | The art form of the event, e.g.,Performance, Music, Literature, Theatre, Talk                                                              | Taxonomy project      |
| Image          | An image associated with the event                                                                                                         |                       |
| Genre          | The genre of the event                                                                                                                     | Taxonomy project      |
| Keywords       | Other terms that describe or classify the event. These can be controlled or freeform as needed                                             |                       |
| StartDate      | The date the event starts                                                                                                                  | ISO 8601: YYYY-MM-DD  |
| EndDate        | The date the event ends                                                                                                                    | ISO 8601: YYYY-MM-DD  |
| StartTime      | The time the event starts                                                                                                                  | ISO 8601: [hh]:[mm]   |
| EndTime        | The time the event ends                                                                                                                    | ISO 8601: [hh]:[mm]   |
| URL            | Persistent URL for event (may be the same as EventID if the URL is used there)                                                             |                       |                                                              |  


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
