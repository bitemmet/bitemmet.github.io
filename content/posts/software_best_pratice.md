+++
title = "Software Best Pratice"
date = 2022-07-10

[extra]
toc = true

[taxonomies]
categories = ["BestPratice"]
tags = ["BestPratice"]
+++

# semantic version
[semantic version](https://semver.org/)

# Changelog
[keep a changelog](https://keepachangelog.com/en/1.0.0/)
don't let your friends dump git logs into changelogs

## What is a changelog?
A changelog is a file which contains a curated,chronologically
ordered list of notable changes for each version of a project.

## Why keep a changelog?
Tol make it easier for users and contributors to see precisely
what notable changes have been made between each release (or 
version) of the project.

## Who needs a changelog?
People do.Whether comsumers or developers, the end users of 
software are human beinngs who care about what's in the 
software. When the software changes, peopole want to know 
why and how.

## How do I make a good changelog?
### Guiding Principles
1. Changelogs are for humans, not machines
2. There should be an entry for envery single version.
3. The same types of changes should be grouped.
4. Versions and sections should be linkable.
5. The latest version comes first.
6. The release date of each version is displayed.
7. Mention whether you follow Semantic Versioning.


### Types of changes
1. **Added** for new features
2. **Changed** for changes in existing functionality.
3. **Deprecated** for soon-to-be removed features
4. **Removed** for now removed features.
5. **Fixed** for any bug fixes.
6. **Security** in case of vulnerabilities.

### How can I reduce the effort required to maintain a changelog?
Keep an **Unreleased** section at the top to track uncoming changes

This serves two purposes:
1. People can see what changes they might expect in upcoming 
release.
2. At release time, you can move the **Unreleased** section changes
into a new release version section.

## Can changelogs be bad?
Yes. Here are a few ways they can be less than useful.

### Commit log diffs
Using commit log diffs as changelogs is a bad idea.
They're full of noise. Things like merge commits, commits with
obscure titles, documentation changes, etc.

The purpose of a commit is to document a step in the evolution
of the source code. Some projects clean up commits.Some don't.

The purporsae of a changelog entry is to document the noteworthy
difference, often across multiple commits, to communicate them
clearly to end users.


### Ignoring Deprecations
When people upgrade from one version to another, it should be
painfully clear when something will break.It should be possible
to upgrade to a version that lists deprecations, remove what's
deprecated, then upgrade to the version where the deprecations
become removals.

If you do nothing else, list deprecations, removals, and any
breaking changes in your changelog.

### Confusing Dates
Regional date formats vary throughout the world and it's often
difficult to find a human-friendly date format that feels 
intuitive to everyone.The advantage of dates formatted like
**2017-07-17** is that they follow the order of largest to 
smallest unints: year, month, and day. This format also doesn't
overlap in ambiguous ways with other date formats, unlike
some regional formats that switch the position of month and day
numbers. These reasons, and the fact this date format is an 
**ISO standard**, are why it is the recommended date fromat
for changelog entries.





