name: lblue
layout: true

class: bg-light, center, middle

---

class: title

# So, you want to build Real-time API. Where do you start?

* <span class="speaker">Phil @leggetter</span>
* <span class="speaker-job-title">Head of Evangelism</span>
* <span class="speaker-pusher-logo"></span>

???


---

# What we'll cover

* 5 Reasons you should offer a Real-Time API
* Transports
* Data
* Real-Time API Quiz
* Tools
* Frameworks
* Security
* Scaling

---

class: bg-dark

# 5 Reasons you should offer a Real-Time API

---

# 1. Faster access to business value

???

* Simple
* The sooner your API consumers can have the data the sooner they gain the business value if offers.

---

# 2. Some Data has a Time Factor

---

background-image: url(./img/warp-core.gif)
class: em-text, trans-h, top

# WCaaS

--

## Warp Core as a Service

---

background-image: url(./img/core-breach.gif)

---

## Time Factor

* Notifications
* Monitoring
* Market data
* Betting
* Incoming phone calls
* Short-lived deals/offers

---

# 3. Developer Convenience

---

background-image: url(./img/developers-want-realtime.png)
class: center, bg-cover, em-text, trans-h, top

## Developers Want Real-Time

[leggetter.co.uk/2012/11/06/developers-want-realtime.html](http://www.leggetter.co.uk/2012/11/06/developers-want-realtime.html)

---

## Deliver the new or updated information to them (Push)

---

# 4. Users Expect Real-Time Experiences

---

class: em-text, bg-cover, trans-h, top
background-image: url(./img/itv-news-may-2014.png)

# Notifications & Signalling

---

class: bg-video, em-text, trans-h, top, vid-width-100

# Analytics/Visualizations

<video id="video" autoplay="true" loop="true">
	<source src="./img/librato.mp4" type="video/mp4">
</video>

---

class: center, bg-cover, em-text, trans-h, top
background-image: url(./img/delighted-app.gif)

# Activity Streams

???

* a stream of activity
* things have - and are - happening
* synonymous with social apps

---

class: bg-dark, bg-cover, em-text, trans-h, top
background-image: url(./img/sprintly.jpg)

# Multi-User Collaboration

???

---

## Enable your customers to Build Apps with Real-Time Features

---

# 5. A Mixture

* Quick business value
* Time Factor/Constraints
* Developer convenience
* Building Real-Time features

---

class: bg-dark

# Real-Time API Transports

???

* How do you deliver the real-time data to your API consumers
* 6 low-level possibilities

---

class: bg-dark

## Factor to consider

* API Consumer? Server or Client
* Message update frequency
* Direction of communication
* Message latency
* Efficiency

---

class: bg-dark

## WebHooks

---

class: bg-dark

## WebHooks

* Server only
* Low update rates
* Uni-directional
* Avg. latency
* Avg. efficiency

---

background-image: url(./img/polling.png)

---

class: bg-dark

## HTTP Polling

* Server or Client
* Low update rates
* Batched bi-directional
* High latency
* Low efficiency

---

background-image: url(./img/long-polling.png)

---

class: bg-dark

## HTTP Long-Polling

* Server or Client
* Avg. update rates
* Batched bi-directional
* Avg. latency
* Avg. efficiency

---

background-image: url(./img/streaming.png)

---

class: bg-dark

## HTTP Streaming

* Server or Client
* High update rates
* Uni-directional
* Low latency
* High efficiency

---

background-image: url(./img/websocket.png)

---

class: bg-dark

## WebSocket

* Server or Client (normally client)
* High update rates
* Bi-directional
* Low latency
* High efficiency

---

class: bg-dark

## WebRTC

---

class: bg-dark

## WebRTC

* Server or Client (normally client to client)
* High update rates
* Bi-directional
* Low latency
* High efficiency

---

class: bg-dark

# Data

???

---

todo

---

# Real-Time API Quiz

---

class: bg-dark

# Real-Time API Tools

???

---

todo

---

class: bg-dark

# Real-Time API Frameworks

???

---

todo

---

class: bg-dark

# Securing Real-Time APIs

???

---

todo

---

class: bg-dark

# Scaling Real-Time APIs

???

---

todo

---

## Resources

* http://pusher.com - easily add realtime messaging to your apps
* http://webcomponents.org/
* https://www.polymer-project.org
* [Eric Bidelman's Google IO 2014 talk](http://polymer-change.appspot.com/)
* [Angular Material](https://material.angularjs.org/)
* [Google Material Design](http://www.google.com/design/spec/material-design/introduction.html)
* [HTML Template Chooser](http://garann.github.io/template-chooser/)
* [IE UserVoice forum](https://wpdev.uservoice.com/forums/257854-internet-explorer-platform/filters/top)
* [Source for these slides](https://github.com/leggetter/web-components-now/tree/devweek-2015)

---

class: title

# Why you should be using Web Components Now. And How.

## Questions?

[leggetter.github.io/web-components-now](leggetter.github.io/web-components-now)

* <span class="speaker">Phil @leggetter</span>
* <span class="speaker-job-title">Head of Evangelism</span>
* <span class="speaker-pusher-logo"></span>
