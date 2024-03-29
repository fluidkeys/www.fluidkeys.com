---
date: 2019-01-11
title: "Week 23: Telling the world about encrypted secrets"
author: Paul Fawkesley
---
**Protecting liberty by simplifying security**

_Recap_: We’re building Fluidkeys, to help you easily send end-to-end encrypted secrets using PGP.

Using Fluidkeys reduces the impact of third-party data breaches, targeted spearphishing attacks and network compromise.

Hope you had a good break!

Some exciting news: we're now part of the Federation, a community built on ethical values.

## The short version:

* We've been accepted into The Federation community!
* We properly announced v0.3
* Enjoyed the front page of Hackernews!

## Joining The Federation

The Federation is close to our hearts as we saw it being born when we were working together at the Co-op in Manchester.

> A community of digital businesses and innovators in Manchester, built on ethical values.

A few months ago we applied for membership and part-time desk space in the co-working space as we wanted to be part of an optimistic network of social entrepreneurs.

We're happy to announce that, thanks to a grant from Luminate, The Federation and Co-op Foundation are funding part-time desk space and membership for us.

In return, we have to formalise as a social enterprise and continue to focus on human rights as the bigger part of our mission. This is exactly what we want to do, so it's exciting being held to it!

On Wednesday I hopped across to Manchester to introduce Fluidkeys and meet the other grantees.

Trying to explain Fluidkeys in 5 minutes was a challenge! I'm going to practise this.

## Announced 0.3

Releasing at 5pm on the Friday before Christmas probably wasn't the nicest approach, but it was good to have it done, though we had no time to actually write about it.

This week we put out a [proper release note](https://www.fluidkeys.com/blog/release-0-3-send-encrypted-secrets/) describing Fluidkeys 0.3 and how you can send encrypted secrets from the command-line.

## Enjoyed the front page of Hackernews!

Hackernews is a strange beast. I submitted the release note on Tuesday and got barely a peep all day. I was feeling a bit disheartened, that nobody was interested in encrypted secrets.

Come Wednesday afternoon though, I got an alert that we'd been mentioned on Twitter by a "Hackernews front page" bot. Action stations!

Once on the front page, things change fast. We got a lot of visitors, downloads, emails and signups to our release notes. Other sites start syndicating which boosts the numbers too.

There was a [fair bit of discussion](https://news.ycombinator.com/item?id=18863528) too which was insightful.

A couple of observations from the comments:

* [Magic Wormhole](https://magic-wormhole.readthedocs.io) is a lovely tool for sending end-to-end encrypted secrets from the command line. If we frame Fluidkeys as "send encrypted secrets" then it's unclear why you'd use Fluidkeys over Wormhole: fair enough.

* It's unclear how Fluidkeys is different from Keybase (this is supported by calls we've taken ourselves):

>  How does this compare to keybase?

>  Also had the same question. :)

>  To be honest this just seems like an insecure version of Keybase.

> We (and everyone else I know that uses Keybase) use it for passing around sensitive information, either through chat, their encrypted Git repos, encrypted messages plopped into emails, etc.

* Multiple people have scripted their own workarounds for sending encrypted secrets. This is generally a good sign: this problem exists.

* Just sending secrets probably isn't valuable enough to charge for (though we'll start validating this ourselves). [This comment](https://news.ycombinator.com/reply?id=18876709&goto=item%3Fid%3D18863528%2318876709) elaborated:

> Without sugar-coating it - a service like this, with the scope it has now, has * zero * chance of successful monetization. 100% guaranteed.
> This is a cosmetic service that aims to address a security need. People who actually need this AND have money to pay for it are in position to explore self-hosted options, which is what they will be looking for in the first place since they DO want proper security. Having a random third party in their security pipeline is not really an option. And people who are not concerned with this part, won't think twice about sending API keys over regular email. In fact, even security-minded people won't have much objection to relaying secrets through their corporate, properly secured email server.

This is all good, rich feedback. This is exactly why we like working in the open and releasing often!

— Paul

*All* feedback is welcome, pop us an email to
[hello@fluidkeys.com](mailto:hello@fluidkeys.com)
