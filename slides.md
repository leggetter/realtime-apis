name: lblue
layout: true

class: bg-light, center, middle

---

class: title

# So, you want to build a Real-time API. Where do you start?

* <span class="speaker">Phil @leggetter</span>
* <span class="speaker-job-title">Head of Evangelism</span>
* <span class="speaker-pusher-logo"></span>

???

* Pusher is a hosted service with APIs & SDKs that make it easy to integrate
real-time data and functionality into web, mobile and IoT apps using any
technology at any stage of development.
* Our customers tend to be building app.
* But some of those customers also share their data with their customers
* Effectively making us a Real-Time API infrastructure

---

# What we'll cover

* 5 Reasons you should offer a Real-Time API
* Transports
* Communication Patterns
* ~~Protocols~~
* ~~Security & Scaling~~
* Frameworks & Tools
* Conclusion
* Real-Time API Quiz (if time)

---

class: bg-dark

# 5 Reasons you should offer a Real-Time API

---

# 1. You have Real-Time Data

---

## Finding the Real-Time Data

Any **event** in your system = **Real-Time Data**

* Changes in data
* System interactions
* User interactions

---

<a href="https://www.youtube.com/watch?v=P31lGHG_lL4">
	<img width="80%" src="./img/you-have-realtime-goffice-record.png" />
</a>


<a href="https://www.youtube.com/watch?v=P31lGHG_lL4">
youtube.com/watch?v=P31lGHG_lL4
</a>

---

# 2. Faster access to business value

???

* Simple
* The sooner your API consumers can have the data the sooner they gain the business value if offers.

---

# 3. Some Data has a Time Factor

---

background-image: url(./img/warp-core.gif)
class: em-text, trans-h, top

# WCaaS

--

## Warp Core as a Service

???

* The saftey system monitoring API needs to be realtime

---

background-image: url(./img/core-breach.gif)

???

* Or the Chief Engineer won't be happy
* Saucer separation scenario

---

## Time Factor

* Monitoring
* Market data & betting
* Communications e.g. phone calls & chat
* Collaborative experiences

---

# 4. Developer Empowerment + Experience

---

background-image: url(./img/developers-want-realtime.png)
class: center, bg-cover, em-text, trans-h, top

## Developers Want Real-Time

