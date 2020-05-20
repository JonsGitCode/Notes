# Notes
Notes, tips, solutions, research, etc.

Selenium "webdriver.Firefox()" as instructed in Automate the Boring Stuff lesson 41 caused an error:
 - problem: missing geckodriver for Firefox. Each browser now requires a driver
 - solution: downloaded Mac driver from Mozilla geckodriver Github page
 - problem: still unable to use: webdriver.Firefox()
 - solution: user webdriver.Firefox(executable_path=r'/Users/jshapiro100/Downloads/geckodriver') to launch a Firefox browser
 - problem: still unable to set browser = webdriver.Firefox(executable_path=r'/Users/[username]/Downloads/geckodriver')
 - solution: use: (webdriver.Firefox(executable_path=r'/Users/[username]/Downloads/geckodriver').get('https://automatetheboringstuff.com')) to open the browser to a URL instead.
