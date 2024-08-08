# Sightseeing Tour Planning
A python tool for planning sightseeing tours in a small urban area.This code is available under Attribution-NonCommercial-ShareAlike 4.0 International license.

*This project was funded by Tehran Municipality to promote tourism in the 11th district.*
## Introduction
Tourism plays an important role in the growth of urban economics. Attractions like historical buildings that capture the essence of life, streets with the hallmarks of the past, and monuments that act as mementos can be lucrative for local businesses and fruitful for the city's culture.

 
The path to an efficient sightseeing tour plan requires both demand evaluation and route planning. This post will discuss only the route planning stage.
In most sightseeing tours, there are two active transportation modes working alongside each other: a major mode that usually provides users with a lift to special stations and a minor mode that connects these stations to the desired attractions.

## Major Mode

The major mode usually follows certain criteria which can later be interpreted into a cost function. some of which can be named as:

    1. The distance of attractions from each other. (in meters)
    2. The duration of travel among attractions. (in seconds)
    3. The exposure of users to appropriate economic land use. (in either meters or seconds)
    4. The exposure of users to historical or leisure inducive land use. (in either meters or seconds)
    5. Economical impact (usually in carbon dioxide equivalent)

The easiest way to embed such an idea is to calculate a matrix with arrays Rij presenting the cost of the cheapest route when the agent travels from the origin i to the destination j. The problem of finding such routes calls for a different post. In this case, we assume we have an algorithm that returns this route. It is obvious that the Rij would not be equal to the Rji as the cheapest route may differ. 

 <figure align=center>
  <img src="https://i2.wp.com/m-movahedi.ml/wp-content/uploads/2020/01/b32e3dc3cf8b9471bc17992160820128.jpg" alt="Trulli" style="width:100%">
  <figcaption>Hassan Abad square, Tehran, Iran.</figcaption>
</figure> 
        
## Minor Mode

In this project, the minor mode refers to the walking routes planned in part of the study area that might induce tourism or any related activity. These areas usually pass through either cultural or historical streets. The criteria for these routes are quite different from normal walking streets, especially when it comes to the desired walking distance and duration since the visitors are willing to interact with what they come upon.

## Route

In this case, the routing problem is not finding a way but finding an optimal sequential that visits all the stations with the lowest cost. The problem is a well-known graph routing problem, also known as the traveling salesman problem.


 Sighseeing Tour Planner by Mohammad Movahedi is licensed under CC BY-NC-SA 4.0 CC
 
 <img src="https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png">
