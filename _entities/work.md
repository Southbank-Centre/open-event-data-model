---
layout: entity
title: Work
url: /schema/work/

breadcrumb: Work
collection: entities
---

An identifiable artistic work that is performed at the event or grouping of events.
  
##Attributes
    
   | Attribute name | Description                                                             | Controlled vocabulary |
   | -------------- | ----------------------------------------------------------------------- | --------------------- |
   | WorkID         | A unique identifier for the work related to the event, e.g., URI or URL |                       |
   | Name           | Name of the work                                                        |                       |
   | Type           | Type of work, e.g., song, composition, play                             |                       |
   | Description    | Description of the work                                                 |                       |                                                                                                     



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
