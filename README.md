# giststest
This code is a JavaScript script that allows you to search for a user's information and gists on GitHub using the GitHub API.
When the user enters a username into the input field and clicks the search button, the script will first clear any previous search results from the page.

It then makes a GET request to the GitHub API to retrieve information about the user, including their avatar, name, bio, and various statistics about their account. This data is then used to create and add an HTML element to the page, displaying the user's information.

Next, the script makes another GET request to the GitHub API, this time to retrieve the user's gists. For each of the gists returned, it creates another HTML element that displays the filename, description, and creation date, and then makes another GET request to the GitHub API to retrieve the raw data of the file, using this data to append the raw data to the HTML element.

Finally, it appends each of the created HTML elements to the gists container on the page. If there's an error in the request, it will display an alert message on the screen.
