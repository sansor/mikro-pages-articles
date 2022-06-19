# The 7 Software “-ilities” You Need To Know
In the world of software architecture there are many “-ilities” you must take into consideration with every project. Prioritizing them is necessary because the client will optimistically ask that you do all of them. To help you out, here is a quick list outlining my top 7 default “-ilities” in the order that I prioritize them:
## 1. Usability
Software usability can be described as how effectively end users can use, learn, or control the system. Some questions to ask yourself to determine usability might be:
* Is there a UI metaphor that I am using to help users adapt? (for example, the ‘desktop’ is a metaphor)
* Are the most common operations streamlined to be performed quickly?
* Can new users quickly adapt to the software without help? (is it intuitive?)
* Do validation and error messages make sense?
## 2. Maintainability ( or Flexibility / Testibility)
The definition of maintainability [for me] implies how brittle the code is to change. As a result, I tie the terms flexibility and testability into the overall maintainability of a project.
* Does the entire team understand the code base or does knowledge islands exist?
* Is the code throughly regression tested?
* Can modifications to the project be done in a timely manner?
## 3. Scalability
Scalability is the ability for your program to gracefully meet the demand of stress caused by increased usage. In short, ensuring your program doesn’t slow or bust when pounded by more users than you originally anticipated.
* What is your current peak load that you can handle?
* How many database records can create until critical operations slow down?
* Is the primary scaling strategy to “scale up” or to “scale out” — that is, to upgrade the nodes in a fixed topology, or to add nodes?
## 4. Availability (or Reliability)
How long the system is up and running and the  [Mean Time Between Failure (MTBF)](http://en.wikipedia.org/wiki/MTBF)  is known as the availability of a program.
* How long does the system need to run without failure?
* What is the acceptable length of time for the system to be down?
* Can down times be scheduled?
## 5. Extensibility
Are there points in the system where changes can be made with (or without) program changes?
* Can the database schema flex to accommodate change?
* Does the system allow Inversion of Control (IoC)?
* Can end users extend the system (scripts, user defined fields, etc)?
* Can 3rd party developers leverage your system?
## 6. Security
I shouldn’t need to go into this one but to be thorough I like this  [definition of security](http://www.softwarearchitectures.com/go/Discipline/DesigningArchitecture/QualityAttributes/tabid/64/Default.aspx) : the measure of system’s ability to resist unauthorized attempts at usage or behavior modification, while still providing service to legitimate users.
* Does the system need user or role based security?
* Does code access security need to occur?
* What operations need to be secured?
* How will users be administered?
## 7. Portability
Portability is the ability for your application to run on numerous platforms. This is can include actual application hosting, viewing, or data portability.
* Can the data be migrated to other systems?
* For web applications, which browsers does your web app support?
* Which operating systems does your program run on?