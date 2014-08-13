bholmes-scratchpad
==================

Ben Holmes' Scratchpad of stuff

* OpenShift Load Test

  A fairly basic test harness which, to use a technical term, hammers your OpenShift gear with upto 7,500 concurrent HTTP requests over a period of 5 mins. From a starting point of 1 gear, this should get you scaled upto at least 3 gears between 33-66% of the way through the test run. You can of course tailor the test to suit your projected request profile by changing the load test parameters.
  The application FQDN you're hitting is controlled by the 'application.url' property at the project level. Change this to match your application, open up the Load Test, and press play.
  Once the test completes (and assuming no other hogh-load requests are currently in-flight) you should see your application scale back after a few minutes of quiet time. 
  
  
* Nginx from SCL
  
  An Nginx cartridge for OpenShift Enterprise, pulling from Software Collections.
  
  
* SpringBoot
  
  A SpringBoot cartridge for OpenShift, which also provides the spring-boot-cli tools.