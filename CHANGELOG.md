## 📅 February 21, 2025

### Targeted editing (functional & visual)

Make specific functional and visual changes to existing sparks using targeted editing. In the Iterate panel click the crosshairs icon to open the targeted editing pane in the app preview display.

https://github.com/user-attachments/assets/8dd7b8d3-b06f-4a5b-9859-7bcc7898f778

### Star shared sparks

When anyone shares their sparks with you, you can now star them and save them to your own dashboard without having to fork (just click the spark title to star). This makes it easier for you and loved ones to use the same spark (think shared meal planning & grocery list apps, family calendars, roommate chore trackers, a trivia app for friends, budgeting app for couples etc).

<img width="346" alt="Screenshot 2025-02-21 at 19 55 38" src="https://github.com/user-attachments/assets/73294c63-0423-44d8-8312-f67f976f77fa" />

![image (2)](https://github.com/user-attachments/assets/cde716ee-749e-4548-92a8-523d91fc4c51)

### Inspiration sparks

In the main dashboard we now always show a variety of inspiration sparks that you can generate with 1-click, or use to come up with new ideas for sparks of your own.

<img width="685" alt="Screenshot 2025-02-21 at 19 37 49" src="https://github.com/user-attachments/assets/cd9c527d-9d7c-4c24-9044-c0a841c871ff" />

### More features & bug fixes

* Made data & code syncing more reliable, and offer users choice on how to handle sync conflicts
* The ability to share sparks from your main dashboard
* Open sparks in edit mode on Desktop for faster access to spark refinements
* Fixed issue with old iteration prompts showing up in different sparks
* Fixed more code generation failure scenarios
* Fixed some buttons requiring multiple taps on Mobile from tooltips

## 📅 February 14, 2025

### Data panel redesign

We've upgraded the Data panel! Instead of editing freeform JSON, you now have a graphical interface that mirrors the structure of your data, making edits safer and more intuitive. Feeling adventurous? The raw JSON edit mode is still available when you need it. Let us know what you think!

https://github.com/user-attachments/assets/25b73cc5-f966-4e1f-9809-3963f90573a9

### More features & bug fixes

- Added an inline autofix button to errors in the Logs panel
- Improved model reliability, fixing more scenarios where Spark might stop generating code before it's finished
- Fixed rendering long instructions in the Iterate panel

## 📅 February 7, 2025

- Show a confirmation dialog when you click "Delete" in the data panel
- Add even more tooltips, this time to the workspace toolbar
- Prioritize showing the spark preview when generating code on mobile
- Add new Discord invite link to user menu

## 📅 February 1, 2025

### Thumbs down menu improvements

We previously introduced the 👎 button so that you can conveniently fix and revert changes that didn't go quite how you'd hoped for. Now we also include potential improvements that are customized for your particular spark. Just answer a few yes/no questions and you can kick off an iteration immediately by hitting "yes" if you see a change you want made. We're continuing to tune this feature and very much appreciate any feedback provided via [our Discord](https://github.com/githubnext/github-spark-user-manual/tree/main?tab=readme-ov-file#feedback).

<img width="600" alt="image" src="https://github.com/user-attachments/assets/f6a1dbde-bca0-4dbe-bcc2-5e17f4f0f33f" />

### More features & bug fixes

- Show more details when the history menu is expanded
- Add label to fullscreen exit button
- Show a red notification dot when errors are present in the log panel
- Auto scroll to the latest log when the log panel is open
- Enable text selection for prompts in editor header
- Added tooltips to sidenav

## 📅 January 17, 2025

### Icons for spark PWAs

As a follow-on to [last week's PWA support](#install-individual-sparks-as-pwas), Spark now generates custom icons for your sparks (in this example, both the metronome and the gym tracker are from Spark):

<img width="421" alt="image" src="https://github.com/user-attachments/assets/2d07e9b7-5904-4a30-90e9-cd4361f30a77" />

These new app icons automatically use your theme's accent color. The theme panel now has a new control to pick a different icon if you'd like to try something different, and clicking your spark's name will show you a preview of the icon if your spark were saved as a PWA.

### More features & bug fixes

- Code generation using Claude 3.5 Sonnet is now much more reliable
- Now clicking autofix after experiencing an error immediately triggers a repair attempt
- Improved editor in the Prompts panel with more reliable variable detection and ability to edit variables directly
- Improve loading state to have more stable UI
- Disallow code editing while code is being generated
- 
## 📅 January 10, 2025

### Install individual sparks as PWAs

Now in addition to letting you install Spark-the-editor on say, your phone, you can also install individual sparks, including ones shared with you.

https://github.com/user-attachments/assets/3155f62b-2ff8-4bbe-845a-25fbf9d73ba5

### More features & bug fixes

- Spark names are now used as page titles
- Scrolling through code as it streams in doesn't jump around anymore
- Make Spark less likely to generate code that uses `alert()` or `confirm()` in favor of in-app UI
- Fixed text cursor jumping while editing
- Fixed login to redirect you back to the original URL you were trying to view

## 📅 December 20, 2024

### URL context

Spark now considers context found in URLs you provide when creating a new spark or iterating on an existing one. Nudge Spark towards using particular libraries by including a link to their docs, or ask it to choose a color palette based on an image URL. This is just the start of being able to provide more context while creating your sparks, as we'll be adding more types of context and more features to interact with them.

### Prompts panel

Did you know that in addition to sparks being generated by LLMs that they can also make use of LLMs themselves at runtime? The "Prompts panel" lets you view and edit prompts in your sparks, all without needing to look at any code. Once saved, your spark's code is transparently updated.

We've just released the beginnings of more fleshed out prompting controls, now with improved editing that makes it easier to edit variables used within your prompts.

<img width="320" alt="image" src="https://github.com/user-attachments/assets/002b83f6-af4c-48d5-9207-fece9b48d854" />

## 📅 December 13, 2024

### Improvements to suggestions

We've made improvements to the suggested next steps feature we introduced <a href=#suggested-next-steps>last week</a>:

* You can request an entirely new set of suggestions
* You can individually dismiss suggestions and a new one will be generated in its place
* When generating new suggestions, it will take into consideration which ones you previously dismissed

<img src=https://github.com/user-attachments/assets/bff3856c-bfae-4cd6-b185-a05269614a32 width=300>

### More iteration controls

We've made it easier to take next steps when an iteration isn't quite what you wanted. There's a new 👎 menu in the toolbar that will let you either fully _Revert_ the most recent iteration, or _Revert & retry_, which will prefill the Iterate panel with the same prompt you just used, giving you the opportunity to further edit the prompt or try with a different model. And if Spark detects any errors, there's a new "Auto fix" button that will prefill the Iterate panel with information about the error. We've found the models to be quite good at fixing most errors – though if you find any particularly tricky ones we'd love for you to let us know in [our Discord](https://github.com/githubnext/github-spark-user-manual/tree/main?tab=readme-ov-file#feedback).

<img width="360" src="https://github.com/user-attachments/assets/960ae88b-f999-4c8b-8cf8-380f36cad8ec" />

### New mobile design

We've refreshed our mobile design to better match our recent [design changes on Desktop](#new-spark-editor-layout-on-desktop). All tabs are now only a single tap away, whereas previously some were hidden behind a menu.

https://github.com/user-attachments/assets/08f9c2f0-fcd4-484b-a2ef-56b1f7882700

### New dialog component

We've added a new `Dialog` component to the built-in Spark design system.

<img width="560" alt="image" src="https://github.com/user-attachments/assets/e7d48ac0-c1cd-4b6c-846e-72f5266b80b0" />

### Quick history access

On Desktop we've added buttons to let you navigate history more easily. Click around and reminisce on how your spark evolved!

<img width="250" alt="image" src="https://github.com/user-attachments/assets/386ef0a8-74ed-42ec-94c1-750c6f8937b8" />

## 📅 December 6, 2024

### Suggested next steps

The Iterate panel now suggests next steps. For example, here are some fun (and useful!) ideas on what we could do next with one of our metronome sparks

<img width="337" alt="image" src="https://github.com/user-attachments/assets/26ef5db2-4b2f-47b0-83b6-606d86250564">

Less typing, more iterating!

### Seed data

We now generate sample data when you're building a spark that persists data. This simulates how your spark might behave after you've used it for a while, and gives you the opportunity to immediately iterate on a new one without having to add your own test data first.

<img src="https://github.com/user-attachments/assets/f48d18bd-88b0-4b1f-9d1e-ec7d388abd8d" height=400>

### Use natural language to change the theme

You can now use natural language to tweak your theme:

<img width="250" alt="image" src="https://github.com/user-attachments/assets/80d6d15e-2c2b-4781-826c-cb3f4bc076f0">

And now brand new sparks will automatically choose accent colors, like the basketball game tracker above in the "Seed data" section that automatically chooses orange. (We apologize for waiting to add this until after Halloween!)

### More theming controls

#### Secondary accent colors

Add a secondary accent color to spice up your sparks:

<img width=400 src=https://github.com/user-attachments/assets/3491d1ee-0bba-4847-87bf-d9be9824d618>

#### More fonts

We added support for more varied fonts:

<img width="250" alt="image" src="https://github.com/user-attachments/assets/1c439e7c-f2b0-4ffb-8124-6f06595aa749">

### Improved variants layout

On Desktop we've moved variants out of the Iterate panel and have given them some space to breathe: 

<img width="600" alt="image" src="https://github.com/user-attachments/assets/6951b7dc-3abf-4b6d-9466-8defb31d8fbe">

## 📅 November 22, 2024

### Features and enhancements

#### New Spark editor layout on desktop

We've listened to your feedback and just added a brand new layout for desktop that makes much better use of the space available on larger screens. By default this new layout gives plenty of room for the spark you're interacting with, and you can optionally expand the new sidebar and then even open multiple panels at once. We're excited about continuing to refine the editor UI and make our panels even more powerful!

<img width="500" src="https://github.com/user-attachments/assets/cc5f25e5-1a0b-4d74-8296-0e13a7056d1a">

#### More icons!

Sparks are now more likely to automatically include icons when building UI. Sparks now default to using [Phosphor icons](https://phosphoricons.com/), which is a huge and varied set of icons.

<img width="500" src="https://github.com/user-attachments/assets/ba4d4189-0c40-4ec8-ac5a-d5613a587910">

#### Theme panel enhancements

And now you can control icon styling – like thin, bold, or our favorite, duotone – right from the Theme panel.
We've also added the ability to quickly change fonts, and expanded the number of accent colors.

<img width="338" alt="accent colors" src="https://github.com/user-attachments/assets/bb969c82-6339-4bd9-b451-41eb791d2425">

#### Built-in Markdown component

We've added a new Markdown component that sparks will now automatically use in order to easily render Markdown. This is especially nice for rendering LLM responses when called at runtime from sparks, but it's also great for little one-off utilities too!

<img width="400" src="https://github.com/user-attachments/assets/c8de326b-fc22-4c9e-b6b4-84d4d1ae683d">

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
