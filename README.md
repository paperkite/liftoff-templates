# PaperKite's Liftoff Template

Inspired by [Ben Kreeger](https://github.com/kreeger/liftoff-templates), We're also going to checkin our liftoff template. 

As we make new projects pretty often, so it makes sense to keep them consistant. This will eventually become natural, and everyone will be on the same page, and know where everything should be when they open a project we've created.

## Installing the Template

First install [liftoff](https://github.com/thoughtbot/liftoff)

	brew tap thoughtbot/formulae
	brew install liftoff

Depending on where you store project repositories determines where you install. Clone this repo to the folder where you clone our projects.

For example say you clone projects to `~/PaperKite/*`, that's where you'd need to clone this to.

	cd ~/PaperKite
	git clone git@github.com:paperkite/liftoff-templates.git ./.liftoff
	ln -s ./.liftoff/.liftoffrc .liftoffrc
	
## Creating a new project

In the directory you cloned this repo (should be the place where you store the various projects you're working on) just run `liftoff` and follow the prompts.

	cd ~/PaperKite
	liftoff
	
The installation can take a few minutes depending how fast the CocoaPods download. Once the process is complete, xcode will open with the new project.
	
There's one thing that liftoff doesn't yet support, and that's warnings as errors on debug builds. So you will have to manually do that. This is found in the 'Build Settings' tab in xcode, search for `Treat Warnings as Errors`, and just flick Debug to Yes.

Now you're ready to write some code!