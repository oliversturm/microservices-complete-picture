title: Microservices
subtitle: An (Almost?) Complete Picture
class: animation-fade
layout: true

<!-- This slide will serve as the base layout for all your slides -->

.bottom-bar[
{{title}}
]

---

class: impact

# {{title}}

## {{subtitle}}

.title-oli[
Oliver Sturm &bull; @olivers &bull; oliver@oliversturm.com
]

.title-logo[
<img src="template/devexpress.png" id="devexpress" alt="DevExpress"><img src="template/mvp.png" id="mvp" alt="MVP">
]

---

## Oliver Sturm

* Training Director at DevExpress
* Consultant, trainer, author, software architect and developer for over 25 years
* Microsoft C# MVP

* Contact: oliver@oliversturm.com

---

## Agenda

* Service structure
  * A look at a microservices architecture
* Communication
  * Considerations pro and con frameworks
  * Working with individual services
* Packaging/deployment
  * Developer concerns
  * Real-world deployment with AWS
* Developer stuff
  * Debugging
* And what about Serverless?

---

## Major Goals of Microservice Architectures

* Services should be easily maintainable _building blocks_
* _Separation of concerns_ and responsibilities, technically and in development teams
* Benefit from _skills_ and _technological advancements_
* Long-term security for investments through _modularization_

---

## Seven Services of the Demo Application

.svg-light-width[
![Seven Services of the Demo Application](services1.svg)
]

---

## Querying Data

.svg-light[
![Querying Data](query.svg)
]

---

## Creating a New Row

.svg-light[
![Creating a New Row](create-new-row.svg)
]

---

## Additional Services for Advanced Architecture

.svg-light-width[
![Additional Services for Advanced Architecture](services2.svg)
]

---

## Querying Data with CQRS/ES

.svg-light[
![Querying Data with CQRS/Event Sourcing](es-query.svg)
]

---

## Creating a New Row with CQRS/ES

.svg-light[
![Creating a New Row with CQRS/Event Sourcing](es-create-new-row.svg)
]

---

## Communication

* Structural question: _who talks to who_?
* Implementation question: _how does the talking work_?

---

## Direct Communication

.svg-light[
![Direct Communication](communication-direct.svg)
]

---

## Using a Broker

.svg-light[
![Using a Broker](communication-broker.svg)
]

---

## How does the Talking Work?

* Each service could be an _open web service_ with its own external interface. REST? Proprietary? Your choice.
* Each service could be implemented to _talk to the broker exclusively_
* _Libraries_ exist that implement communication

---

## Packaging/Deployment

* Running lots of services manually isn't much fun
  * Consider _automation_
* Services may need _individual runtime environments_
* _Container systems_ to the rescue!

---

## Debugging

* _Granularity_ of services makes it easy to test
* Services can be debugged as _individual autonomous entities_
  * Best regards from functional programming!

---

## And what about Serverless?

* These considerations still apply:
  * Structural aspects
  * Communication
* Per platform, choices are made for us in order to save work

  * Communication
  * Deployment
  * General service environment

* Some aspects, like testing and debugging, get way more complicated...

* Serverless is Microservices taken to extremes &mdash; but also without some of the benefits!

---

## Sources

* This presentation:

  * https://oliversturm.github.io/microservices-complete-picture
  * PDF download: <br>https://oliversturm.github.io/microservices-complete-picture/slides.pdf

* Demo code:

  * https://github.com/oliversturm/cqrs-grid-demo (check _master_ and _event-sourcing_ branches)

---

class: impact

# Thank You

Please feel free to contact me about the content anytime.

.title-oli[
Oliver Sturm &bull; @olivers &bull; oliver@oliversturm.com
]

.title-logo[
<img src="template/devexpress.png" id="devexpress" alt="DevExpress"><img src="template/mvp.png" id="mvp" alt="MVP">
]
