## Purpose

To show `base_path` does not work as expected in Bridgetown 2.0.0.beta2

## Getting started

```bash
git clone https://github.com/konnorrogers/bridgetown2-base-path-issue.git
cd bridgetown2-base-path-issue
bundle install
npm install
bin/bridgetown start
```

Navigate to `http://localhost:4000/content-editable` and it should be broken.

Now, go to `Gemfile`, and make the following change:

```diff
- gem "bridgetown", "~> 2.0.0.beta2"
+ gem "bridgetown", "~> 1.3"
```

Run `bundle update`

and then try `bin/bridgetown start` and navigate to `http://localhost:4000/content-editable` and it should work as expected.
