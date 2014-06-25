force-unlink Cookbook
=====================

Minimal case to repro possible bug.

Template may be notifying a service restart before it has set permissions on the managed resource. This should setup the environment, and then explode if it is incorrect.

```
bundle install
bundle exec kitchen test
```
