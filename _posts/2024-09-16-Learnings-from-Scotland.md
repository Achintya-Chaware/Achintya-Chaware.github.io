
<p align = "justify">
In my engineering at MIT WPU, I was a part of a student team called Vegapod Hyperloop. I joined the team towards the end of my first year as an electronics and navigation engineer, then became the Head of the electronics and navigation subsystem in the next year.
</p>
<p align = "justify">
Vegapod Hyperloop is a student team working towards building the technologies for the Hyperloop which is a fifth mode of transportation envisioned by Elon Musk that focuses on speed and sustainability. Hyperloop is a futuristic transportation system that envisions eliminating all friction from the current high speed trains. The “pods” will levitate and won’t touch the track eliminating friction and they will run inside vacuum tubes eliminating drag. This whole system will use advanced technologies and material and will be powered using a sustainable source of energy. 
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%201.jpeg" width = "350"/>
  <figcaption>Team Vegapod Hyperloop at the Mumbai Airport</figcaption>
</figure>
<br>
<p align = "justify">
Every year, we participate in a competition called the European Hyperloop Week. This competition is organized collectively by four student hyperloop teams from University of Edinburgh, Technical University of Valencia (UPV), ETH Zurich and TU Delft. Teams from various top universities globally participate in this competition. The nature of competition is quite open ended in a way that it does not define a hyperloop system in any way but the development has to be done adhering to a very strict rulebook with a core focus on safety. The competition has 4 stages, namely, the Intent to Demonstrate (ITD), the Final Design Documentation (FDD), the Testing and Safety Documentation (TSD) and the final jury round at the venue of the competition. 
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%202.jpeg" width = "560"/>
  <figcaption>The Team at the University of Edinburgh</figcaption>
</figure>
<br>
<p align = "justify">
The EHW 2023 was held at the University of Edinburgh in Scotland. I participated in that competition along with the team as the Head of Electronics in that competition. For the previous one year leading up to the competition, I led a team of 5-6 people working on the electronics and navigation system of the pod which was responsible for controlling the entire pod and acquiring various data about its health and performance. For a new team like ours with a very low budget compared to others, we did quite well. We became the first Indian team to clear the TSD rounds and to be inspected by the jury, and the jury was very happy with the work we had done to say the least.
</p>
<br>
<figure align = "center">
  <img src=" https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%203.jpeg" width = "560"/>
  <figcaption>Me and the Pod</figcaption>
</figure>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%204.jpeg" width = "560"/>
  <figcaption>Assembling the Pod in the Living Room of our Airbnb</figcaption>
</figure>
<br>
<p align = "justify">
This whole journey though, was not perfect by any standards. My own subsystem did not work and we faced a lot of issues that prevented us from running the pod on the track and getting nominated for any awards. I have spent a lot of time analyzing what could have been done better, especially personally. This article is a compilation of a few broad, top level learnings about making a complex system and leading a team learnt from my and the team’s mistakes and also the things done right by the other teams.
</p>
<p align = "justify">
Although these learnings are from a mere student competition, I hope they are transferable to other things in life.
</p>
<h2>1. Focus is Key</h2>
<p align = "justify">
It is very easy to fall for the trap of over-engineering. We have always heard that simple systems are very robust blah blah but it goes beyond that. It is important to question, at every step, whether what you are doing is really necessary and if you are reinventing the wheel. Especially when you are short on money or time or both.
</p>
<p align = "justify">
It is easy to end up doing what is more lucrative than what is required. In our case, lucrative was something that was technically more challenging, because we were doing this to improve our skills. 
</p>
<p align = "justify">
Having a strong set of cohesive top-level objectives and requirements for any complex system is very important. Focus is working towards fulfilling these objectives and requirements in the best possible way rather than making something that is sophisticated. 
</p>
<p align = "justify">
Oftentimes we chase perfection, by making every single element of the system “perfect” and somehow hoping that all the elements will somehow converge to form a perfect system. But, in my experience, perfection is extremely hard to achieve bottom up. For most things, if we have some strong top-level objectives and requirements and if we make a system that is optimized for perfection within those constraints, we just have to choose elements of subsystems that “work”, which is much easier to do.
</p>
<p align = "justify">
Since I come from an electronics background, I would especially emphasize that the electronics or the control system is often the top level subsystem in these types of systems. So making sure that objectives and requirements are being met almost becomes the job of the person responsible for the control systems.
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%205.jpeg" width = "560"/>
  <figcaption>The Brain behind our Edinburgh Pod (the “MVCU”)</figcaption>
</figure>
<br>
<p align = "justify">
In the context of Vegapod, we used to have a working electronics and navigation system based on the RPi. It was easy to work with and we could’ve run the pod using that. But, instead, we decided to make a fully embedded, delocalised system because we thought that it would be very cool. In theory, if this system worked, it would have been brilliant. But it wasn’t practical. In a tough competition, we should have done what works for sure rather than what sounds cool to do.
</p>
<p align = "justify">
Focus is a game of what you optimize for. We optimized for learning and that wasn’t necessarily wrong. 
</p>
<h2>2. Improvise when Time is Short</h2>
<p align = "justify">
I have this habit of having to understand something through and through before actually using it for a practical application. But, I have learnt that it is important to improvise. If you find some resource that gives you the recipe to use that tool or an example of a prior usage of that tool, make use of that tool by following that recipe. It is okay if you don’t understand fully how it works as long as it works. This isn’t always a good idea, but more often than not it is, also because when you follow the recipe and use that tool, you will understand how it works to a certain extent. This particular thing is generally done for code when we use libraries. We don’t necessarily have to know what the library is doing internally as long as it produces the result we want. 
</p>
<p align = "justify">
Making a system that satisfies the given basic requirements takes some effort and time but more than that, optimizing that system takes more effort and time. When time is short, this optimization part can be saved for the end if there is spare time.
</p>
