
--Problem example
For initial launch rail sims, I had no knowledge of MatLab, so I wrote up everything in excel. The problem came up when I had to implement a way to account for applying numerical approximation via iteration with different constraint variables: min AoA, wind speed, rail tilt, and rail length. There was no native feature for this in excel, but I did find a solution in VBA code within excel which allows for cell edits in real-time, which permitted me to iterate towards a solution for a given set of constraints. This was able to give me the desired results in a feasible, yet somewhat long runtime.


--Conflict Example

YJSP git branch merge conflict


--Why I am passionate about Space

I am passionate about space for numerous reasons, which can be summarized by innovation, survival, and exploration. To me, the most important aspect of space exploration lies in the innovative technologies that are developed alongside a launch vehicle. Whether it be GPS satellites or ISS research, it is impossible to dispute that humans have used space to develop many new technologies and data tools that have improved the standard of living for nearly every person on the planet. The cost of each space mission is still way too high to be relevant to most people, however, and innovations in rocket manufacturing will undoubtedly be key to reducing the cost of launch making space much more accessible. Next to innovation is our survival as a species, and it is clear that in order to ensure the best chance of avoiding extinction, we must expand our presence beyond Earth and establish ourselves as an interplanetary species. Specifically, Mars and the Moon are prime candidates for human colonies, which will also enhance our research capabilities in these unique environments. As for exploration, I am naturally curious about our surroundings and want to explore beyond where the eye can see. We can see a lot with modern telescopes, but advancing rocket technologies and efficiency in the next few centuries could enable us to extend our reach beyond our solar system and push humanity closer to Type II on the Kardashev scale.


--Technical project example

One of my technical projects from my work on the Yellow Jacket Space Program involved translating data from our static hot fires to models for engine performance including thrust and mass-loss rate. This process involved integrating a basis of knowledge about liquid rocket engine systems and data science to combine multiple datasets from different hot fires into a single curve to model a full duration burn. More specifically, I scaled the time windows to be the same for each hot fire, and then I performed a piecewise logistic regression on these datasets. The cutoffs to separate phases of the piecewise regression related to the various phases of engine performance during the burn: startup, stabilization, steady-state, and cutoff.
My role as a Flight Dynamics Simulation Architecture Engineer in the Yellow Jacket Space Program at GA Tech is my contribution to the organization's long-term goal of being the first collegiate team to design and build a liquid-propelled rocket that passes the Karman Line at 100 km altitude. All of my work relates to the flight dynamics team and most of my work is within the subteam of simulation architecture. On this simulation architecture subteam, there's usually an average of 5 members, and I have been responsible for managing certain parts of our 6DOF MatLab code by making key decisions regarding go/no-go specifications based on vehicle launch stability analyses.
