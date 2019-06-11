# Debug-Disabler

##### Non-destructively disables Debug from being called in the editor console and in the build.

### Instructions

Import script into your project. The script can be placed in any folder.

This script overrides Unity's Debug class and prevents them from being called via __Platform Dependent Compilation__. This is non-destructive, meaning none of your project is altered.

You would want to disable Debug since it is technically bad to have it constantly called in your project, as it generates _stack trace parsing_ and writes to the editor log each time it is called. Use this only if you specifically want to disable Debug for performance or clutter reasons.

If you want to quickly debug something to the console without having to remove the script, an alternative is to use `print("");`.
