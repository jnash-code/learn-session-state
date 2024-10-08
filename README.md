# Fist Part
## Explanation
First run: The first time the app runs for each user, Session State is empty. Therefore, a key-value pair is created (`"counter":0`). As the script continues, the counter is immediately incremented (`"counter":1`) and the result is displayed: "This page has run 1 times." When the page has fully rendered, the script has finished and the Streamlit server waits for the user to do something. When that user clicks the button, a rerun begins.

Second run: Since "counter" is already a key in Session State, it is not reinitialized. As the script continues, the counter is incremented (`"counter":2`) and the result is displayed: "This page has run 2 times."
