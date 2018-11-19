![original](img/title.png)

---

![original](img/slide1.png)

---

### Visualizing Serverless Architectures
#### What makes a **healthy** serverless application?

---

# About Me

* @nodebotanist
* Mx. Kas Perch (They/Their/Them)
* Developer Relations Specialist
* Maker
* EE Student

![right](~/Dropbox/img/alladinsane.jpg)

---

# [fit] Robots/Nodebots Author

![](~/Dropbox/img/book1.jpeg)
![](~/Dropbox/img/book2.jpg)
![](~/Dropbox/img/book3.png)

---

## Catparent

![](~/Dropbox/img/babies.jpg)

---

# [fit] There are still a lot of
# [fit] misconceptions
# [fit] about serverless

---

"We just spent 10 years convincing people that JS belongs on servers, and now they want to take servers away!"

- Some Rando

---

![inline](~/Dropbox/GIFS/welp.gif)

---

# The state of Serverless ops: Reactionary

* Firmly in the reactionary stage in most cases
	* "Oh no, it's down, why is it down?!"
* We keep some metrics, but there's so many unknowns!

---

## Development and Ops tooling from **most** providers is still kind of a nightmare.

## Third-party tools are starting to fill some gaps, but we're still a bit behind.

---

# Why are observability and monitoring so hard in Serverless?

![](~/Dropbox/img/jawbreaker.jpg)

Because it is an abstraction of runtime environment-- your provider controls your access to any information about your runtime environment, from the version of your language to the OS.

---

Because at the end of the day, developers love abstractions (don't @ me on this one).

![inline](~/Dropbox/GIFS/smoke-bomb.gif)

---

# The ideal: Preventative

* Being able to observe your serverless application from the 10,000m view down to each invocation
* Being able to see metrics over time, to see problems before they arise
* Instead of wondering why the app is down, prevent the problems that would take it down

---

# [fit] But how do we get from 
# [fit] **reactionary**
# to 
# [fit] **preventative**?

---

# The Observability Craze

* Monitoring is out, observability is in
* Observability allows us to handle unknowns better in this chaotic, uncharted new space
* It's less of a craze and more of an evolution in operations technique

---

# [fit] However,
# [fit] **Metrics**
# are still 
# [fit] **important**!

---

# Metrics are still important

* We need some landmarks to gauge where we're going and where we've been
* It's hard to ingest large amounts of observed data without categorization
* Metrics, when planned well, are easy to turn into digestable, usable visualizations

---

# [fit] Some common serverless metrics

---

# Memory usage/CPU Usage

* Spot memory leaks over time
* Know when to scale up (or down!) your serverless functions
* Know when to split off a task or use an external service

---

# Errors

* You want to know when, why, and how a function invocation fails
* You want to know if there's a ripple, and where that ripple begins
* Is the cause your app, or a dependency being down, or a provider outage?
* What is the user seeing when your function errors?

---

# Error Rate

* You don't need to sound the alarms (necessarily) if 100 invocations cause an error...in over 1,000,000 invocations total (.01% error rate)
* The rate of errors to invocations is a key piece of perspective when evaluating the health of a serverless application!

---

# Cold Starts

* If you have a high rate of cold starts, you'll have to factor in how this affects your performance
* You need to be able to tell why there is a high rate of cold starts: is the function not called often enough? Or are there peaks of activity that require lots of instances to be spun up all at once?

---

# Custom Metrics

* One of the key benefits of observability is the ability to define your own custom metrics that fit your particular goals
* The amount of time a certain task takes, the user data that impacts your function, or anything you can think of!
* The downside: this does require instrumentation of your code
	* (But there are tools out there to help!)

---

# But what about
# [fit] **Observability**?

---

# Moving into observability

The key difference between monitoring and observability is monitoring is watching the data points you know about, observability means collecting as much relevant data as possible to see the bigger picture

---

# Observability in Serverless Applications

What we're looking for is the ability to see what was happening in our application is a given point in time, so we can pull data points that may later become metrics from it.

---

# Another key element: Time

* Data is most useful when aggregated and visualized over time
* Staring at the data during an incident only gives you the knowledge to fix it now, not necessarily prevent it from happening again

---

# [fit] Observability = **Context**

---

## **Demo Time**: 

### [Attempt at] Observing an Azure Function

### nodebotani.st/set?color=[your css color]

---

The world of serverless observability and operations is trying to keep pace with an explosion of growth in serverless use. But the tooling is working its way through, and the future is bright!

---

# Thanks for Listening!

* Kassandra Perch
* @nodebotanist
* Developer Relations Specialist

![inline](~/Dropbox/GIFs/carl-sagan-youre-awesome.gif)

---

![original](img/slide2.png)

---

![original](img/slide3.png)