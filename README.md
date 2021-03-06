sys-proctree
============

Discovers and lays waste to process trees on various operating systems.

Guide
-----

* gem install sys-proctree

```ruby
    require 'sys/proctree'

    ::Sys::ProcTree.find(2134) # Returns an array containing pids of the process tree whose root has pid 2134, children first

    ::Process.kill_tree(9, 2134) # Kills all processes in the tree of pid 2134 using kill signal 9
```

Dependencies
------------

Uses sys-proctable to discover process trees.  See sys-proctable for supported operating systems.

Requirements
------------

* Ruby 1.9

Build Status
------------

[![Build Status](https://travis-ci.org/MYOB-Technology/sys-proctree.png)](https://travis-ci.org/MYOB-Technology/sys-proctree)
