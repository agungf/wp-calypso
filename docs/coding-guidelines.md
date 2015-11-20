Coding Guidelines
=================

Our coding guidelines are based on the standards adopted by the WordPress core project and WordPress.com with adjustments based on some of the particulars of Calypso and other improvements. If you come across issues or have suggestions, don't hesitate to open a PR.

### Language-Specific Guidelines

- [HTML](coding-guidelines/html.md)
- [SASS/CSS](coding-guidelines/css.md)
- [JavaScript](coding-guidelines/javascript.md)

### General Rules

1. Keep it Simple Stupid (KISS)
2. Write your code with your fellow developers in mind. A large part of the developer experience is being able to randomly open any file in the project and understand the code.
3. Try to stay consistent with the rest of the codebase, and when you recognize inconsistencies or fundamental design issues, bring them up. We all own the codebase and like a garden, we all need to help tend the weeds and keep the plants fertilized. 
4. Avoid premature optimization. Write clean code and if it doesn't perform well, then optimize.
5. Avoid both over-engineering and under-designing the code. Things should be thought out in the context of what they do now and how they are utilized.

Calypso already encourages a modular approach to architecting a system. Apply this throughout all the levels of what you do, from your functions to your files.


#### Trailing Whitespace

All files should have trailing whitespace removed.

It can be easy to leave whitespace at the end of lines by mistake. If you use Sublime Text you can strip this out automatically on save. Go to SublimeText 2 > Preferences > Settings - User (or just hit the Mac Standard cmd + ,). This should open your User Settings as a JSON file. Add the following to your file

```
"trim_trailing_white_space_on_save": true
```

If you use Coda2 you can use the Whiteout plugin: http://erikhinterbichler.com/apps/white-out/

When touching code that does not have trailing whitespace trimmed, make a separate commit that does the stripping before starting to make changes. This makes it easier to follow changes when looking at the history.