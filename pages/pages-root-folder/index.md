---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: Interconnect_pcb.jpeg
widget1:
  title: "First TestStation <br> Project"
  url:  #'http://FirstTestStation.github.io/FTS_Website/info/'
  image: FirstTestStation.png
  text: "The project's objective is to provide, at a low cost, a starting test platform for testing electronic production boards or electronic systems. Designed as a free project by just retired Test Engineer, it will offer a complete test solution by providing a complete testing example."
widget2:
  title: "Test Automation"
  url: 'http://opentap.io/'
  image: opentap2.jpg
  text: '<a href= "http://opentap.io/OpenTap">OpenTap</a>, a free open source test automation software, will be used to perform the test sequence execution. The new software on the test industry is well documented, and you can access many training videos on <a href="https://www.youtube.com/results?search_query=opentap">YouTube</a>.'
 
  #video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Download Project"
  url: 'https://github.com/FirstTestStation'
  image: github.jpg
  text: The '<em>FirstTestStation</em>' project is an open-source initiative providing schematics, Gerber files, and source code for a complete testing solution, freely available on GitHub.
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
########## DL
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

