#!/bin/bash
yum update -y
yum install httpd -y
service httpd start
chkconfig httpd on
cd /var/www/html
echo "<html>
<div id="header"></div>
<div class="left"></div>
<div class="stuff">
  <br><br>
  <h1>The Amazing Resume</h1>
  <h2>Chuck McFeezy</h2>
  <hr />
  <hr />
  <br>
  <p class="head">Amazing Talents</p>
  <ul>
    <li>Reading really fast</li>
    <li>Doing math Problems really fast</li>
    <li>Running really fast</li>
    <li>Doing Really Cool Macho Stuff</li>
    <li>Gladiator</li>
  </ul>
  <p class="head">Skills</p>
  <ul>
    <li>Web Design with HTML & CSS</li>
  </ul>
  <p class="head">Education</p>
  <ul>
      <li>Amazing High School</li>
    </a>
  </ul>
</div>
</html>" > index.html
