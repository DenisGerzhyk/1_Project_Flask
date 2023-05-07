# 1_Project_Flask

This is a Python code for a Flask web application. Here's a brief description of the code:

The first line of code imports the Flask framework and other necessary libraries.

The next line creates an instance of the Flask class and assigns it to the variable app.

@app.route('/') is a decorator that defines the route for the root URL of the web application. When the user navigates to the root URL, the index() function is called.

The index() function returns a rendered HTML template named 'index.html' using the render_template() function.

@app.route('/count', methods=['POST']) is a decorator that defines the route for the '/count' URL of the web application. This route only accepts HTTP POST requests.

The count() function is called when the user submits a form with the HTTP POST method to the '/count' URL. The text variable is assigned the value of the form input field named 'text'.

The number of words in the input text is calculated using the len() function and split() method, and stored in the words_count variable.

Finally, the count() function returns a rendered HTML template named 'count.html', passing the words_count variable as a parameter.

The if __name__ == '__main__': block is executed when the script is run as the main program. It starts the Flask development server by calling the run() method of the app object, with the debug=True option enabled. This allows for easier debugging during development.
