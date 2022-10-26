# leapyear -  [![Java CI with Maven](https://github.com/Scarcy/leapyear/actions/workflows/maven.yml/badge.svg?branch=main&event=push)](https://github.com/Scarcy/leapyear/actions/workflows/maven.yml)
Oblig 3 innlevering: Oblig 2 med CI github actions

I used Maven to build and run the tests. I added Maven surefire so Github actions could find and run the tests (I also needed to rename the test files to follow surefire convention). I used "-Dmaven.test.skip=true" to skip running the test in the build phase so the build and test are seperate 
(So it's easier to see if there's something wrong with the build or if it's just the tests failing).

Also changed the settings so merging to main requires passing tests

Finally, I used "dorny/test-reporter@v1" to create a Test Report so the JUnit tests are shown in a clean way. This also makes the result of the test available to users that aren't logged in
