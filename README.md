# leapyear
Oblig 3 innlevering: Oblig 2 med CI github actions

I used Maven to build and run the tests. I added Maven surefire so Github actions could find and run the tests (I also needed to rename the test files to follow surefire convention). I used "-Dmaven.test.skip=true" to skip running the test in the build phase so it's easier to see if there's something wrong with the build or if it's just the tests failing
