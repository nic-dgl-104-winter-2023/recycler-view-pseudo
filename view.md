# View
A view is generally some interface element in an app or web app. A view could be something as simple as a textbox, or something more complex, like a form (often composed of multiple views).

The view captures most user interaction and in many platforms this interaction triggers events, which are caught by other layers of the system. A view should be thought of as reactive to state changes (i.e. changes to data, based on user input), but should not be directly responsible for managing those state changes itself.

## Pseudocode
```
DEFINE each view element and provide hooks to access each via the adapter

