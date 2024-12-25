# Event Counter Application

## Overview
This is a simple HTML, CSS, and JavaScript application that tracks various user interaction events on an input text box. The application counts the number of times specific events occur and dynamically updates the counts in an HTML table.

## Features
1. Tracks the following events on the input text box:
   - `input`
   - `mouseover`
   - `mousemove`
   - `mouseup`
   - `mouseout`
   - `keydown`
   - `keypress`
   - `keyup`
   - `blur`
   - `focus`
2. Displays the counts for each event in a styled HTML table.
3. Simple and clean user interface.

## File Structure
- **HTML**: Contains the structure of the application, including the input box, button, and table.
- **CSS**: Styles the table and its elements with dashed borders and proper alignment.
- **JavaScript**: Adds event listeners to the input text box and updates the event counts in real-time.

## How It Works
1. An input text box and a "Submit" button are rendered at the top of the page.
2. Below the input box, an HTML table displays the event names and their respective counts.
3. Event listeners are added to the input text box to capture interactions such as typing, mouse movements, and focus/blur actions.
4. When an event occurs, its count is incremented and displayed in the table.

## Code Breakdown
### HTML
- The input text box and "Submit" button are inside a `<div>` element.
- The table contains rows for each tracked event. The first column lists the event name, and the second column shows the count.

### CSS
- Table elements (`<table>`, `<th>`, `<td>`) have dashed black borders for a consistent style.
- Table headers are styled with larger font sizes and bold text.
- Padding ensures proper spacing within table cells.

### JavaScript
- Each event is tracked using an event listener attached to the input text box.
- The count for each event is stored in a variable and updated dynamically when the event occurs.
- The corresponding table cell is updated with the new count using `innerHTML`.

## Usage Instructions
1. Open the `index.html` file in a web browser.
2. Interact with the input text box:
   - Type text.
   - Hover over the text box.
   - Move the mouse inside the text box.
   - Click, release, or move the mouse outside the text box.
   - Use keyboard keys while the text box is focused.
   - Focus or blur the text box.
3. Observe the event counts updating in the table below.

## Example Output
After interacting with the input box, the table might look like this:

| Event        | Number |
|--------------|--------|
| Input        | 3      |
| Mouseover    | 2      |
| Mousemove    | 5      |
| Mouseup      | 1      |
| Mouseout     | 1      |
| Keydown      | 4      |
| Keypress     | 4      |
| Keyup        | 4      |
| Blur         | 2      |
| Focus        | 1      |

## Customization
- Modify the styles in the `<style>` block to change the appearance of the table.
- Add more event listeners if you want to track additional events.
- Adjust the table width or padding as needed for better responsiveness.

## Notes
- The `keypress` event is deprecated in modern browsers. Use `keydown` and `keyup` for consistent results.
- Ensure your browser supports the latest JavaScript features for optimal performance.

## Author
This application was created to demonstrate basic DOM manipulation and event handling in JavaScript.

