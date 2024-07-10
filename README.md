# Resource Generator

This is an marker pack for Azgaar's _Fantasy Map Generator_

Link to original project: [azgaar.github.io/Fantasy-Map-Generator](https://azgaar.github.io/Fantasy-Map-Generator).

I have created a set of markers that represent resources on the map. For me to write a good state conflict story economy and resources are key behind motivation and making it believable so here it is:
![Screenshot_1](https://github.com/Azgaar/Fantasy-Map-Generator/assets/174297022/f3f55045-ea8f-4af1-87a6-4306b2fb0d95)
10k
190
![Screenshot_2](https://github.com/Azgaar/Fantasy-Map-Generator/assets/174297022/19bdb00a-6285-41fc-8428-bc6102042374)
50k
530
![Screenshot_3](https://github.com/Azgaar/Fantasy-Map-Generator/assets/174297022/af269528-f267-4181-a0ca-e81bac96bced)
100k
860

Below every screenshot there is points number followed by the amount of markers.

Most markers are generated taking into account cells temperature, precipitation, biome, ect. so the placement of markers, for me is pretty reflective of reality.
 
 To install, you'd have to open generator on your local host (I personally use OSpanel) then download the second zip file from the top (Fantasy-Map-Generator-master.zip), unzip it, put inside projects folder and start up your local host server and that's it. Create new map or open saved one, after doing so, go ahead and hide markers layer and show it again for size to be updated
 
 This is very raw version, so no editor inside client, and when manipulating multiplier in client bugs out the generator, not sure how to fix it yet.
 If you would like to change/add a resource open marker generator, in` GetDefaultConfig` function add your resource, then create new List[resource] function for generation configuration and Add[resource] function for description. If you would like to change the frequency of resource generation, find your resource in  `GetDefaultConfig`, and manipulate 'each' variable. the less the value the more resources will be generated
 to adjust marker size and shape, go to layers.js, `GetPin`, choose your marker shape, below that you can find `DrawMarker` and adjust its size
 
 In future I plan to:
 1. Make generation more precise 
 2. Add each states resources counter 
 3. Add state resources needs 
 4. Resources filter for visual cleanse 
 5. Resource editor in client
