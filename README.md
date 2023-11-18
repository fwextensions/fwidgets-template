# fwidgets-template

> Create a simple Figma plugin UI with zero UI code.

![screenshot](https://user-images.githubusercontent.com/61631/280552964-f63c103e-61db-4b7b-8610-2116613e665d.png)

Many useful Figma plugins run only in the main thread, where they can access the API and modify the document.  But sometimes you want to extend them with simple user interface elements, like a textbox to enter a name, or a color picker to customize the output.  Unfortunately, Figma doesn't offer any built-in UI components, so you have to roll your own, using a framework or vanilla JS/HTML/CSS.  And then you have to post messages back to the main thread in response to UI events, just so your plugin can actually make changes to the Figma document.

`fwidgets` is intended to dramatically simplify this process by letting you add basic UI functionality without writing any UI code.  Think of it like adding a series of interactive prompts to a command line tool, similar to the wizard structure of something like `create-react-app`.  `fwidgets` lets you show one UI element at a time to the user, awaiting their input and then responding to it, while keeping all of your code in the main thread.


## Install

This repo includes all the scaffolding needed to use [`fwidgets`](https://github.com/fwextensions/fwidgets) in a Figma plugin.  It's easiest to start with a copy of it by running this command:

```shell
npx --yes degit fwextensions/fwidgets-template my-plugin-name
```

Replace `my-plugin-name` with whatever you want to call the directory for your plugin.


## Usage

See the [`fwidgets` readme](https://github.com/fwextensions/fwidgets#usage) for details on how to use it to show UI controls within your plugin.
