CucumberByCommit
================

commit by commit process of setting up cucumber/ruby tests


some links to read
the main cucumber site: http://cukes.info/
a cucumber wiki: https://github.com/cucumber/cucumber/wiki
cucumber backgrounder: https://github.com/cucumber/cucumber/wiki/Cucumber-Backgrounder

the site I want to test: http://dan-the-baker.com/toastbar/


commands
`bundle install` - ran this after making the Gemfile. this produced the Gemfile.lock file

tried running cucumber:
`bundle exec cucumber`
got:
```bash
No such file or directory - features. Please create a features directory to get started. (Errno::ENOENT)
```

made a features directory (`mkdir features`)
and ran `bundle exec cucumber` again:
```bash
CucumberByCommit master@0684848 ✗ $ bundle exec cucumber
0 scenarios
0 steps
0m0.000s
```

added a feature file `features/visit_a_site.feature` and reran cucumber:
```bash
CucumberByCommit master@6857010 $ bundle exec cucumber
Feature: Visiting the site

  Background:  # features/visit_a_site.feature:3

  Scenario:  # features/visit_a_site.feature:6

1 scenario (1 passed)
0 steps
0m0.001s
```

