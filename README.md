# Project Title

Final project for the Building AI course

LLLAIHL (pronounced Layla) stands for Location, Location, Location AI Home Locator

## Summary

LLLAIHL is an AI powered tool that helps home buyers find the property of their dreams by augmenting the ususal property site search tools with advanced techniques that allow them to find houses using less easy to categorise (or perhaps even more subjective) attributes such as having an attractive view from the property. 

## Background

Despite all the online tools available finding a new home is still difficult and time consuming. If your needs are simple - you need x bedrooms in <this> location at <this> price band, existing search tools on sites like Rightmove work just fine. If however you want a property with a view, or on a plot of land over a certain size you have to manually search through all the properties yourself. This project intends to create a tool that helps buyers automate the process of finding these properties as they come to market increasing the chances of finding the home of their dreams.

## How is it used?

This solution is indended to satisfy the needs of more 'selective' house buyers who are looking to move to a new property that satisfies more than a set of basic criteria.

The user will need an account with LLLAIHL. LLLAIHL will have an interface that displays results, and (later) configuration options so users can add their own criteria. It will also provide an email address so that email alerts sent from the property site can be received.

Once they have a LLLAIHL user account the user will need to set up a property alert using a property search tool of their choosing (e.g. rightmove.co.uk). This will ensure the basic parameters are already satisfied before the more advanced search is carried out.

They will then set an alert up ensuring that any new properties that meet their criteria are sent to their LLLAIHL email address.

![Example of a Rightmove Property Alert](/RightMove_Property_Alert.png)
Example of a Rightmove Property Alert

When LLLAIHL receives an emial alert it will follow the embedded links to each property, extract the location of the home from the site it is linked to and use this information to obtain an image of the property using the satellite image from a mapping service like Google maps (using a know zoom level).

LLLAIHL will analyse this image to dertmine if it classifies as an POI (Property of Interest).

The criteria LLLAIHL will use it to simply look for homes that have no other properties boardering at least one side of the property. For example homes on the edges of a village or town, or homes who have sufficiently large gardens, or back onto another neighbours (large) garden.


## Data sources and AI methods



Where does your data come from? Do you collect it yourself or do you use data collected by someone else?
If you need to use links, here's an example:
[Twitter API](https://developer.twitter.com/en/docs)

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

## Challenges

What does your project _not_ solve? Which limitations and ethical considerations should be taken into account when deploying a solution like this?

## What next?

How could your project grow and become something even more? What kind of skills, what kind of assistance would you  need to move on? 


## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc
