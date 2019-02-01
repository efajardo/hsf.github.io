---
title: Evaluation of scalability of protocols to serve data for jobs for LIGO/Collaboration
layout: gsoc_proposal
project: HTCondor
year: 2019
organization: UCSD
---

## Description

The LIGO experiment is adopting the use of GlideinWMS, a distributed resource manager, for its computing needs. Currently, passing input data to the parallel jobs is accomplished via either HTCondor-based file transfer or downloading from a set of Xrootd-powered distributed caches. Past work has been done on testing the scalability of these transfer methods, but not in the context of the needs of the LIGO experiment. We will attempt to test at what concurrency levels different components of the GlideinWMS infrastructure break while keeping conditions aligned to the needs of the LIGO experiment. 


## Task ideas
 * Replicate the tests of the HTCondor transfer method that were done for GlueX [1].
 * Use glideTester to evaluate the usage of a Cache, a set of caches with/without SSD up to 5000 parallel jobs.
 * Combine the results of both and submit an abstract for CHEP Conference 2019.

## Expected results
Obtain conlcusive results on the current limitations of hardwared and software to support concurrency levels up to a five thousand jobs uploading or downloading data at different read and write speeds. 

## Requirements
Python, HTCondor (desirable)

## Mentors
  * [Edgar Fajardo](mailto:emfajard@ucsd.edu)
  * [Igor Sfiligoi](mailto:isfiligoi@sdsc.edu)
  * [Frank Wuerthwein](mailto:fkw@ucsd.edu)

## Links
  * [HTCondor](http://research.cs.wisc.edu/htcondor/)
  * [Limits of HTCondor Transfer System | https://indico.cern.ch/event/587955/contributions/2937378/contribution.pdf]

