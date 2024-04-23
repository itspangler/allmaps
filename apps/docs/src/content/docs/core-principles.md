---
title: Core Principles
description: ''
---

## Principle I: Open data in, open data out

Allmaps uses open data to make open data. Following [FAIR data principles](https://www.go-fair.org/fair-principles), the Allmaps Project defines "open data" as data that is findable, accessible, interoperable, and reusable. Making it easy to create, curate, and update spatial data for georeferencing maps---and making sure that data is stored in an open, easily interchangeable format---guides all aspects of how the Allmaps ecosystem operates.

### Spatial data

In Allmaps, the *input data* is always **structured metadata about a map**. Allmaps works by parsing [IIIF manifests](https://iiif.io/api/content-state/1.0/) and displaying their contents in a viewer. In this viewer, users can create and view georeferenced maps.

> Should we include an example of input data here? e.g., a IIIF manifest?

The *output data* are **georeference annotations**, or JSON files that store information about how a map should be georeferenced according to the [IIIF Georeference Extension](https://iiif.io/api/extension/georef/). At minimum, a georeference annotation contains two main components:

1. A **mask**, or a simple polygon that specifies which parts of a georeferenced map should be displayed (anything outside the mask will **not** be displayed)
2. A set of **ground control points** which associate pixel coordinates of a point in the input image with the geographic coordinates where they belong in the real world

> Should we include an example of output data, e.g. a georef annotation?

### User data

Users will never need to submit personal information in order to use Allmaps. However, some users may need advanced features, such as the ability to specify a version of a georeferenced map or manage a crowdsourced georeferencing project. In such cases, Allmaps securely collects and stores a **minimal amount** of user-submitted information in order to establish a `profile` entity in the Allmaps ecosystem.

There are two kinds of entities in the Allmaps ecosystem: `users` and `profiles`. A `user` is anyone who interacts with spatial data in Allmaps (e.g., creates or edits a georeference annotation), while a `profile` is anyone who has created an account for the Allmaps ecosystem.

To create an account, users voluntarily provide their email, a username, and a password. Allmaps securely stores this information in **how is this stored??** in accordance with the [GDPR](https://gdpr.eu/what-is-gdpr/). After creating an account, users with a `profile` can save and share collections of IIIF maps; specify thier "personal version" of georeferenced maps, including [content state views](https://iiif.io/api/content-state/1.0/); and administer georeferenced crowdsourcing projects.

> [See the Allmaps FAQs]() for more information on [how Allmaps stores data]() and our [commitment to making data sustainable]().

| Entity | Definition | What it can do | Application | 
| :-- | :-- | :-- | :-- |
| `user`    | Anyone who interacts with spatial data in the Allmaps ecosystem | Create and edit georeference annotations | Allmaps Editor, Allmaps Viewer |
| `profile` | Anyone who has created an account in the Allmaps ecosystem      | Save and share collections of IIIF maps; specify versions of maps; administer crowdsourced georeferencing projects. | Allmaps Curator |

## Principle II: Distributed, modular and interoperable

## Principle III: How is Allmaps organized?
