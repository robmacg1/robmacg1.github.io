# Programming for Geographic Information Analysis: Portfolio

### About Me
> I am a masters student of Geographic Information Systems at the University of Leeds. I became aware of GIS during my undergraduate in Wildlife Ecology and Conservation Science. Graduating in the midst of a global pandemic was less than ideal but it gave me time to reflect on what I am interested in and where I would like to take my career. To create solutions and make educated decisions to mitigate the environmental, social and political uncertainty we face ahead, understanding systemic structures and how they organise across space has never been more important. On a more personal level, I can find a lot of satisfaction in seeing for myself how patterns can be discerned when spatial data is visualised through the convention of mapping.

### Agent Based Model
> For this assignment I have modeled sheep on a hillside as they are harassed by a sheep dog.
> 
> #### The model can be accessed from [this github repository](https://github.com/robmacg1/model1) and all the information to run it can be found in the readme there.
>
> **The sheep will:**
> 1. **Eat their environment**
> - As the sheep graze the grid of integer values that is used to create a raster image of the hillside from the top down is modified as the pixel values change.
> - The sheep become visually larger as they feed until they reach a fullness threshold and defecate, becoming smaller again.
> 2. **Flock together**
> - The sheep modify their behaviour depending on whether other sheep are nearby, becoming less likely to move and to move shorter distances.
> 3. **Share with each other**
> - These sheep are able to somehow share their stores of food with each other when nearby if they are fuller than those nearby
> 4. **Die**
> - After a few bowel movements the sheep no longer function
> - If their fullness drops to zero they die!
> 5. **Run from the sheep dog/wolf**
> - When the sheep dog gets too close the sheep drop what they are doing and run in the opposite direction.
> - The sheep dog will take bites out of their stores when it gets close and if their fullness drops to zero they die!
> - Running causes the sheep to lose fullness and they can't eat whilst running so if they can't get away from the sheep dog in time... they die!
> 
> **The sheep dog will:**
> 1. **Chase the nearest sheep**
> - The sheep dog scans the area and finds the nearest sheep and chases after it.
> 
> **The model ends when half of the initial number of sheep have been eaten or have died of old age or starvation.**
> 
> **Extras:**
> 1. The sheep's initial locations are taken from a webpage that the model scrapes.
> 2. When the model has finished running it outputs a text file with how many iterations it ran for.
> 3. The model features a GUI with a menu from which you can run it.
![](/animation.gif "Agent Based Model")
