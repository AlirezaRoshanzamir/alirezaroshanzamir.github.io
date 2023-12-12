---
weight: 4
title: "Python Acceptance Test Frameworks Comparison"
date: 2023-12-12T00:00:00+00:00
lastmod: 2023-12-12T00:00:00+00:00
draft: false
author: "Alireza Roshanzamir"
authorLink: "https://alirezaroshanzamir.github.io/about/"
description: "Python BDD frameworks comparison"
images: []
resources:
- name: "python-acceptance-test-frameworks"
  src: "python-acceptance-test-frameworks.png"

tags: ["Acceptance Testing", "Testing", "BDD", "Behavior-Driven Development", "Gherkin", "GWT", "Given-When-Then", "RobotFramework", "Behave", "Cucumber", "Continuous Delivery", "UAT", "JIRA", "Xray", "ATDD", "Acceptance Test-Driven Development"]
categories: ["Libraries/Tools"]

lightgallery: true
---

<table>
  <tr>
    <th>Property</th>
    <th>
      <a href="https://behave.readthedocs.io">Behave</a>
    </th>
    <th>
      <a href="https://pytest-bdd.readthedocs.io">Pytest-BDD</a>
    </th>
    <th>
      <a href="https://robotframework.org">Robot Framework</a>
    </th>
    <th>Hamgam (proprietary)</th>
  </tr>
  <tr>
    <td>GitHub stars</td>
    <td>3k</td>
    <td>1.2k</td>
    <td>8.5k</td>
    <td>0</td>
  </tr>
  <tr>
    <td>Used by</td>
    <td>10.1k</td>
    <td>3k</td>
    <td>8.8k</td>
    <td>30</td>
  </tr>
  <tr>
    <td>Contributers</td>
    <td>73</td>
    <td>50</td>
    <td>177</td>
    <td>7</td>
  </tr>
  <tr>
    <td>Forks</td>
    <td>682</td>
    <td>208</td>
    <td>2.2k</td>
    <td>0</td>
  </tr>
  <tr>
    <td>Commit/Week</td>
    <td>1</td>
    <td>1</td>
    <td>10</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Open issues</td>
    <td>60</td>
    <td>110</td>
    <td>275</td>
    <td>0</td>
  </tr>
  <tr>
    <td>Open PRs</td>
    <td>28</td>
    <td>33</td>
    <td>32</td>
    <td>0</td>
  </tr>
  <tr>
    <td>Gherkin/GWT<br>
      <small>More BDD and agile friendly. Also, can utilize Xray <a href="https://docs.getxray.app/display/XRAY/Automated+Steps+Library">steps library</a>.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>Almost <span style="font-size: 30px">✓</span>
      <br>
      <small>A subset of the Gherkin (for example, doesn't support <a href="https://github.com/pytest-dev/pytest-bdd/issues/411">tags for different scenario outline examples</a>).</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>But has some <a href="https://pypi.org/project/gherkin2robotframework/">translators</a>, however, the result is not human-readable.</small>
      <br>
      <small>Also, you can <a href="https://robotframework.org/?tab=0&example=BDD-Example#getting-started">mimic GWT</a> using custom keywords.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Currently, you can only write scenarios in a GWT manner.</small>
    </td>
  </tr>
  <tr>
    <td>JIRA Xray automation support<br>
      <small><a href="https://docs.getxray.app/display/XRAYCLOUD/TTT%3A+Automation">The exported test cases from Xray are directly usable, and the execution outputs can be imported directly.</a></small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small><a href="https://docs.getxray.app/display/XRAYCLOUD/Testing+using+Behave+in+Python">By exporting <strong>Cucumber</strong> test feature files and importing JSON results.</a></small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small><a href="https://docs.getxray.app/display/XRAYCLOUD/Generate+Cucumber+Features">By exporting <strong>Cucumber</strong> test feature files</a> and <a href="https://docs.getxray.app/display/XRAYCLOUD/Testing+using+pytest+in+Python">importing JUnit XML report.</a></small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small><a href="https://docs.getxray.app/display/XRAYCLOUD/Testing+using+Robot+Framework+integration+in+Python+or+Java">By exporting <strong>Generic</strong> test files and importing the JUnit XML results or using the REST APIs.</a></small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Custom languages (rather than Gherkin/GWT)</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span> (but only in Python)
    </td>
  </tr>
  <tr>
    <td>Graphical report</td>
    <td>
      <a href="https://github.com/behave-contrib/behave-html-formatter">
        <span style="font-size: 30px">✓</span>
      </a>
    </td>
    <td>Partly <span style="font-size: 30px">✓</span>
      <br>
      <small>Can use Pytest graphical reports (such as <a href="https://pypi.org/project/pytest-html/">pytest-html</a>, <a href="https://pypi.org/project/pytest-html-reporter/">pytest-html-reporter</a>, or any other JUnit based reports).</small>
    </td>
    <td>
      <a href="https://robotframework.org/robotframework/latest/images/screenshots.png">
        <span style="font-size: 30px">✓</span>
      </a>
      <br>
      <small>
        <a href="https://docs.robotframework.org/docs/reporting_alternatives">Also supports multiple alternative reporters.</a>
      </small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Writing custom reports</td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>
        <a href="https://behave.readthedocs.io/en/stable/formatters.html">Using Formatters and Reporters.</a>
      </small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>
        <a href="https://docs.pytest.org/en/latest/reference/reference.html#hook-reference">Using Pytest hooks</a>
      </small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Custom data driver</td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented in a tricky way, but has an <a href="https://github.com/behave/behave/issues/622">open pull-request for CSVs</a>.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented in a <strong>very</strong> tricky way.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using a <a href="https://github.com/Snooz82/robotframework-datadriver">robotframework-datadriver</a> plugin.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Dry run</td>
    <td>Syntax: <span style="font-size: 20px">✓</span>
      <br>Reporters: Partly <span style="font-size: 20px">✓</span>
      <br>Type check: <span style="font-size: 20px">✗</span>
      <br>Auto-wiring: <span style="font-size: 20px">✗</span>
      <br>Pre/post-conditions: <span style="font-size: 20px">✗</span>
    </td>
    <td>Syntax: <span style="font-size: 20px">✗</span>
      <br>Reporters: <span style="font-size: 20px">✗</span>
      <br>Type check: <span style="font-size: 20px">✗</span>
      <br>Auto-wiring: <span style="font-size: 20px">✗</span>
      <br>Pre/post-conditions: <span style="font-size: 20px">✗</span>
    </td>
    <td>Syntax: <span style="font-size: 20px">✓</span>
      <br>Reporters: <span style="font-size: 20px">✗</span>
      <br>Type check: <span style="font-size: 20px">✗</span>
      <br>Auto-wiring: <span style="font-size: 20px">✗</span>
      <br>Pre/post-conditions: <span style="font-size: 20px">✗</span>
    </td>
    <td>Syntax: <span style="font-size: 20px">✓</span>
      <br>Reporters: <span style="font-size: 20px">✓</span>
      <br>Type check: <span style="font-size: 20px">✓</span>
      <br>Auto-wiring: <span style="font-size: 20px">✓</span>
      <br>Pre/post-conditions: <span style="font-size: 20px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Declarative steps/keywords/actions</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Filter tests</td>
    <td>File: <span style="font-size: 20px">✓</span>
      <br>Scenario: <span style="font-size: 20px">✓</span>
      <br>Parameters: <span style="font-size: 20px">✗</span>
    </td>
    <td>File: <span style="font-size: 20px">✓</span>
      <br>Scenario: <span style="font-size: 20px">✓</span>
      <br>Parameters: <span style="font-size: 20px">✓</span>
    </td>
    <td>File: <span style="font-size: 20px">✓</span>
      <br>Scenario: <span style="font-size: 20px">✓</span>
      <br>Parameters: <span style="font-size: 20px">✗</span>
      <br><small>But each record can have a name and be filtered.</small>
    </td>
    <td>File: <span style="font-size: 20px">✓</span>
      <br>Scenario: <span style="font-size: 20px">✓</span>
      <br>Parameters: <span style="font-size: 20px">✓</span>
    </td>
  </tr>
  <tr>
    <td>T-wise or pair-wise testing execution</td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>But can be implemented using hooks.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>But can be implemented using hooks.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>But can be implemented in the data-driver layer.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Auto-wiring</td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Pre/post-conditions</td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>Can be implemented manually.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Hooks</td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <a href="https://docs.robotframework.org/docs/extending_robot_framework/listeners_prerun_api/listeners">
        <span style="font-size: 30px">✓</span>
      </a>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Parallel execution</td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>But has some <a href="https://github.com/hrcorval/behavex">wrappers</a> and has an <a href="https://github.com/behave/behave/pull/616">open pull-request</a>.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using Pytest parallel execution plugins.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using plugins.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>But only in a single process.</small>
    </td>
  </tr>
  <tr>
    <td>Model-based testing</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td> Unit-test friendly <br>
      <small>Can have acceptance unit-tests and reuse codes.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Marks/tags</td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>
        <a href="https://github.com/pytest-dev/pytest-bdd/issues/411">But for the whole scenario not the examples.</a>
      </small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>But for the whole scenario not the examples.</small>
    </td>
  </tr>
  <tr>
    <td>IDE friendly</td>
    <td>Highlight: <span style="font-size: 20px">✓</span>
      <br>Auto-complete: <span style="font-size: 20px">✗</span>
      <br>Execute: <span style="font-size: 20px">✓</span>
    </td>
    <td>Highlight: <span style="font-size: 20px">✓</span>
      <br>Auto-complete: <span style="font-size: 20px">✗</span>
      <br>Execute: <span style="font-size: 20px">✓</span>
    </td>
    <td>Highlight: <span style="font-size: 20px">✓</span>
      <br>Auto-complete: <span style="font-size: 20px">✓</span>
      <br>Execute: <span style="font-size: 20px">✓</span>
    </td>
    <td>Highlight: <span style="font-size: 20px">✓</span>
      <br>Auto-complete: <span style="font-size: 20px">✓</span>
      <br>Execute: <span style="font-size: 20px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Programming statements (for, if, while, ...)</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Background (setup/teardown)</td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Reusable fixtures</td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using Pytest fixtures mechanism.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
  </tr>
  <tr>
    <td>Localization</td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Learning curve</td>
    <td>Good</td>
    <td>Good</td>
    <td>Good</td>
    <td>Normal (for scenarios)</td>
  </tr>
  <tr>
    <td>Rich plugins and related libraries</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      Partly <span style="font-size: 30px">✓</span>
      <br>
      <small>Can use Pytest plugins, but doesn't have GWT steps.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Selenium, HTTP requests, Appium, REST, SSH</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>In-browser execution</td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using <a href="https://pyodide.org/en/stable/">WASM Python</a>.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
    </td>
  </tr>
  <tr>
    <td>Multiple programming languages for steps implementation</td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Most programming languages have some implementations for Gherkin.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Most programming languages have some implementations for Gherkin.</small>
    </td>
    <td>
      <span style="font-size: 30px">✓</span>
      <br>
      <small>Using <a href="https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#remote-library-interface">Remote Library</a> concept.</small>
    </td>
    <td>
      <span style="font-size: 30px">✗</span>
      <br>
      <small>It only supports Python.</small>
    </td>
  </tr>
</table>