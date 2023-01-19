# What is Streamlit
Turns data scripts in shareable web apps in minutes using only python. NO FE knowlede required.

Streamlit is a platform (web app/server) that provides  an easy web to render charts and analize data.

Way of thinking: Streamlit is platform for develop multiple and individual apps (dashboard/python files)

## Data Flow
Streamlit apps work like normal Python scripts. When the screen needs to be updated, Streamlit runs the python script from top to bottom (all is executed)

Cases when the script is rerun:
- When the source code is modified
- When the user interacts with the charts, press a button, input text...
- Every time the dashboard is opened in the browser

Callbacks are available when interacting with the charts. 
Refer [Streamlit State API](https://docs.streamlit.io/library/api-reference/session-state#use-callbacks-to-update-session-state)

Cache data for the charts is also available 
Refer[Streamlit Cache API](https://docs.streamlit.io/library/get-started/main-concepts#caching)

## Display and style data
There are two ways:
- Use Magic
- Write a data frame 

### Use Magic
Streamlit detects data frames automatically and render them without specifying a chart

// Add snipet

### Write a data frame
Using `st.write()` can specify the data frame to be render as a chart.
This functionality support multiple graphic library like Matplotlib, Altait or Plotly

// Add snipet

When to use `st.write()`
- Magic and `st.write()` both detects the data frame and automatically choose the type of graph to render it. But if want to use a specific chrat type or add some functionality, `st.write()` allows it by supporting multiple libraries 
- Can manage objects returned bu other methods
- Can customize behavior and set multiple arguments 

