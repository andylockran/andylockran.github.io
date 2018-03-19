---
layout: post
title: DevSecOps?
date: 2018-03-19 20:00:00.000000000 +00:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- Social
- Technology
tags:
- aws
- dmz
- metadata
- networking
- routing
- devops
meta:
  _publicize_twitter_user: "@andylockran"
  _edit_last: '1'
  _wpas_done_all: '1'
  _gtm_vars: a:0:{}
  _wpas_skip_13286454: '1'
  _wpas_skip_9106205: '1'
author:
  login: andy
  email: andy@zrmt.com
  display_name: andylockran
  first_name: Andy
  last_name: Loughran
---

I consider that one of the most important aspects underwriting systems development is the ability to understand risk and probability.

In many lines of work you can be considered particularly unlucky should the 'stars align' and more than three simultaneous assumptions be undone to open up a path to disaster, but in DevOps and systems management, it's more than often the case that you're battling against most of your assumptions being wrong; not because of poor judgement, but because of the pace of change.

There are two ways to look at the problem, one is to slow things down and make sure everything is documented to the nth degree to reduce risk - but in my view that serves to create menial tasks that don't lend themselves directly to the business objectives.  Instead I advocate for a more lean approach, whereby the risks are documented in the code and dynamic checks (logs, tests .etc) are implemented to understand the shape of the risks.  The old mantra 'move fast and break things' also dies, with 'move fast and break things [but only for yourself]' - by testing your assumptions on off-master branches and reverting them should they be proven incorrect.

I also find that it's important to share with the wider team the ability to understand, break and resolve issues with the infrastructure.  Yes, they should get the support of the Systems experts when they need it - but you cannot have a DevOps culture without more people in the team being knowledgable about DevOps.  The team also need to be aware of the security implicatons of their decisions.  Lessons are learned far harder from your own mistakes, rather than those of others.  Allow more team members to make more, but less serious mistakes helps them learn faster on how to keep systems secure.

Finally, logging.  It's the forgotten child; the discarded penny, but it is also the diamond in the rough.  Immutable logs sent to a third party are an absolutely godsend in the event of any incident.  They provide assurances around what assumptions have been made, and can verify the integrity of a system as well as provide heuristics and a base for analysis as a system scales beyond the capability of individual analysis.  Loglevels, Syslog-NG (CloudWatch/CloudTrail on AWS) are relatively simple to learn but are an incredible weapon to have in your arsenal as a DevSecOps specialist.

For me, to be working in DevOps is to embrace DevSec ops.  If you're managing systems and security isn't at the top of your list then you're sleepwalking into a problem.