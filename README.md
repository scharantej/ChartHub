## Flask Application for Stock Price Chart Chatbot

### HTML Files
- **index.html**:
   - Main page of the application, used to interact with the chatbot.
   - Contains a text input field for the user to enter stock names.
   - Includes a button to trigger the creation of a stock price chart.
   - Displays the generated chart, if any.
- **chart.html**:
   - Used to display the stock price chart.
   - Receives the stock price data from the server via a Flask route.
   - Contains the necessary JavaScript and HTML elements to create the chart.

### Routes
- **`/get_stock_prices`**:
   - Handles GET requests and retrieves stock price data for the given stock name.
   - Uses a stock API or financial library to obtain historical prices.
   - Returns the JSON response containing the stock price data.
- **`/create_chart`**:
   - Handles POST requests and generates a stock price chart using the received data.
   - Creates a static image or interactive web chart using a suitable charting library.
   - Returns a redirect to the `chart.html` page, passing the chart URL as a query parameter.