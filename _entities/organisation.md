---
layout: entity
title: Organisation
url: /schema/organisation/

breadcrumb: Organisation
collection: entities
---

An identifiable person or organisation who has a role related to the event or grouping of events.
     
##Attributes
    
| Attribute name | Description                                                                                         | Controlled vocabulary |
| -------------- | --------------------------------------------------------------------------------------------------- | --------------------- |
| PersonID       | A unique identifier for the person or organisation (group), e.g., URI or URL                        |                       |
| Name           | The name of the person or organisation                                                              |                       |
| Type           | Type of person, e.g., Person, Organisation, Group                                                   |                       |
| Role           | The role the person or organisation plays in the event, e.g., performer, producer, composer, author |                       |
| Image          | A base image of the person or organisation                                                          |                       |



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
