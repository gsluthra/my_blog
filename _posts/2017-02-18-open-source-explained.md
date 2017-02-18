---
layout: post
last-modified: '2017-02-18T12:00:00+05:30'

title: "Understanding Open Source Software"
subtitle: "A Developers guide to understanding Open Source Software"
cover_image: general/orange-evening.jpg
cover_image_caption: "Near the Norbulingka Institute, Dharamshala, India"
og-image: "general/orange-evening.jpg"

excerpt: "In this blog I explain what Open Source Software (OSS) means, why does Open Source Software get built, a little
about licenses, and why developers should contribute to OSS."

author:
  name: Gurpreet Luthra
  twitter: _zenx_
  bio: Software Craftsman and Lead Consultant Developer at ThoughtWorks
  image: general/gp-square-v.jpg
---

## Just because the source code is available does not mean it is Open Source

Most people explain _Open Source Software_ as --- a software that has made its source code available publicly.
That is an incomplete and incorrect definition of the term _Open Source Software (OSS)_.

An Open Source software is software where the code is not only freely available to view, but also to
modify, and re-distribute, and has an associated License that allows for this to happen.
This is how Wikipedia defines [Open Source Software (OSS)](https://en.wikipedia.org/wiki/Open-source_software):

_Open-source software (OSS) is computer software with its source code made available with a license
in which the copyright holder provides the rights to study, change, and distribute the software to anyone
and for any purpose._

Irrespective of the OSS License being applied, the above conditions should be true for a software to call
itself Open Source.

A more precise, easy-to-understand and widely referenced definition of Open Source Software is maintained
 and managed by the Open Source Initiative (OSI) on this page: [Open Source Definition](https://opensource.org/osd-annotated). It mentions 10 criteria that should be satisfied by the distribution terms of the sofware license for it to be accepted as Open Source.

## So then what is the deal with the different licenses -- GPL, MPL, Apache, etc?

**Note:** _I am not a lawyer. Please consult a qualified lawyer when you are inspecting / figuring out an OSS License for your company / software. My advice here is informal._

There are many OSS Licenses publicly recognized and available to make it convenient for you to use the one that suits your needs the most. The Open Source Initiative (OSI) maintains a [list of approved licenses here](https://opensource.org/licenses/alphabetical) for your to choose from.

All these licenses are recognized as Open Source Licenses, and hence should provide the same freedom as mentioned above while explaining what does OSS mean -- but there are some things about them you need to know.

For instance, some licenses can be [viral in nature](https://en.wikipedia.org/wiki/Viral_license), like the GPL license. If you use a GPL Licensed software library in your software you will have to make your own software freely available under the GPL License. Obviously, if you are a commercial, proprietary software developer you **DO NOT** want to do that to your proprietary software!  Do check out: [Can I use GPL software in a commerical application?](https://softwareengineering.stackexchange.com/questions/47032/can-i-use-gpl-software-in-a-commercial-application) As an example -- iText is a library for generating PDFs which provides it sofware under AGPL license (free) and also a commerical license (paid). You will not be able to use its free version for commercial software for the same reasons articulated above. Read about [iText License implications here](http://itextpdf.com/legal).

An interesting related article: [The Decline of GPL?](https://opensource.com/article/17/2/decline-gpl)

**Important Notes**:

1. _I work on an open source hospital system called [Bahmni](http://bahmni.org), for low-resource environments. This software is licensed under AGPL license, for good reasons. We would like that any paid development done for Bahmni is made available to all for free! The software is meant to benefit humanity, and not for making shit loads of money -- like many EMR vendors seem to have done! [Read more about the problems here](http://www.openhealthnews.com/blogs/ramaduro/2017-01-19/obama-and-biden-blast-ehr-vendors-data-blocking)._
2. _Linux is licensed under GPLv2. For good reasons again. From this [article](http://www.zdnet.com/article/linus-torvaldss-love-hate-relationship-with-the-gpl/), Linus Torvalds says: "The GPL ensures that nobody is ever going to take advantage of your code. It will remain free and nobody can take that away from you. I think that's a big deal for community management."_
3. _Do you know the differences between Red Hat Enterprise Linux RHEL (paid) and CentOS Linux (free)? You might be surprised to know that the code of CentOS Linux is created from RHEL source code with all Red Hat trademark information removed -- because Red Hat invests/pays for the trademark and logo, but the underlying Linux and its modifications are required to be made freely available as source code -- which allows the creation of CentOS. This is why so many companies use CentOS -- because they believe they get the same quality for free! Amazing. Isn't it? Read more [here: Wikipedia/CentOS](https://en.wikipedia.org/wiki/CentOS) and [here: Wikipedia/RedHatDerivatives](https://en.wikipedia.org/wiki/Red_Hat_Enterprise_Linux_derivatives)._

But most OSS would like people to adopt them widely, especially software platforms and libraries -- because the wider the adoption of a software, the more chances are that its bugs will surface quicker, it will become more stable, it will have more impact, and more people will contribute to it. Once a company or a team invests in a software stack, its unlikely that they would want to throw it away on the slightest excuse! This is why many Open Source Softwares choose a more liberal license which allows you to ship and use them in commercial packages. Think of [Angular.js](https://github.com/angular/angular.js/blob/master/LICENSE), [React.js](http://react-etc.net/entry/your-license-to-use-react-js-can-be-revoked-if-you-compete-with-facebook), [Postgres](https://www.postgresql.org/about/licence/), [Spring Framework](https://en.wikipedia.org/wiki/Spring_Framework), [Ruby Language](https://www.ruby-lang.org/en/about/license.txt), [jQuery](https://github.com/jquery/jquery/blob/master/LICENSE.txt), [Tomcat Server and other softwares from Apache](https://tomcat.apache.org/legal.html), [Nginx](https://en.wikipedia.org/wiki/Nginx), [Selenium Test Framework](https://en.wikipedia.org/wiki/Selenium_(software)), [jUnit](https://en.wikipedia.org/wiki/JUnit) and many other softwares & libraries & tools which we all use in proprietary softwares -- are all Open Source! They are licensed in a manner that allows others to benefit off them. Isn't that awesome! So -- have you given them back something? Have you helped making them better or popular?

**A note on React.js**: _I just got to know that apparently, Facebook has the rights to revoke your license to use React.js, if it feels that your software application competes with Facebook. Really?! Wow! [Read more about this here](http://react-etc.net/entry/your-license-to-use-react-js-can-be-revoked-if-you-compete-with-facebook). Can someone confirm this is true? I think the update says this is not true. But worth confirming._

## So do people make any money with Open Source Softwares?

Yes. A lot of companies and people make money with Open Source Software. There are [15+ business models with OSS](https://en.wikipedia.org/wiki/Business_models_for_open-source_software) mentioned on Wikipedia. The obvious ones are Support and Professional Services around the software package, but people can do a lot more including writing paid add-ons, software-as-a-service, advertisements, trainings, etc. And some softwares become more successful after they become open source. For instance, read this article: [Why Microsoft is turning into an Open Source company](http://www.zdnet.com/article/why-microsoft-is-turning-into-an-open-source-company/). The author says: _"Open source has become the dominant development paradigm. While people used to talk about open source and free software in terms of religion or cancer, depending on which side you were on, the real reason open source has won is that it makes **hard financial sense**."_

## OK. Open Source Rocks! Now what do I do?

If you are a developer, a QA, a BA, a technologist -- you have very little excuse to not be involved in some Open Source Software. Why should you limit your exposure, experience and learnings to _only_ the project you are on? Why not contribute and learn from the zillions of OSS that are out there. Most of these softwares are looking for technical contributions and to make greater impact.

Pick a topic that you love. Or a software you would be interested in. Do you like Security, Music, Medicine, Programming Languages, Painting, Maths, Teaching, Kids, Criminology, Guitar, Sports, Gym, FILL-IN-THE-BLANKS? Find an OSS in your chosen area, whatever motivates you, and jump in. Projects need help on everything under the sun -- from developing small/large features, to writing unit/integration/functional tests, to setting up CI/CD servers, to documentation, to creating stories, to fixing bugs, to creating presentations, to publishing videos, to organizing events, to evaluating libraries, to helping in rollouts and implementations of their softwares, to.... you get it. Whatever you do in your orgnaization on your project; the OSS also needs that to be done.
Plus, you can be a QA contributing to Development tasks, or a Dev contributing to recoding videos, and so on.. because no one cares what "role" you come from -- its what you want to do!

Most OSS projects will have a chatroom on IRC/Slack/etc, a mailing list, a public version control repository (likely Github), a public task management system (like JIRA, Github Issues, Trello, etc), and periodic virtual meetings. If you go in with sincerity, and resolve --- your work will be highly appreciated.


## A list of Open Source Projects you might consider

A short list of suggestions from my side. It's a drop in the ocean. The important thing is to "want" to contribute to the one you choose. Find your holy grail.

- [Bahmni](http://bahmni.org): Open Source EMR & Hospital System (or [OpenMRS](http://openmrs.org))
- [Pixelated](https://pixelated-project.org/): Encrypted/Private/Secure Web based email
- [Moodle](https://moodle.org/): Free Learning Management System
- [KeepassX](https://github.com/keepassx/keepassx): Cross platform Password Manager
- [BugZilla](https://www.bugzilla.org/): Task Management and Issue Management System
- [Ushahidi](https://www.ushahidi.com/): Real time, croud-sourced crisis management and mapping tool
- [Audactiy](https://github.com/audacity/audacity): Digital Audio Editor
- [Wikipedia/List of Open Source Softwares](https://en.wikipedia.org/wiki/List_of_free_and_open-source_software_packages): Huge list of Open Source softwares by category


The Open Source Software movement is big.
It's time to jump in. Give back. Learn. Soak. And be part of alternative communities, across multiple countries. Believe me -- you will be welcomed.