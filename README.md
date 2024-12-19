# Guide to operating the profile webpage

## How is this website organized?

The profile_webpage repo hosues the code for the website.
The adityahebbani.github.io repo is what the website will be deployed off of with Github Pages.

To preview the website, in the profile_webpage repo:

```
hugo server
```

## How is the website deployed?

The profile_webpage repo has adityahebbani.github.io as a submodule. It is a reference to the website repo. How do I do that?

```
git submodule add -b main "github.io url" public
```

Keep in mind, you only need to do this once. This creates the reference to the main branch of the github.io repo and puts it in a folder called "public".

The static files that are generated are then automatically added to the public folder.

## How do I build it?

To populate the github.io (and therefore the public folder in this repo), run:

```
hugo -t hugo-profile
```

Then go into the public folder and commit and push to update the static items (adityahebbani.github.io) repository.
It will then automatically deploy and you can visit it at adityahebbani.github.io.

It does take a minute to do this.

