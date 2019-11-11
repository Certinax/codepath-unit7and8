# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Unauthenticated stored cross site scripting
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.4.1
  - [x] GIF Walkthrough: 
  <img src="https://github.com/Certinax/codepath-unit7and8/blob/master/xss3.gif">
  - [x] Steps to recreate: 
  Get an admin to upload a link with an embedded XSS in it. on load it fires the script
  - [x] Affected source code:
    - [Link 1](https://wpvulndb.com/vulnerabilities/7945)
2. Unauthenticated short code tags Cross-Site Script
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.3.1
  - [x] GIF Walkthrough: 
  <img src="https://github.com/Certinax/codepath-unit7and8/blob/master/xss1-2.gif">
  
  - [x] Steps to recreate: 
  a new post must be created and a xss alert must be embedded into a tag on the page when you click on the tag the alert will be triggered.
  - [x] Affected source code:
    - [Link 1](https://wpvulndb.com/vulnerabilities/8186)
3. Unauthenticated cross site scripting
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [x] GIF Walkthrough: 
  <img src="https://github.com/Certinax/codepath-unit7and8/blob/master/xss1-1.gif">
  <img src="https://github.com/Certinax/codepath-unit7and8/blob/master/xss1-2.gif">
  - [x] Steps to recreate: 
  Attacker will write a very long comment with a xss script embedded that cannot be properly handled by the database, then tthe scriptt will be executed once the admin approves and looks at the posted comment. 
  - [x] Affected source code:
    - [Link 1](https://wpvulndb.com/vulnerabilities/7945)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

A lot of things I tried didn´t work. XSS seems to be the easiest to reproduce.

## License

    Copyright [2019] [Certinax]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
