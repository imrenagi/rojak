# Rojak

Rojak is a **non-profit** and open source project used for observing online news
website in any election in Indonesia. It could be presidential, governor, or
even major election. The project was initialized first time in October 2016 [here](https://github.com/pyk/rojak) to observe 2017 governor election in DKI
Jakarta.

## Why is Rojak?

In the very long run of an public election, people tend to get informations about
the election candidate from the online news site. Unfortunately, some of the news
online tend to  take a side in one of particular candidate. This makes bias to
some/all of the informations published on that online news. It could give
positive impact for a candidate they take the side with, or even bad impact to
another candidate. As the consequences, there might be some resentments and  various
disputes in the community that are ultimately very difficult to resolve.

By developing this project, we have huge hope that the citizen will get prior
general knowledge about how any particular media creates stories and takes a
side in an election. In addition, this project is also able to be more more subtle
and not easy to be provoked.

## Main Features

For the first major release, this project will provide the following functionalities:
* **Sentiment analytics** from all online news sites to all candidates in an election.

## System Architecture

There are 4 main applications running for this project. They are:
* Rojak Frontend Web
* Rojak API
* Rojak Pantau
* Pub/Sub Application. This might gonna be Kafka/Redis/GCP Pubsub.

![New Architecture](./new-architecture.jpg)

## How to contribute

This application consists of 3 main parts and each part will have its own github
repositories. They are `rojak-pantau` (includes crawler and machine learning),
`rojak-api` (RESTful API server built by Spring Boot and Spring Cloud) and
`rojak-web-frontend` (built by ReactJs).

To contribute, please create Pull Request from specific git repositories, instead of
to this repository. FYI, each project will have list of TODO's located on
`Project` tab in each repository. If you are interested in one of the task given
there, please convert the task into an issue and assign the issue to yourself.

When you made pull request, please specify which issue that the PR referred to.
Please check [this](https://github.com/blog/1506-closing-issues-via-pull-requests)
following article to get more information about how to do so.
