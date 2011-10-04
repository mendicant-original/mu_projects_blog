---
layout: post
title: "List of Documentation Needs for MRI"
---

Many modules in Ruby lack a basic top-level description of what they do. In many cases, this is a relatively easy task to do. What is needed is one or two paragraphs of description, and a couple of realistic examples of its use.

## Example of well documented classes

  - [OpenSSL](https://github.com/rmu/ruby/blob/trunk/ext/openssl/ossl.c#L418-790)
  - [BasicObject](https://github.com/rmu/ruby/blob/trunk/object.c#L2618-2669)

## Classes/Modules which lack documentation

  -  Debug
  -  Encoding
  -  Fiddle
  -  IRB*
  -  Mkmf
  -  Monitor::MonitorMixin
  -  Mutex_m
  -  Profile, Profiler
  -  Random
  -  Range
  -  RbConfig
  -  RSS
  -  Shell
  -  Thread

## Classes/Modules with poor documentation

  - ARGF
  - Array
  - CMath need clarifications (Complex is now in core, what does it do now?)
  - Digest: no examples (Digest::MD5 is not even in the class list)
  - Enumerable
  - Etc
  - Float
  - Hash
  - PTY
  - Racc
  - Rinda
  - Sync, Sync_m
  - Time
  - ZLib

## More specialized things

  - initialize_copy
  - Object#hash


## Some other tips for finding areas to document

  - Look near `Init_<class name>` in `<class_name>.c`

  - [List of class-level documentation by byte length](https://gist.github.com/1254953). Low numbers don't necessarily mean poor documentation, but if you see a much-used class low on the list, it may be a candidate for improvement. 

