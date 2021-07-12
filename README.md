# gittests

This repository has been for running some tests with github actions.

The workflow files in here are based on two approaches, one is the standard semantic release for automated tag creation.
The first work wokflow uses the package.json file for the semantic release configuration and tag naming.

The other(second workflow) is based on another github action tooling which also uses the semantic release capabilities but provides more
flexibility when managing the tag names. This allows you set variying tag names based on the folder that a commit occurs.

Why two workflows that use different tooling?

Well, it is simply because the semantic release does not provide for multiple application folders using different package.json files 
at the root of those package directiories.

A walk around this is to have one workflow use the package.json(with varying tag name) file and the other workflow uses 
the other tooling for tagging.

