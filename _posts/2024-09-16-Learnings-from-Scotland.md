
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
<h2>3. Systems Engineering</h2>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%206.jpeg" width = "350"/>
  <figcaption>The Immaculate Swissloop Pod Interior</figcaption>
</figure>
<br>
<p align = "justify">
As the title suggests, systems engineering is a type of engineering technique that is used to develop and manage complex systems. This framework is extremely useful to break down complex systems into its constituent pieces and solve them one piece at a time. It is a methodical approach to deal with complexity and has been extensively used by the likes of NASA. NASA has a systems engineering handbook that is especially useful for getting started with this framework (https://www.nasa.gov/wp-content/uploads/2018/09/nasa_systems_engineering_handbook_0.pdf). We did not use systems engineering frameworks for working on our pod. This taught me that it is not only an engineering framework but also a team management framework. There are two aspects in which it could’ve helped 
</p>
<ol type="a">
  <li align = "justify">Our pod turned out to be a patchwork of every team member’s individual efforts rather than a homogeneous system. If the requirements analysis was done properly, it might have helped with the hundreds of constituent parts to make a homogeneous system. The way that we used to make our parts fit together was to make a mechanical CAD of the complete pod with the constituent parts still under development and undergoing changes. We locked the functionality/solutions on the basis of basic requirements set by the rulebook rather than locking the complete requirements and then finding the solution that fits best.</li>
  <li align = "justify">It is very easy for teams to get lost in activity. Especially when they are college students who are forced to sit and work in the workshop. Progress on a project has to be measured on the basis of results (https://www.youtube.com/watch?v=JAk448volww). For any kind of project, we cannot wait for the project to get over to access the results. Various kinds of indicators are used for this purpose in the industry. But for complex systems, the requirements we define in the very beginning can serve as the indicators. Looking at the requirements and concluding, using credible testing or hypothesis that they are indeed getting solved one by one is an indicator of the puzzle getting solved one requirement at a time.</li>
</ol>
<h2>4. Continuous Testing</h2>
<p align = "justify">
As mentioned in the last point, we have to keep testing using credible methods whether the system we are making is fitting the requirements we have set. Credible test methods can include specialized test setups, templates, etc. Making test setups is one area where there is a lot of opportunity for some out of the box thinking. If we do not keep testing our system and its individual parts, we do not know whether we are fulfilling the requirements.
</p>
<p align = "justify">
Doing testing parallel to the entire development lifecycle also gives us an opportunity to double down on what works and drop what doesn’t work. In Vegapod electronics, we tried to design the perfect system. But perfection only matters if functionality exists.
</p>
<p align = "justify">
These principles of continuous integration are widely used in software development but not so much in hardware, because it is hard. The point about improvising that I mentioned before might sound exactly opposing this, but improvising is about the methodology and testing is about the outcome. We have made the mistake of improvising the outcomes which is basically the infamous “Jugaad”.
</p>
<h2>5. Having a Plan B, C, D and Further</h2>
<p align = "justify">
Every decision that affects a functional requirement must have multiple contingency plans in case the original plan doesn’t work out. In our pod, we were betting on a series of interdependent things just working out without a solid plan B. What makes a plan B solid is whether or not that plan or method has been validated by someone or somewhere before. This is quite difficult for new teams like us who do not have a legacy of previous generation systems.
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%207.jpeg" width = "560"/>
  <figcaption>The 2023 Delft Hyperloop Pod</figcaption>
</figure>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%208.jpeg" width = "560"/>
  <figcaption>Plan B Implementation on the Delft Hyperloop Pod</figcaption>
</figure>
<br>
<p align = "justify">
The 2023 Delft Hyperloop pod demonstrated this very well. While the pod was brilliantly engineered, admittedly they did not have a strong electronics team that year and they had to rely on a plan B subsystem that looked as if it was put together at the last moment.
</p>
<h2>6. Someone has Probably Done it Before</h2>
<p align = "justify">
There are some problems which you will take months to solve but there definitely exists a person who can solve it in days or hours. Especially in the case of student teams, it happens sometimes that all we can see is the problem and we try to solve it with the tools or knowledge that we have. In my experience, whenever you are stuck, it is a great idea to ask yourself and explore. Take a step back and get a big picture on the situation, explore if you have any “wild card” ways to solve that problem. Can we use a totally different approach? Are there any tools to solve this problem that we don’t know? Is there any common knowledge that is used by the people who work on these sorts of problems every day? Is there anyone we can ask about this?
</p>
<p align = "justify">
In Vegapod, our electronics subsystem was based on an embedded delocalised architecture connected in a star topology. Inspired by the AUTOSAR architecture, there was an MVCU (Master Vehicle Control Unit) and a bunch of VCUs (vehicle Control Units) were attached to it. These communicated with the MVCU using CAN (Controller Area Network), an automotive industry standard.
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%209.jpeg" width = "560"/>
  <figcaption>One of the VCUs</figcaption>
</figure>
<br>
<p align = "justify">
Implementing CAN into our system proved to be a major challenge for us as we were doing it from scratch and we almost had no idea what are the possible ways of implementing it. But in hindsight, if we had contacted someone from the automotive industry who is experienced with CAN, it would’ve helped us massively at the time because it turns out that there are totally different ways available of implementing that topology more easily and robustly.
</p>
<h2>7. Presentation</h2>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%2010.jpeg" width = "560"/>
  <figcaption>Me Presenting the Electronics Subsystem to the Jury</figcaption>
</figure>
<br>
<p align = "justify">
I think that the objective of a presentation is to create a narrative rather than to simply deliver information. You are trying to “present” your version of the story. A way to think about this is that an audience is a mandatory component for a presentation. So, it is important to think from the audience’s perspective and present them with something that keeps their attention and delivers the necessary information. Presentation offers you some room to emphasize on what you set out to create rather than giving the technical details of what you have created. You can be generous about explaining your vision for the system that you have created. You can control what the person thinks about what you have created through the presentation. I believe that we did not use this power that presentations provide to the full extent. We could’ve been more on point with the information and more persuasive with the narrative. I think Swissloop and Delft Hyperloop had some of the best presentations I have seen, they killed it. 
</p>
<br>
<p align = "justify">
EHW 2023 was an exhilarating (and sometimes almost traumatic) experience for me. It showed me how valuable it can be with the best in your field, albeit for only a week. It was not just a great engineering experience but it was much more than that. I am fortunate that I got to make the mistakes that I did, I think the memories and learnings will stay with me forever. Here’s a bonus picture of the beautiful city of Edinburgh! 
</p>
<br>
<figure align = "center">
  <img src="https://raw.githubusercontent.com/Achintya-Chaware/Achintya-Chaware.github.io/master/images/Scotland%20Blog%2011.jpeg" width = "560"/>
  <figcaption>Probably the Most Beautiful City I have been to</figcaption>
</figure>
