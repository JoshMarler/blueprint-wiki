# Getting Started

This guide assumes you have some familiarity with [React.js](https://reactjs.org/) and with [JUCE](https://juce.com/), and it is therefore recommended that you spend some time getting comfortable there, if you're not already, before embarking on this guide.

## Dependencies
To get started with Blueprint, you'll first need to install a few dependencies:

* [Node.js](https://juce.com/) v8.11.0+
* [npm](https://www.npmjs.com/) v5.6.0+
* [JUCE](https://juce.com/) v5.4.2+ (Optional if you are only running the examples)
* Xcode9.4+ (MacOS)
* Visual Studio 2017+ (Windows)

Once you have the dependencies installed, we need to clone the Blueprint repository
itself. Blueprint's git repository contains necessary submodules, so we'll need to
collect those as well, which we can do one of two ways:

```bash
$ git clone --recurse-submodules git@github.com:nick-thompson/blueprint.git
```
or
```bash
$ git clone git@github.com:nick-thompson/blueprint.git
$ cd blueprint
$ git submodule update --init --recursive
```

Note that the `git@github.com` prefix here indicates cloning via SSH. If you prefer
to work with git via HTTPS you'll want to swap in `https://github.com/nick-thompson/blueprint.git`
in the above commands.

## Building juce-blueprint
Now we almost have everything we need to start working with Blueprint. The last step
is to build the `juce-blueprint` JavaScript library included in the repository. From within
the root of the `blueprint` git repository:

```bash
$ cd packages/juce-blueprint
$ npm install
$ npm run build
```

At this point, we've got everything ready to get our project up and running. Let's
move on to the next step, [[running the demo plugin|running-the-example]].
