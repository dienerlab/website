# The lab website

This is out lab website, a static page built with [Hugo](https://gohugo.io) on AWS Amplify.

## Getting a local copy and adding modifications

[Create a fork to your own Github account](https://github.com/dienerlab/website/fork) and get a local copy to your own machine:

```bash
git clone git@github.com:my_user/website
```

You can edit the webpage or also install [Hugo](http://gohugo.io) and have a look at you edits by running

```
hugo server
```

and opening https://localhost:1313 in your browser.

Once you are satisfied you can create a pull request by committing and pushing your changes

```bash
git add .
git commit -am "description of the changes"
git push
```

After that you can crate a pull request by going to https://github.com/dinerlab/website and clicking on the pull request button.

## Adding a new team member

This should hopefully be straight-forward and has 2 steps.

1. Add a new file to the team folder, like `content/team/my_name.md`. This is just a markdown file with some metadata in the header that you will fill out. For instance:

```markdown
+++
picture = "bruno.jpg"
first = "Bruno"
last = "Pelaez"
email = "bruno [at] dienerlab.com"
status = "active"
position = "The real boss"
twitter = ""
bluesky = ""
mastodon = ""
orcid = ""
website = ""
date = "2024-02-08T17:30:20-08:00"
+++

<!-- Very short bio here -->
```

You can leave socials empty if you don't have an account. For the date use the date you joined the lab.

2. Copy the picture you mentioned in step 1 to `static/media/team`. This should be a rectangular picture.

That's it. You can now create a pull request as described above.
