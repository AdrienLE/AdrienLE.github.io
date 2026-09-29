A Github Pages template for academic websites. This was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

I think I've got things running smoothly and fixed some major bugs, but feel free to file issues or make pull requests if you want to improve the generic template / theme.

## Dependency security

Keep both `Gemfile.lock` and `package-lock.json` committed. Update dependencies and run the audits below when a security advisory arrives; deleting a lockfile does not fix a vulnerable dependency.

The Ruby bundle uses Jekyll 3.10 and the plugins this site uses. It does not install the full `github-pages` theme bundle, whose unused remote-theme dependency restricts rubyzip to vulnerable versions. This keeps the local build on the GitHub Pages-compatible Jekyll series. GitHub's managed Pages builder controls its own installed dependencies.

Dependabot checks the Ruby, npm, and GitHub Actions dependencies weekly. The validation workflow builds the site, audits both dependency sets, and checks that the committed JavaScript bundle is reproducible.

# Instructions

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## Run locally

Use Ruby 3.4 and Node.js 22 or newer.

```sh
bundle install
npm ci --ignore-scripts
npm run build:js
bundle exec jekyll serve --livereload --host 127.0.0.1 --config _config.yml,_config.dev.yml
```

The development configuration uses localhost URLs and disables analytics. Browse to `http://localhost:4000`.

## Validate dependency updates

```sh
bundle exec bundle-audit check --update
npm audit
npm run build:js
npm run check:js
bundle exec jekyll build
```

Commit the updated lockfiles and `assets/js/main.min.js` together with dependency changes. jQuery and Magnific Popup are locked npm dependencies; their code is included in the committed bundle, so rebuilding it is required for visitors to receive an update.

# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch. 

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20). Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.
