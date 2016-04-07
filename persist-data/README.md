# Persist Data

__Q__: Can a mobile browser persist data in a cross-domain iframe? (using localStorage or cookie)<br>
__A__: Almost, but not quite.

### Setup

- Run a local server to serve up `index.html`
  - use `ngrok` to make your local server globally accessible
- Make at least two external servers load our page in an iframe, say jsbin, jsfiddle, or codepen

To test:

- Open any of the external URLs in a mobile browser.
- Type any text and see if the text is stored to localStorage or cookie by looking at the labels
- Open the other external URLs to see if the localStorage or cookie labels reflect what you typed previously
- Close and reload the tabs to test data persistence.
- Close and reload the whole browser to test data persistence.

### My Results:

In Mobile Safari:

| test | result |
|------|-----|
| cookie access? | NO |
| localStorage access? | YES |
| localStorage persist after tab close? | YES |
| localStorage persist across domains? | sometimes... |
| localStorage persist after browser close? | NO |
