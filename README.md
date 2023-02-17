# PacktPub - free book downloader
Ruby exercise project: how to get a free book from packtpub

# What would you need to run this

jRuby, or another Ruby interpreter.
Installed gems:
 - mechanize
 - openssl
 - watir
 
 Watir is a library to run your browser using Chromecast. Chromecast needs to be on your path before, howether one can just set it as current dir:
  set PATH=.\;%PATH%
 
 To get proper Chromecast version, visit https://chromedriver.chromium.org/downloads
 If you pick wrong version, do not worry: the message will tell you what you need.
 
 Last but not least, you need PacktPub account
 
 # What script does
 
 This Ruby script:
  - applies for free book using a browser controlled by Watir
  - then logs to you account using APackPub API and downloads all the formats available (mobi, pdf, epub, and code URL)
 
 For this purpose it must be started with parameters: user and password as registered in PackPub.
 
 # Issues
 During the run it may happen that script is too fast in the "apply for book" part. You can add more delay, see the "sleep" lines.
 It also can happen you will see CAPTCHA test - you need to solve it youself in few seconds, as that script does not use any AI.
 
 
 
