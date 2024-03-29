---
date: 2019-02-22
title: "Week 29: Create a team"
author: Paul Fawkesley
open_graph_type: "article"
open_graph_image: "images/2019-02-22-fk-team-create-static.png"
---
**Protecting liberty by simplifying security**

_Recap_: Fluidkeys makes PGP simple for engineering teams. It helps you safeguard your source code
and protect passwords, secrets and personal data.

## The short version

* We built `fk team create` to bootstrap a team
* We improved error handling in Mojave (macOS)
* We've decided on a non-profit structure!

## We built `fk team create` to bootstrap a team

Wow, what a week. Since we [publicly committed](/#roadmap) to a date for our first teams release,
we've been setting tough weekly goals.

We didn't *quite* define the full scope of the first teams release, partly because the feedback we
solicited is still rolling in, and partly because we were too focused on building...

This week we built an MVP version of `fk team create` which lets you start defining a team.

Ian went to town on making it help you out by looking in gpg for existing keys you might have for
your team. That makes it a little quicker to get started.

![A terminal animation showing creating a team in Fluidkeys.](/images/2019-02-22-fk-team-create.svg)

There's some important detail which makes teams harder than it sounds: teams are defined in a
cryptographically signed file that only *you* can modify.

The file is hosted in our server, but because a signature is required, it's technically impossible
for us to sneak an extra key into your team. Without access to your team admin's private key, we
can't create the signature required to change the team.

Of course, we have no plans to backdoor our customers, but we think it's important that the
technical design means you don't have to believe that.

We're calling this a *signed team roster* and we're grateful to Micah and co at First Look Media
for inspiring this approach with their
[Keylist / fingerprints.txt](https://datatracker.ietf.org/doc/draft-mccain-keylist/) standard.

## We improved error handling in Mojave (macOS)

We chose to use cron to run Fluidkeys regularly (for automatic key rotation) because it exists
on Linux and macOS. We understood that Apple advise against this (recommending instead to use
launchd) but at the time, a cross platform approach seemed the best compromise.

The macOS update Mojave introduced a new permissions model for any applications wanting to
modify a users's crontab.

![A prompt saying Terminal would like to administer your computer.](/images/2018-12-15-mojave-terminal-prompt.png)

It's a pretty brutal dialog, and understandably people aren't in a hurry to grant Fluidkeys access
to "administer your computer". Unfortunately, if people did click "Don't Allow", Fluidkeys would
blow up. Not good.

Now, just before that prompt comes up we hint *why* it's happening. And if the user denies access,
we tell them how to add Fluidkeys to their crontab manually:


![A screenshot of a terminal with an error message and instructions](/images/2019-02-19-failed-to-schedule-maintenance.png)

## We've decided on a non-profit structure!

Thanks to the support we're receiving from the
[Co-op Foundation](https://www.coopfoundation.org.uk/about.html) we had our second session with
[Adrian Ashton](https://www.adrianashton.co.uk/).

Adrian is helping us to explore what legal structure best fits our mission, our goals, our
outlook, how we want to be perceived, and so on.

After running through the homework he'd set us, we ruled out a number of structures.

The biggest surprise to us was that our position and narrative against mass surveillance is
likely to be too political for a charity or a community interest company. It would be awkward if
chose a structure which was incompatible with us running cryptoparties, participating in the
Internet Freedom Festival, supporting the Tor network, and so on.

We're happy to announce that we've decided to incoporate as a [Company Limited by
Guarantee.](https://en.wikipedia.org/wiki/Private_company_limited_by_guarantee)

We'll use our articles of association to enshrine three essential components, namely:

* Our social purpose (we'll nail this down in the next 2 weeks)
* An asset lock, protecting the things the company owns from being sold inappropriately
* Profit distribution: how we'll spend the majority of profit on furthering the social purpose.

Considering we spent 90 minutes talking about legal structures, we both emerged extremely positive
and fired up.

Forming a non-profit is a powerful way of signalling that our motivations are bigger than money. Or
in other words, putting our money where our mouth is :)

Adrian has been brilliant. If you're exploring social enterprises, consider this a strong
recommendation.

## Next week

Next week we will:

* Make the website reflect upcoming release (rolling in some of the
  [preview site](/fluidkeys-v1-preview)
* build an MVP invite, create and join flow


Thanks for getting this far!

— Paul

*All* feedback is welcome, pop us an email to
[hello@fluidkeys.com](mailto:hello@fluidkeys.com)
