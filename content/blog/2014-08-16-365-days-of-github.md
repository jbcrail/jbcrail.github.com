+++
title = "365 Days of GitHub"
aliases = [
    "/2014/08/16/365-days-of-github/"
]
taxonomies.tags = [
    "github",
]
+++

> A man who can't bear to share his habits is a man who needs to quit them.
> ― Stephen King, The Dark Tower

It started off as a simple challenge to refamiliarize myself with areas
I rarely cover in my day job.  Inspired by the previous works of
[John Resig](http://ejohn.org/blog/write-code-every-day/),
[Ryan Seys](http://ryanseys.com/blog/177-days-of-github/), and
[Geoff Greer](http://geoff.greer.fm/2014/01/06/365-days-of-github/), my daily
habit snowballed into 20,000+ lines of code, 12 programming languages,
11 merged pull requests, and 8 new repositories.

The final body of work includes solutions to [Project Euler](https://projecteuler.net/),
a [RESTful content-addressable storage server](https://github.com/jbcrail/cas),
a [proxy for local and remote filesystems](https://github.com/jbcrail/fsproxy),
a [LINQ-inspired shell](https://github.com/jbcrail/crash),
a [simple performance monitor](https://github.com/jbcrail/quidnuncd),
a beanstalkd [library](https://github.com/jbcrail/beanstalk-rs),
a [library](https://github.com/jbcrail/vindinium-starter-erlang) for writing an
AI bot for [Vindinium](http://vindinium.org/), and documentation for
[Rust](https://github.com/rust-lang/rust). Other minor projects included a
[visualization of local crime data](http://bl.ocks.org/jbcrail/928bfd1882df644e0ba1)
and a [script](https://gist.github.com/jbcrail/8232863) that plots the intensity
of accelerometer values from a Wiimote.

### Unintended effects

After writing a non-trivial amount of code in a dozen languages, I've developed a
feel for which programming language concepts and syntax are better suited for
certain domains, especially the mathematical and performance-critical space
inhabited by Project Euler.

When tackling a new problem, Clojure and Python were essential for testing out
potential solutions in small incremental steps. Both are armed with a REPL, good
libraries, and a dynamic type system. I solved many problems without worrying
about the total run time of each solution.

As the problems increased in space and time complexity, I typically switched over
to Go and Rust in order to find a solution in a reasonable amount of time. Both
languages balance the need for performance and quick development without getting
sidelined by too much boilerplate or scaffolding. Even though this doesn't matter
as much for personal projects, I especially like the attention and thought put
into Go's and Rust's development tools.

When looking back, I continuously found myself using pattern matching, list
comprehensions, guards, closures, type inference, and traits. These features
mapped well to mathematical domains, but readable yet compact code was a fortunate
side-effect.

### Lies, damned lies, and statistics

Due to the breadth of the implementations, my Project Euler solutions turned into
a mini programming language shootout. The following table shows only lines of
code and relative expressiveness of each language (as represented by the __LOC Per
Problem__ column). I do have run time performance statistics, but it didn't seem
fair to publish the data until I reduced the startup cost for certain languages.
I will say that Go, Rust, SML, and Haskell were very competitive with C++.

| Language | Lines of Code (LOC) | Solved Problems | LOC Per Problem |
|----------|---------------------|-----------------|-----------------|
| Haskell  | 505                 | 37              | 13.6486         |
| Scala    | 333                 | 24              | 13.875          |
| Clojure  | 1318                | 71              | 18.5634         |
| Ruby     | 1443                | 73              | 19.7671         |
| SML      | 264                 | 12              | 22              |
| Python   | 1828                | 82              | 22.2927         |
| Erlang   | 1083                | 48              | 22.5625         |
| PHP      | 1378                | 56              | 24.6071         |
| Java     | 2005                | 62              | 32.3387         |
| Rust     | 2420                | 72              | 33.6111         |
| C++      | 2528                | 73              | 34.6301         |
| Go       | 3004                | 82              | 36.6341         |

### So what's next?

I'm not exactly sure. The daily act of committing code is ingrained at this
point so I'll probably continue for the forseeable future. As noted by others
who have undertaken similar challenges, the benefits have far outweighed
any downsides.
