# Performance Testing Mindmap

Pull requests welcome

Table of Contents
=================

   * [Table of Contents](#table-of-contents)
      * [Mindmap](#mindmap)
      * [Legend](#legend)
      * [Backend Tools](#backend-tools)
         * [HTTP](#http)
         * [Multi-protocol](#multi-protocol)
         * [Cloud](#cloud)
         * [Low Level](#low-level)
         * [Frameworks](#frameworks)
         * [Database](#database)
         * [Other](#other)
      * [Frontend Tools](#frontend-tools)
         * [Cloud](#cloud-1)
      * [Web Links](#web-links)
         * [Where to Start](#where-to-start)
         * [Continuous Integration](#continuous-integration)
         * [Frontend Performance](#frontend-performance)
         * [Video Streaming](#video-streaming)
      * [Community](#community)
   * [Contributing](#contributing)
   * [License](#license)

## Mindmap
![Performance testing mindmap](images/performance_testing_mindmap.png)

Editor: [Xmind](http://www.xmind.net/)

## Legend
:moneybag: - Paid services, tools, etc.

## Backend Tools

### HTTP

* [Siege](https://www.joedog.org/siege-home/)
* [Apache Benchmark](https://httpd.apache.org/docs/2.4/programs/ab.html)
* [Boom!](https://github.com/tarekziade/boom)
	* [Break](https://github.com/tarekziade/break)
* [wrk](https://github.com/wg/wrk)
	* [WRK the HTTP benchmarking tool - Advanced Example](http://czerasz.com/2015/07/19/wrk-http-benchmarking-tool-example/)
* [Vegeta](https://github.com/tsenart/vegeta)
* [Gatling](https://gatling.io/)
* [httperf](https://github.com/httperf/httperf)
* [GoReplay](https://goreplay.org/)
* [weighttp](https://redmine.lighttpd.net/projects/weighttp/wiki)
* [httpress](https://bitbucket.org/yarosla/httpress/wiki/Home)
* [Web Polygraph](http://www.web-polygraph.org/)
* [Bees with Machine Guns!](https://github.com/newsapps/beeswithmachineguns)
* [k6](https://k6.io/)
* [Goad](https://github.com/goadapp/goad)
* [hurl](https://github.com/VerizonDigital/hurl)
* [autocannon](https://github.com/mcollina/autocannon)
* [Iago, A Load Generator](https://github.com/twitter/iago)

### Multi-protocol

* [Jmeter](http://jmeter.apache.org/)
    [Ruby-JMeter](https://github.com/flood-io/ruby-jmeter)
* [LoadRunner](http://www8.hp.com/pl/pl/software-solutions/loadrunner-load-testing/) :moneybag:
* [NeoLoad](https://www.neotys.com/neoload/overview) :moneybag:
* [LoadComplete](https://smartbear.com/product/loadcomplete/overview/) :moneybag:
* [Locust](http://locust.io/)
* [Tsung](http://tsung.erlang-projects.org/)
* [Grinder](http://grinder.sourceforge.net/)
    * [nGrinder](http://naver.github.io/ngrinder/)
* [SmartMeter.io](https://www.smartmeter.io/) :moneybag:
* [Artillery.io](https://artillery.io/)

### Cloud

* [Blazemeter](https://www.blazemeter.com/) :moneybag:
* [CloudTest](https://www.soasta.com/load-testing/) :moneybag:
* [flood IO](https://flood.io/) :moneybag:
* [Loader](https://loader.io/) :moneybag:
* [OctoPerf](https://octoperf.com/) :moneybag:
* [Loadmill](https://www.never-crash.com/) :moneybag:

### Low Level

* [stress-ng](https://github.com/ColinIanKing/stress-ng)
* [sysbench](https://github.com/akopytov/sysbench)
* [Phoronix Test Suite](https://www.phoronix-test-suite.com/)
    * [Phoromatic](https://www.phoronix-test-suite.com/?k=phoromatic)
* [OpenSSL Speed](https://www.openssl.org/docs/manmaster/man1/openssl-speed.html)
    * [NGINX SSL Performance](https://cdn.wp.nginx.com/wp-content/uploads/2014/07/NGINX-SSL-Performance.pdf) 
    * [Improving OpenSSL Performance - Intel](https://software.intel.com/en-us/articles/improving-openssl-performance)
* [TRex Realistic traffic generator](https://trex-tgn.cisco.com/)
* [Avalanche](https://www.spirent.com/Products/Avalanche) :moneybag:
* [hdparm -tT /dev/sda](https://linux.die.net/man/8/hdparm)
* [dd](https://linux.die.net/man/1/dd)
  * [How to use 'dd' to benchmark your disk or CPU?](https://romanrm.net/dd-benchmark)
  * Write
    * `dd bs=16k count=102400 oflag=direct if=/dev/zero of=test_data`
    * `dd bs=1M count=256 if=/dev/zero of=test conv=fdatasync`
  * Read
    * `dd bs=16K count=102400 iflag=direct if=test_data of=/dev/null`
* [Bonnie++](https://www.coker.com.au/bonnie++/)
    * [bonnie++(8) - Linux man page](https://linux.die.net/man/8/bonnie++)
* [hyperfine](https://github.com/sharkdp/hyperfine)

### Frameworks

* [Taurus](http://gettaurus.org/)
* [Pbench](https://github.com/distributed-system-analysis/pbench)
* [Multi-Mechanize](https://github.com/cgoldberg/multi-mechanize)
* [Zopkio](https://github.com/linkedin/Zopkio)
* [Funkload](https://github.com/nuxeo/FunkLoad)
* [Jagger](https://jagger.griddynamics.net/index.html)
* [airspeed velocity](http://asv.readthedocs.io/en/latest/)
* [Yandex Tank](https://github.com/yandex/yandex-tank)
* [PerfCake](http://perfcake.org/)
	* [PerfCake - a Lightweight Open Source Performance Testing Tool](http://www.methodsandtools.com/tools/perfcake.php)

### Database

* [dbstress](https://github.com/semberal/dbstress)
* [HammerDB](http://www.hammerdb.com/)
* [NdBench](https://github.com/Netflix/ndbench)
* [Yahoo! Cloud System Benchmark (YCSB)](https://github.com/brianfrankcooper/YCSB)
    * [Yahoo Cloud Serving Benchmark](https://research.yahoo.com/news/yahoo-cloud-serving-benchmark/)

### Other

* [Dynamometer](https://github.com/linkedin/dynamometer)

## Frontend Tools

* [Sitespeed.io](https://www.sitespeed.io/)
* [Lighthouse](https://developers.google.com/web/tools/lighthouse/)
* [YSlow command line](http://yslow.org/command-line-har/)
* [Test website performance with Puppeteer](https://michaljanaszek.com/blog/test-website-performance-with-puppeteer)
* [Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)
    * [Mobile-Friendly Test API for Node.js](https://github.com/denar90/mobile-friendly)
* [browser-perf](https://github.com/axemclion/browser-perf)
* [speed-demon](https://github.com/morsssss/speed-demon)

### Cloud
* [Webpagetest](https://www.webpagetest.org/)
    * [Private Instances](https://github.com/WPO-Foundation/webpagetest-docs/blob/master/user/Private%20Instances/README.md)
* [SpeedCurve](https://speedcurve.com/) :moneybag:
* [GTmetrix](https://gtmetrix.com/) :moneybag:
* [Pingdom](https://www.pingdom.com/) :moneybag:
* [DareBoost](https://www.dareboost.com) :moneybag:
* [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* [Google Mobile Website Speed Testing Tool](https://testmysite.withgoogle.com)
* [Website Speed Test](http://sitespeedtester.com/)
* [Website Speed Test - Cloudinary](https://webspeedtest.cloudinary.com/)
* [KeyCDN Website Speed Test](https://tools.keycdn.com/speed)
* [Site Relic](https://tools.geekflare.com/)
* [Treo](https://treo.sh/) :moneybag:
* [Calibre](https://calibreapp.com/) :moneybag:

## Web Links

### Where to Start

* [Performance Testing Guidance for Web Applications](https://msdn.microsoft.com/pl-pl/library/bb924375.aspx)
* [Performance Testing Checklist](http://www.seleniumtests.com/2016/02/performance-testing-checklist.html)
* [JMeter Tutorial for Load Testing – The ULTIMATE Guide](https://www.javacodegeeks.com/2014/11/jmeter-tutorial-load-testing.html)
* [High Performance Browser Networking](https://hpbn.co/)
* [3 best practices for container performance testing](https://techbeacon.com/3-best-practices-container-performance-testing)
* [Measure Performance with the RAIL Model](https://developers.google.com/web/fundamentals/performance/rail)
* [Using Avalanche vs. TRex to Simulate CDN and Attack Traffic](https://www.incapsula.com/blog/trex-traffic-generator-software.html)
* [Open Source Load Testing Tool Benchmarks V2](http://blog.loadimpact.com/open-source-load-testing-tool-benchmarks-v2)
* [A Quick Start Guide To Learning Performance Testing](https://dojo.ministryoftesting.com/lessons/a-quick-start-guide-to-learning-performance-testing)
* [Performance: which testing tool and why?](https://club.ministryoftesting.com/t/performance-which-testing-tool-and-why)
* [JMeter vs. Locust - Which One Should You Choose?](https://www.blazemeter.com/blog/jmeter-vs-locust-which-one-should-you-choose)
* [Elasticsearch Load Testing - Learn How](https://www.blazemeter.com/blog/elasticsearch-load-testing-learn-how)
* [HTTP Load Testing with Vegeta (and a dash of Python)](https://serialized.net/2017/06/load-testing-with-vegeta-and-python/)
* [Locust Assertions - A Complete User Manual](https://www.blazemeter.com/blog/locust-assertions-a-complete-user-manual)
* [Performance: Testing and Tuning - DZone's Guide](https://dzone.com/guides/performance-testing-and-tuning-1)
* [Keeping Node.js Fast: Tools, Techniques, And Tips For Making High-Performance Node.js Servers](https://www.smashingmagazine.com/2018/06/nodejs-tools-techniques-performance-servers/)

### Continuous Integration

* [Continuous Integration 101: How to Run JMeter With Jenkins](https://www.blazemeter.com/blog/continuous-integration-101-how-run-jmeter-jenkins)
* [Integrating Taurus with Jenkins](http://gettaurus.org/kb/Jenkins/)

### Frontend Performance

* [Measuring Wikipedia page load times](https://phabricator.wikimedia.org/phame/live/7/post/83/measuring_wikipedia_page_load_times/)
* [Rendering Metrics](https://speedcurve.com/blog/rendering-metrics/)
* [Front-End Performance Checklist 2018](https://www.smashingmagazine.com/2018/01/front-end-performance-checklist-2018-pdf-pages/)
* [The Cost Of JavaScript](https://medium.com/dev-channel/the-cost-of-javascript-84009f51e99e)
* [Web Performance Fundamentals: what is the Speed Index?](https://blog.dareboost.com/en/2018/02/speed-index-web-performance/)
* [A Beginner’s Guide to Website Speed Optimization](https://kinsta.com/learn/page-speed/)
* [Why Performance Matters](https://developers.google.com/web/fundamentals/performance/why-performance-matters/)
* [Measuring HTTP response times with cURL](https://ops.tips/gists/measuring-http-response-times-curl/)
	* [Analyze Your Website’s TTFB (Time to First Byte)](https://haydenjames.io/analyze-websites-ttfb-time-first-byte/)
* [Awesome WPO - A curated list of Web Performance Optimization](https://github.com/davidsonfellipe/awesome-wpo)
* [First Input Delay](https://developers.google.com/web/updates/2018/05/first-input-delay)

### Video Streaming

* [HLS | Video Streaming Performance Testing](https://www.swtestacademy.com/video-streaming-performance-testing/)

## Community
* [Jmeter users slack](https://jmeterusers.slack.com/)

# Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

# License

```
MIT License

Copyright (c) 2018 Maciej Gąsiorowski

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
