---
layout: post
title: Why Your Business Needs Devops
date:   2019-04-18 08:43:59
author: Christopher Timberlake
categories: editorials
disqus_disabled: false
---

* *Disclaimer: I have worked with airlines, Nothing in this article is confidential. Some of these things are common sense. *

### Introduction

Recently I was watching a video titled [How Airlines Decide Where To Fly](https://www.youtube.com/watch?v=E3jfvncofiA) by Wendover Productions. He dives into the topic and glosses over the topic. He explains to a lay-person how this is done; However I'd like to answer it differently.

## How Do Airlines Decide Where To Fly? Answer: Dev-Ops.

### The Problem
In the Youtube video linked above; They go over the topic of knowing where travelers are going from Point A to Point Z and instead have to go to Point B and Point C before hitting Z. Airlines have a lot of data about their travellers and where their planes go and how full they are.

The truth is much deeper than that. Airlines, can and should track all data. *Wait Chris, All data?* Yes, All data. Not only are their travellers going from Point A to Point Z, But they're taking a plane. That plane which is succeptible to turbulence, thermal turbulence, weather, delays, and maintenance concerns. 

Asking a question such as *Which routes are going to be profitable in 2020?* seems like such a simple question. However the reality of this is it's a question without an answer. You can only provide a best-case answer with the data you have on hand. 

Ever have one of those math questions about how if a train leaves Station A.. You get where i'm going with this. It's one of those questions. If a 787 leaves LAS at 7:45 PM on a Friday and travels to JFK. Is it profitable? What about if it leaves at 7:30 PM, Is it more or less profitable? 

To answer this question you have to calculate (revenue - costs). However costs is a consistantly moving target. Specially with climate change. If it's now 2 degrees warmer in Las Vegas, that means more fuel burn on take-off and landings due to a flatter climb. That 2 degrees difference could also result in thermal turbulence that causes a plane to utilize more fuel. Now we have a new calculation for fuel costs. Fuel Cost = (Lbs Used * Fuel Price) at 7:45 PM, versus 7:30 PM. 

These types of calculations go into the thousands of variables. What if we put a 400lb Person into Seat 15A versus Seat 26B. How does this affect the balance of the plane in flight, and thus does it result in a fuel cost increase or decrease?

### The Solution
Gathering and storing all of this data takes tons of storage. Processing all of this data takes tons of processes and servers. But what happens when you're not needing to process the data? Do you just have millions of dollars in servers just chilling on a rack somewhere?

No, You use DevOps to dynamically scale up and down your servers and processes. You gather tons of data, and provision more storage as you need it. Then run your applications to analyze this data and do tens of thousands if not millions of calculations to get the answers you need out of it. These applications take in all the variables and will answer what the cost of a 400lb person in Seat 15A versus Seat 26B will be. They'll also tell you the fuel cost when leaving LAS at different times. Correlating that data with what your customers wants and their behaviors.

Resulting in a beautiful graph that allows you to determine the outcome of numerous actions.

**But wait, There's a problem with my calculation. ALL CALCULATIONS ARE WRONG**

Yeah, That happens a lot. Following proper DevOps practices you're probably running something like GitLab and Kubernetes. GitLab allows you to make code changes quickly and compile them. Allowing you to get fixes in your application out quickly. Kubernetes allows you to schedule your application on multiple servers at once. To take advantage of that power. 

You can roll out your fixes at scale, and quicker than any other way. That means instead of going through a change request process, you can submit your application and if it meets the criteria, Then it ships and produces those calculations. Saving hours, maybe weeks for an answer.

### The Cost

Oh, you thought DevOps was more expensive. No, it's cheaper. Because once you've got these calculations. You *destroy everything* freeing up those servers and storage clusters for other uses. Then when you need to do another round of calculations. By following DevOps Practices you can use Infrastructure as Code to scale everything else up.

** One of the key tenants of a successful business isn't just having a compelling product. But bringing changes and iterations to products, or entirely new products to market before the competition. So, how much is not doing DevOps costing you? **