[leggetter.co.uk/2012/11/06/developers-want-realtime.html](http://www.leggetter.co.uk/2012/11/06/developers-want-realtime.html)

---

## Deliver the new or updated information to them (Push)

---

# 5. Users Expect Real-Time Experiences

---

<img width="20%" src="./img/facebook.png" />
<img width="20%" src="./img/uservoice.png" />
<img width="25%" src="./img/google-docs.png" />
<img width="20%" src="./img/uber.png" />

---

## Enable your customers to Build Apps with Real-Time Features with your API

---

# Why have a Real-Time API?

* You have real-time data. Gain value from it!
* Quick business value
* Time Factor/Constraints
* Improve the Developer Experience & Empower them
* Help consumers building Real-Time features

---

class: bg-white
background-image: url('./img/apps-with-realtime-apis.png')

???

* This image shows only "apps" with realtime APIs
* Not included API services - Pusher, Twilio, SendGrid, MailJet, Firebase etc.

---

class: bg-dark

# Real-Time API Transports

???

* How do you deliver the real-time data to your API consumers?

---

class: bg-dark

## Factors to consider

* API Consumer? Server or Client
* Message update frequency
* Direction of communication
* Message latency
* Efficiency

---

class: bg-dark, top

## WebHooks

--

* Server only
* Low update rates
* Uni-directional
* Avg. latency
* High. efficiency (for servers)

---

background-image: url(./img/polling.png)
class: bg-dark, trans-all

--

* Server or Client
* Low update rates
* Batched bi-directional
* High latency
* Low efficiency
--
<img src="./img/no-entry.png" class="fill overlay" />
---

background-image: url(./img/long-polling.png)
class: bg-dark, trans-all

--

* Server or Client
* Avg. update rates
* Batched bi-directional
* Avg. latency
* Avg. efficiency

---

background-image: url(./img/streaming.png)
class: bg-dark, trans-all

--

* Server or Client
* High update rates
* Uni-directional
* Low latency
* High efficiency

---

## Server-Sent Events

If you're considering either HTTP Long-Polling or HTTP Streaming then align with the
[Server-Sent Events standard](http://www.w3.org/TR/2009/WD-eventsource-20091029/).

---

background-image: url(./img/websocket.png)
class: bg-dark, trans-all

--

* Server or Client (normally client)
* High update rates
* Bi-directional
* Low latency
* High efficiency

---

class: bg-dark, top

## WebRTC

--

* Server or Client (normally client to client)
* High update rates
* Bi-directional
* Low latency
* High efficiency

---

class: bg-dark

# Real-Time Tech Communication Patterns

(Not considering WebHooks or WebRTC)

???

---

## Real-Time Tech Communication Patterns

* Simple messaging
* Publish-Subscribe
* RPC/RMI
* Data Sync

???

---

## Simple messaging

No abstractions. Just messages.

* Fits well with HTTP/REST
* Many persistent connections

???

* Keep existing RESTful GET endpoints
* Allow GET requests to be long-held
* Infrastructure to support connections
* Clients need to make many connections

---

## PubSub

Subscribe & Publish on "channels"

* Channels. Multiplexed. Single connection
* Clearly partitions complex data
* Dedicated endpoint
* Requires SDK

???

* Efficient PubSub requires push over single connection
* WebSocket required if subscriptions change frequently
* Or client publishes frequently

---

## RPC/RMI

Call API "methods"

* Dedicated endpoint + protocol
* SDK required
* Hides network activity from developer

???

*

---

## Data Sync

Interact with, and synchronize, data structures

* Dedicated endpoint + Protocol
* New paradigm
* SDK required
* Hides network activity from developer

???

* 

---

class: bg-dark

# Real-Time API Frameworks

???

---

class: bg-white
background-image: url(./img/realtime-web-solutions-updated.png)

---

class: top

## Choose one that meets your requirements

How do you do that?

--

1. Choose one that offers the functionality you need
--

2. Watch my videos :)

<a href="https://www.youtube.com/watch?v=PUENh1Ym9E4"><img src="./img/10min-guide-realtime.png" width="40%" style="float: left; margin-left: 5%;" /></a>

<a href="https://www.youtube.com/watch?v=VENVNimklWg"><img src="./img/fowa-choosing-realtime.png" width="40%" style="float:right; margin-right: 5%;" /></a>

---

background-image: url(./img/rtw-api-decision-matrix-bg-white.png)

---

background-image: url(./img/rtw-tech-decision-matrix-solutions.png)

---

class: bg-dark

# Real-Time API Tools

???

---

## Real-Time API Tools? Not Many

* Lots for WebHooks - it's HTTP
* [SwaggerSocket - REST over WS](https://github.com/swagger-api/swagger-socket)
* Fanout.io<sup>†</sup>
* StreamData.io<sup>†</sup>
* SailsJS<sup>†</sup>

<small>† frameworks, but offer a form of tooling</small>

???

* No standard for WebHooks other than POST and signed auth

---

class: top

## So, you want to build a Real-time API. Where do you start?

1. **Understand** & **Identify** your valuable Real-Time Data (**Events**)
2. Define the API Consumer and choose **Transports**
3. Decide on the best **Communication Pattern**
4. Can an existing **Real-Time Framework** help?
--

5. We need better Real-Time API tooling 

???

1.
2. Consumed by server, browser, mobile, fridge... ?
3. For your API functionality

---

class: title

# So, you want to build a Real-time API. Where do you start?

## Questions?

[leggetter.github.io/realtime-apis](http://leggetter.github.io/realtime-apis/)

* <span class="speaker">Phil @leggetter</span>
* <span class="speaker-job-title">Head of Evangelism</span>
* <span class="speaker-pusher-logo"></span>

---

# Appendix

---

# Real-Time API Quiz
## Example Scenarios

1. What transport?
2. What communication pattern?
3. What's the company?

---

class: top

## Scenario 1

* Predefine query within service
* Push to servers
* Frequent data updates
* Potentially large message payloads

--
* **HTTP Streaming**

--
* **Simple messaging**

--

![DataSift logo](./img/datasift.png)

---

class: top

## Scenario 2

* Push to server
* Occasional data updates ("events")
* Delivery within ~1 of event

--
* **WebHooks**

--
* **Simple messaging**

--

![Twilio Logo](./img/twilio.png)

---

class: top

## Scenario 3

* Push to browsers, native mobile & anywhere
* Frequent data updates ("events")
* Delivery within 250ms
* Partitioned data

--
* **WebSocket** + HTTP fallback

--
* **PubSub** + events

--

![Pusher Logo](./bower_components/pusher-remark-themes/img/pusher-logos/pusher-slogan-dark.png)

---

class: top

## Scenario 4

* Multi-device comms via central storage
* Frequent data updates
* Delivery within 1s

--
* **WebSocket** (+ HTTP Streaming)

--
* **Data Sync**

--

![nest Logo](./img/nest.png)

---

## Resources

* [leggetter.github.io/realtime-apis](http://leggetter.github.io/realtime-apis/) - slides
* [pusher.com](https://pusher.com) - real-time infrastructure as a service
* [Real-Time Technology Guide](http://www.leggetter.co.uk/real-time-web-technologies-guide/)

---

class: title

# So, you want to build a Real-time API. Where do you start?

## Questions?

[leggetter.github.io/realtime-apis](http://leggetter.github.io/realtime-apis/)

* <span class="speaker">Phil @leggetter</span>
* <span class="speaker-job-title">Head of Evangelism</span>
* <span class="speaker-pusher-logo"></span>
