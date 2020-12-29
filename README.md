# Project Title

Final project for the Building AI course

LLLAIHL

## Summary

LLLAIHL augments the usual property site search tools with advanced techniques that allow them to find houses using less easy to categorise/subjective attributes such as having an attractive view from the property.

## Background

Despite all the online tools available finding a new home is still difficult and time consuming. If your needs are simple - you need x bedrooms in <this> location at <this> price band, existing search tools on sites like Rightmove work just fine. If however you want a property with a view, or on a plot of land over a certain size you have to manually search through all the properties yourself. This project intends to create a tool that helps buyers automate the process of finding these properties as they come to market increasing the chances of finding the home of their dreams.

## How is it used?

This solution is intended to satisfy the needs of more 'selective' house buyers who are looking to move to a new property that satisfies more than a set of basic criteria. In the first version it will simply try to categorise properties that have a 'good' view.

The user will need an account with LLLAIHL. LLLAIHL will have an interface that displays results, and (later) configuration options so users can add their own criteria. It will also provide an email address so that email alerts sent from the property site can be received.

Once they have a LLLAIHL user account the user will need to set up a property alert using a property search tool of their choosing (e.g. rightmove.co.uk). This will ensure the basic parameters are already satisfied before the more advanced search is carried out.

They will then set an alert up ensuring that any new properties that meet their criteria are sent to their LLLAIHL email address, either directly or via a rule in their own email client.

![Example of a Rightmove Property Alert](/RightMove_Property_Alert.png)
Example of a Rightmove Property Alert

When LLLAIHL receives an email it will follow the embedded links to each property, extract the location of the home from the site it is linked to and use this information to obtain an image of the property using the satellite image from a mapping service like Google maps (using a know zoom level).

LLLAIHL will analyse this image to dertmine if it classifies as a POI (Property of Interest).

The criteria LLLAIHL will use it to look for homes that match a set of homes provided in the training data. For example homes on the edges of a village or town, or homes who have sufficiently large gardens, or back onto another neighbours (large) garden would be identified as a POI.


## Data sources and AI methods

Training and testing data will need to come from Google maps with the individual properties classified as POI = 1 or 0.
It is assumed that the collection and classification of these images will be a mostly manual process although it would need to be automated for LLLAIHL.

Real data will be retrieved by finding the location of the property from the provided link which is then used to find the location on a map. An image tile would then be extracted for analysis.

I am expecting a nearest neighbour algorythm would be a potential solution as it can be used for classification tasks like the one described above.

## Challenges

The initial analysis is likely to very crude and will not take into account the elevation of the property, or height of any surrounding vegitation or buildings that may restrict any views. The algorythm will also not know what a 'good' view looks like, simply that there are likely to be no buildings blocking the view.

The locations of properties may not be accurately recorded. 

There is a chance that both properties with and without views will be incorrectly classified however it is equally likely that a human would miss these too.

## What next?

The next step would be to use other information to help determine if the property is likely to have a good view. For example determining the elevation of the property compared to its immediate surroundings.

Once this feature is working reliably other attributes could be searched for, for example proximity to a 'busy' road.

As well as the AI problem there is also an amount of automation required to search for and extract the image data to be analaysed.
 
## Acknowledgments

My own frustration in searching for homes with nice views :)
