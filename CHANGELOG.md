## 📅 November 15, 2024

### Features and enhancements

#### Raycast extension

We've created an extension for Raycast to make it even quicker to try out your ideas for new sparks. Instead of navigating to existing apps, this essentially lets you "navigate" to brand new apps that are created on demand.

Once installed, just search for the extension...

<img width="795" alt="image" src="https://github.com/user-attachments/assets/bab0c0b5-954b-4e29-b698-905c28976b37">

...and get to creating!

![image](https://github.com/user-attachments/assets/c6f08673-6b37-4443-aab8-0bcc1b339cef)

Grab the extension today at <https://www.raycast.com/github-next/github-spark>.

#### Create new sparks straight from the URL

Behind-the-scenes the Raycast extension makes use of another new feature: the ability to create a new spark straight from any URL bar. Using `https://spark.githubnext.com/new/<prompt>`, you can jump straight into a brand new spark. You can also specify which model to use and whether to generate variants: <a href="https://spark.githubnext.com/new/make a tic tac toe game that's lizard themed?model=sonnet&generateVariants=true">`https://spark.githubnext.com/new/make a tic tac toe game that's lizard themed?model=sonnet&generateVariants=true`</a>. We're curious to see what other integrations people will make using these URLs!

#### Added support for more Web APIs

We've added support for more advanced web APIs in the spark runtime, including [Web MIDI](https://developer.mozilla.org/en-US/docs/Web/API/Web_MIDI_API), [Web Bluetooth](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API), and [WebUSB](https://developer.mozilla.org/en-US/docs/Web/API/USB).

Here's a quick MIDI event viewer at <https://spark.githubnext.com/share/amYNXdV3EtV6paF5LiwWA>, but we're even more excited about you all will create, from custom synthesizers to interactive visualizations.

<img width="600" alt="image" src="https://github.com/user-attachments/assets/17262618-3ce3-467a-94dd-3abe450e714e">

#### Made it easier to work with prompts

You all have been busy typing! These are the first steps we're taking to make creating and refining sparks a little smoother. First, some breathing room! In both the dashboard and the editor you can now see multiple lines of text:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/c8d7c53c-fcd4-4aca-9564-325b0fcb9756">

And to make it easier to tweak your wording, you can go back to your previous prompt by pressing `Up Arrow` in the iterate textbox.

#### Improved custom colors in dark mode

When tweaking colors on some elements, some sparks would only look correct in light or dark mode and not have enough contrast in the other. We've now made it so sparks use adaptive color palettes by default and automatically adjust custom styled elements to light/dark mode.

### Bug fixes

This is where we fight every patch note writer's instinct to write "General system stability improvements" and call it a day. But you deserve more!

- **Improved code generation reliability:** we identified the most common cases causing generated code to not run on the first try. We've solved many of these, through a combination of runtime tweaks, and being even nicer to our models.
- **Improved syncing reliability**: some sparks were consistently failing to sync, which is now fixed.
- **Save your work-in-progress prompts**: we no longer clear the prompt when you switch between tabs. Can't figure out how to word your instructions until you change the theme from green to orange? Well this fix is for you!
- **Fixed rendering of the "none" border radius choice**: blocky elements might not be our thing, but we didn't mean to stop you! The "none" option should work much more consistently now. 

## 📅 October 29, 2024

Initial release at GitHub Universe 2024! 🚀
