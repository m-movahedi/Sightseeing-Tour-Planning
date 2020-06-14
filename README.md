# sighseeing_tour_planning
A python tool for planning sightseeing tours in a small urban area.This code is available under Attribution-NonCommercial-ShareAlike 4.0 International license.

<img src="https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png">

*This project was funded by Tehran Municipality to promote tourism in the 11th district.*
## Introduction
Tourism plays an important role in the growth of urban economics. Attractions like historical buildings that gasp the essence of the life, streets with the hallmarks of the past, and monuments that act as mementos can be lucrative for local businesses and fruitful for the culture of the city.

 
The path to an efficient plan for sightseeing tours requires both demand evaluation and route planning. In this post, only the route planning stage of such will be discussed.
In most of the sightseeing tours, there are two active transportation modes working alongside each other, a major mode which usually provides users with a lift to especial stations and a minor mode that connect these stations to the desired attractions.

## Major Mode

The major mode usually follows certain criteria which can later be interpreted into a cost function. some of which can be named as:

    The distance of attractions from each other. (in meters)
    The duration of travel among attractions. (in seconds)
    The exposure of users into appropriate economic land use. (in either meters or seconds)
    The exposure of users into historical or leisure inducive land use. (in either meters or seconds)
    Economical impact (usually in carbon dioxide equivalent)

The easiest way to embed such an idea is to calculate a matrix with arrays Rij presenting the cost of the cheapest route when the agent travels from the origin i to the destination j. The problem of finding such routes calls for a different post. In this case, we assume we have an algorithm that returns this route. It is obvious that the Rij would not be equal to the Rji as the cheapest route may be different. 

 <figure align=center>
  <img src="https://i2.wp.com/m-movahedi.ml/wp-content/uploads/2020/01/b32e3dc3cf8b9471bc17992160820128.jpg" alt="Trulli" style="width:100%">
  <figcaption>Hassan Abad square, Tehran, Iran.</figcaption>
</figure> 
        
## Minor Mode

In this project, the minor mode refers to the walking routes planned in part of the study area which might induce tourism or any related activity. These areas usually pass through either cultural or historical reached streets. the criteria for these routes are quite different from normal walking streets especially when it comes to the desired walking distance and duration since the visitors are willing to interact with what they come upon.

## Route

In this case, the problem of routing is not the problem of finding the way but to find an optimal sequential which visits all the stations with the lowest cost. The problem is a well-known graph routing problem as known as the traveling salesman problem.
