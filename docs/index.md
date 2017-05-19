# Kalastatic

Kalastatic is a prototyping framework.

It can be (and has been) used to build beautifully crafted static sites at [Kalamuna](http://www.kalamuna.com).

However, its primary purpose is to put into practice atomic web design principles to produce a living styleguide/component library that can be used to guide back-end implementations in a framework agnostic approach.

Kalastatic integrates tightly with Drupal 7 and 8, effectively sharing twig templates between the styleguide and the CMS.

It serves as a point of convergence between front-end development, back-end development, and content strategy. Ultimately it facilitates putting design first, and this in front users for testing, and stakeholders for meaningful and timely feedback.


## Overview

## Benefits
### Stakeholders
#### Clients
- Small uncertainties in communication get ironed out much earlier/
- I don't want to see a generically styled, broken dev site for the first few weeks of a project.
- Real, demonstrable progress, earlier than before.
- Many concerns can be addressed during the project, instead of waiting for certain milestones.
- Whole process becomes more participator.

#### Agency, PMs, Account Managers
- The client never sees a barebones generic site, during demos.
- From first contact, their branding, typography and colors are in place. This avoids uncertainty, stress, and eucation on my part.
- Questions around specifics arise much earlier in the process.

#### User Experience
- We can test assumptions earlier.
- We can put our designs and patterns in front of Stakeholders and Clients earlier in the process.
- We can "show not tell" more effectively.
- Easier to communicate with stakeholders about abstractions.

#### Frontend Dev
- Can work in tools commonly used in the trade.
- Now in control of markup, as opposed to working around it.
- Can be involved earlier, and stick around later in the process.
- We begin working through responsive issues as soon as we begin styleguiding, this results in more successful first passes, less suprises, and better decisions about our responsive/adaptive patterns.

#### Content Strategist
- Doesn't have to wait for the CMS to be in place to see content in-situ.
- Git and markdown is still a real challange in this case.

#### Backend developers
- Component Documentation
- Json mock data tells me what needs to be made available to templates


## Features

### Styleguide

#### What's a styleguide?

A web Styleguide offer a way of ensuring consistency between brand, design and code.
Herein we are looking documenting every component and its code on the site in one place to ensure "same-pagey" communications between designers, front end developers and developers.

The pattern portfolio expresses every component and layout structures throughout the site.
It articulates the atomic design structure, and is used to illustrate the project’s shared vocabulary.

#### Our Styleguide

A statement about styleguides serving both as pattern library, but also useful as brand styleguide, to ensure consistency and conformancy in the use of brand assets.

Kalastatic uses [node-kss](https://github.com/kss-node/kss-node) as the basis for it's styleguide.

To acheive some larger goals beyond documentating component design patterns, namely providing brand-style and usage documentation Kalastatic uses  the [KSTAT-KSS-Builder](https://github.com/kalamuna/kstat-kss-builder) to generate the styleguide, which extends some of the documenation features, making better suited for documenting colors, and other brand-related style concerns.

The hope is to both house a component library while also providing a decent brand-guide experience.

### Prototype

To provide working, responsive prototypes, we use [metalsmith](metalsmith.io) and a bevvy of [other tools](https://github.com/kalamuna/kalastatic/blob/master/package.json)

Prototyping is most useful to consider the components with layouts, side by site with other elements. Where the styleguide documents components in isolation, prototyping helps us see all the bits in context, and even develop behaviors (js) and other integrations, before we dive into CMSs and app-frameworks.