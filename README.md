# PacktPub - free book downloader

Ruby exercise project: get a daily free book from PacktPub!

# What would you need to run this

jRuby (or another Ruby interpreter).
Installed gems:
 - mechanize
 - openssl
 - watir
 
 Watir is a library to run your browser (the default is Chrome, with usage of Chromecast driver).
 More information you can find on project page.
 Chromecast needs to be on your path before, howether one can just set it as current dir in some run.cmd script:
  
  set PATH=.\;%PATH%
 
 To get proper Chromecast version, visit https://chromedriver.chromium.org/downloads
 If you pick wrong version, do not worry: the message will tell you what you need.
 
 Last but not least, you need a PacktPub account. That will store your books!
 
 # What script does
 
 This Ruby script:
  - applies for free book using a browser controlled by Watir
  - then logs to you account using PackPub API and downloads all the formats available of today's free book (mobi, pdf, epub, and code URL)
 
 The files will be saved in the execution folder.
 
 # How to run
 
 Script shall be started with parameters: user-email and password as registered in PackPub.
 
 jruby -W0 packt.rb <your packtpub user-email> <your password>
 
 # Issues
 
 During the run it may happen that script is too fast in the "apply for book" part. You can add more delay, see the "sleep" lines.
 It also can happen that you will see CAPTCHA test - you need to solve it youself in few seconds, as that script does not use any AI.
 Good side, most of the time all the actions wil not need your clicks.
 
 
