# Description
- In the 'Validator.side' file there is a list of test for the Validator UI.
- In the metadata folder there are some xml files useful some test (you have to specify folder's path as described below).
  
# Preliminary steps
- From one of the most commons browsers, install the extension 'Selenium'.
  (e.g. for Chrome https://chromewebstore.google.com/detail/selenium-ide/mooikfkahbdckldjjndioackbalphokd, for Firefox https://addons.mozilla.org/it/firefox/addon/selenium-ide/)
- Open it, select 'Open an existing project' and select the file 'Validator.side' and then click the 'Run all tests' button.
- Wait for the end and if some test go wrong, select them individually and try to re-run selecting the 'Run current test' 
  button.
- You can modify also the 'Test execution speed' from the clock button (default is fast) if the speed is too fast for a
  particular test (e.g. there are some errors because the page is not properly loaded).
  
# Before running test with Selenium:
- Make sure base URL present in the file you select (e.g. https://inspire.ec.europa.eu/validator/home/index.html in the "_production" file ) is correct. 
  Substitute with the correct one if it isn't the environment's URL you want to test or copy the file substituting the correct URL.
- Substitute the <path> string (present twice in the test file: rows 92 and 195) with the correct path where is the folder 
  'metadata' (now it is under 'selenium-test').
- Make sure captcha verification is disabled (you can make this action from config.js) (if you can't do it, don't consider the test that pass from captcha)
