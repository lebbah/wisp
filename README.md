**Wisp** : **W**isp **I**s **S**cala **P**lotting is a console-centric plotting library for scala.
It focuses on existing web-based plotting libraries, and strives to bring the power and flexibility of web-based plotting
tools to the scala console, while preserving an at-your-finger-tips feel readily found in matlab, R, and many other languages.

<!---[![Build Status](https://travis-ci.org/quantifind/Wisp.svg?branch=master)](https://travis-ci.org/quantifind/Wisp)--->
<!---TODO: coverage--->

<!---Todo: logo--->

It is available on maven central. The alpha release of wisp is available as `0.0.1`. An sbt dependency would look like:

    "com.quantifind" %% "wisp" % "0.0.1"

<!---Todo: Integration with 3-rd party libraries: Highcharts, vega, etc. etc.?--->

## Usage

Full usage can be found on the [wiki](https://github.com/quantifind/wisp/wiki), but by means of example:

![Line Chart](https://github.com/quantifind/wisp/blob/master/images/line.png)

generated by

```
austin-2:wisp austin$ sbt 'project wisp' console
[info] Loading project definition from /Users/austin/IdeaProjects/wisp/project
[info] Set current project to wisp (in build file:/Users/austin/IdeaProjects/wisp/)
[info] Set current project to Wisp (in build file:/Users/austin/IdeaProjects/wisp/)
[info] Starting scala interpreter...
[info]
Welcome to Scala version 2.10.3 (Java HotSpot(TM) 64-Bit Server VM, Java 1.7.0_25).
Type in expressions to have them evaluated.
Type :help for more information.

scala> import com.qf.charts.repl.Highcharts._
import com.qf.charts.repl.Highcharts._

scala> line((1 to 10), (1 to 10))
serving resources from: file:/Users/austin/IdeaProjects/wisp/index-1418179288496.html
2014-12-09 18:41:29.188:INFO:oejs.Server:jetty-7.6.0.v20120127
2014-12-09 18:41:29.216:INFO:oejsh.ContextHandler:started o.e.j.s.ServletContextHandler{/,file:/Users/austin/IdeaProjects/wisp/index-1418179288496.html}
2014-12-09 18:41:29.225:INFO:oejs.AbstractConnector:Started SocketConnector@0.0.0.0:53495
Server started: http://172.20.10.2:53495/index-1418179288496.html
Output written to http://172.20.10.2:53495 (CMD + Click link in Mac OSX).
res0: com.qf.charts.highcharts.Highchart = Highchart(List(Series(Vector(Data(1,1,None,None), Data(2,2,None,None), Data(3,3,None,None), Data(4,4,None,None), Data(5,5,None,None), Data(6,6,None,None), Data(7,7,None,None), Data(8,8,None,None), Data(9,9,None,None), Data(10,10,None,None)),None,None,None,Some(line),None,None,None,None,series)),Some(Title(,None,None,None,None,None,None,None,title)),None,None,Some(Credits(None,,None,None,)),Some(Exporting(chart,None,None,None,None,None,None)),Some(Legend(None,None,None,Some(false),None,None,None,None,None,None,None,None,None,None,None,None,None,None,None,None,None)),None,true,None,None,Some([Lcom.qf.charts.highcharts.Axis;@40dc66ae))

scala>
```

<!---
## Builtin Help

Todo: repl help ? Reflect method names?
--->

## More Info

[Watch the introductory video](https://www.youtube.com/watch?v=LZH9rCEP-6w)

Greater detail can be found on the [wiki](https://github.com/quantifind/wisp/wiki)

Wisp is open source, and we hope to get involvement from the community.  We'd love to get some pull requests.  Also, even if you don't
have a fix, feel free to report bugs or just request new features through the [github issue tracker](https://github.com/quantifind/wisp/issues?state=open).

## Contributors

We would like to thank all of the engineers who helped make this possible

<table border="0">
  <tr>
    <td><a href=https://github.com/ajberglund >Andrew Berglund</a></td>
    <td>Original prototype, plot server</td>
  </tr>
    <tr>
    <td><a href=http://www.ee.calpoly.edu/faculty/adanowit/ >Andrew Danowitz</a></td>
    <td>Naming Wisp!</td>
  </tr>
    <tr>
    <td><a href=https://github.com/AustinBGibbons >Highcharts integration</a></td>
    <td>Original prototype, plot server</td>
  </tr>
    <tr>
    <td><a href=https://github.com/dadarakt >Jannis Eichborn</a></td>
    <td>Least squares regression</td>
  </tr>
    <tr>
    <td><a href=https://github.com/kthn >Karthik Thiyagarajan</a></td>
    <td>Json parsing</td>
  </tr>
    <tr>
    <td><a href=https://github.com/ajberglund >Pierre Andrews</a></td>
    <td><a href=http://unfiltered.databinder.net/Unfiltered.html >Unfiltered</a> support</td>
  </tr>
    <tr>
    <td><a href=https://github.com/ryanlecompte >Ryan LeCompte</a></td>
    <td>Type-Class wizardry</td>
  </tr>
</table>

and the entire [Quantifind](http://quantifind.com/) family for all their help in design, support, and execution!

## Contributing

Wisp is released under the Apache License and we **welcome any contributions** within this license. Any pull request is welcome and will be reviewed and merged as quickly as possible.

Because this open source project is released by [Quantifind](http://www.quantifind.com) as a company, if you want to submit a pull request, you will have to sign the following simple contributors agreement:
- If you are an individual, please sign [this contributors agreement](https://docs.google.com/a/quantifind.com/document/d/1RS7qEjq3cCmJ1665UhoCMK8541Ms7KyU3kVFoO4CR_I/) and send it back to contributors@quantifind.com
- If you are contributing changes that you did as part of your work, please sign [this contributors agreement](https://docs.google.com/a/quantifind.com/document/d/1kNwLT4qG3G0Ct2mEuNdBGmKDYuApN1CpQtZF8TSVTjE/) and send it back to contributors@quantifind.com

## Highcharts

This library includes links to [Highcharts](http://www.highcharts.com/). It does not include a copy of the source code, and does not modify the source code.

[Highcharts](http://www.highcharts.com/) is available freely for non-commercial use under [Creative Common NonCommercial 3.0](http://creativecommons.org/licenses/by-nc/3.0/). It is **not** free for [non-commercial use](http://shop.highsoft.com/faq/non-commercial#what-is-non-commercial). 
