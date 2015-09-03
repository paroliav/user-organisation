# AAF Technical Test

**Confidential**

Welcome to the technical test. This project has a number of flaws which you may
like to correct. Take a look at the GitHub issues if you're looking for a place
to start.

Feel free to look around, find anything that deserves fixing, and fix it. This
may include:

* Code not functioning as intended
* Code which should be more idiomatic
* Security problems
* Ruby style issues (we like the [Ruby Style Guide][style-guide] and
  [Rubocop][rubocop])
* Incorrect tests, or tests that don't actually exercise the code correctly
* Missing coverage
* Anything else you want to fix

To save you some time, here are some areas of the code that don't have any
deliberate flaws:

* Basic project configuration &mdash; Rails `application.rb`, `environment.rb`,
  `database.yml`, `config.ru`, `Gemfile`
* `spec/spec_helper.rb` and `spec/rails_helper.rb`
* `db/schema.rb` (we committed exactly as generated by Rails)

[style-guide]: https://github.com/bbatsov/ruby-style-guide
[rubocop]: https://github.com/bbatsov/rubocop

## Setting up the project

The project will require a Ruby version of at least 2.0. We used 2.2.2 while
creating this project.  We like [rbenv][rbenv] and [ruby-build][ruby-build] for
installing Ruby, but you can use whatever installation method works best for
you.

Once you have a working Ruby installation, and have cloned the application, the
following commands will get you running:

```
bundle exec rake db:schema:load db:seed
bundle exec guard
```

Once Guard has launched, press enter to have it run the full suite of tests and
checks against the project.

To start the web application:

```
bundle exec unicorn
```

[rbenv]: https://github.com/sstephenson/rbenv
[ruby-build]: https://github.com/sstephenson/ruby-build

## Submitting changes

AAF works using [GitHub Flow][flow]. Before you start making any changes, you'll
want to create your own branch. For this project (and all projects in AAF should
you be offered a position), you will not need to fork the repository to your own
account.

We'll be reading your commit log, so if each commit is fairly atomic and has a
[quality commit message][commit-message], it will be easier for us to understand
your work.

Please submit your work by pushing **your branch** to the original repository,
and creating one or more pull requests. The pull requests should be formatted in
a way that you would feel comfortable submitting to an open source project.

[flow]: https://guides.github.com/introduction/flow/
[commit-message]: https://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message