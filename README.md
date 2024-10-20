# Hardcover Book Search and Add to List Web App
This html application allows Hardcover users to search for books and manage their reading lists by fetching user lists and adding new books to them. It utilizes the Hardcover API to access book data and manage user lists.
<p>Screenshots are attached at the end of this text.</p>

## Acknowledgments

This application is built upon queries made by [emgoto](https://github.com/emgoto). A React app version is also available on their [GitHub repository](https://github.com/emgoto).

## Features

- **Find User's Lists by Username**: Enter a username to retrieve their reading lists.
- **Fetch Current Books in a List**: Input a list ID to view the current books in that list.
- **Search for New Books**: Add new books to a list by searching for them using their title and author.
- **Display Search Results**: See search results with options to add books to the selected list.
- **User Notifications**: Receive notifications for successful actions or errors.

## How to Use

### Prerequisites

1. **API Token**: You will need an API token to access the Hardcover API. You can find this token in the settings under **Hardcover API**. The token should be in the format `Bearer <your_token>` (e.g., `Bearer abc123...`).
### Notice 
 Your API token need to be kept secure don't share it or the completed web app file to anyone. It's intended for personal use only with individual API keys entered.

### Step-by-Step Instructions

1. **Setup the HTML File**:
   - Copy the provided HTML code into a text editor and save it as `filename.html`.

2. **Replace API Token**:
   - Open the `filename.html` file and locate the sections of the code that contain the line:
     ```
     'Authorization': 'Enter your full api token with the single brackets with the word bearer included'
     ```
   - Replace the entire mock text (including `X` and the description) with your actual API token, ensuring it retains the format:
     ```
     'Authorization': 'Bearer <your_token>'
     ```
   - Repeat this for all five occurrences in the code.

   - Notice: Find and automatic replace might not work properly with notepad as all the characters in the token will not get pasted. 
   - You can keep track of the ones that need to be changed with the numbered - 'x.Replace with your actual token' comment that i have added beside 5 spots that need change.

3. **Open the HTML File in a Browser**:
   - Open the `filename.html` file using any web browser to access the web app.

### Using the Application

1. **Finding User Lists**:
   - Enter your username in the "Find User's Lists by Username" section.
   - Click the "Get Lists" button to retrieve and display the user's reading lists.

2. **Fetching Current Books**:
   - Enter the list ID of the list you wish to view in the "Fetch Current Books in List" section.
   - Click the "Fetch Current List" button to display the current books in that list.

3. **Adding New Books**:
   - In the "Add New Books" section, enter books in the format: `title1,author1; title2,author2`.
   - Tip-Ask ChatGpt or any LLM to format the list for you
   - Add a 5-8 books at a time to avoid being rate limited
   - Click the "Search Books" button to search for the specified books.
   - Review the search results and click "Add to List" next to the desired book to add it to the previously fetched list.

4. **Notifications**:
- Notifications will appear below buttons to indicate successful actions or errors encountered during processes.
- Click fetch current list after adding books to refersh it
- Click search books once again after adding to refrsh the Status and Position Columns 
## Additional Information

- This application is intended for personal use. Please adhere to the API usage guidelines provided by the Hardcover API.
- Please remember not to share your API key or completed file to anyone.

## Potential Errors
-If the book's name has some specil characters, it may fail to find the book sometimes.
-The App looks for the book with the most similar match with the most number of readers, but its not foolproof. If it's a niche book it might return a wrong book.

## Screenshots
### Getting to Api Key
 ![Getting to API Key](https://i.postimg.cc/4xBKtfGW/Screenshot-2024-10-20-200652.png)
 ![Getting to API Key](https://i.postimg.cc/XJc6GJSJ/Screenshot-2024-10-20-213534.png)
 ![Getting to API Key](https://i.postimg.cc/BvTVNVh7/Screenshot-2024-10-20-200732.jpg)

 ## Findidng Location of the Placeholder
![Getting to Key](https://i.postimg.cc/xTLp97Qf/Screenshot-2024-10-20-221515.png)

## Displaying Your Lists
![Getting to Key](https://i.postimg.cc/G2hnDRcx/Screenshot-37.jpg)
 
## Displaying Books in Your List
Notice- This List was Initially Empty. This screenshot is from after adding the books and refreshing the list by clicking fetch current list once more.
![Getting to Key](https://i.postimg.cc/xTHjn0qX/Screenshot-41.jpg)

## Searching and Adding Books
![Getting to Key](https://i.postimg.cc/MHM40KgV/Screenshot-40.jpg)

## Display after Resreshing Searched Books
Note- The Already added notification and red button will display after clicking it. The position and status updates only after refesh by clicking search books once again.
![Getting to Key](https://i.postimg.cc/CLJPZ8RX/Screenshot-42.jpg)

## Info
Hope this web app was of help to you. Please ping @Zoborist on Hardcover discord if you have any doubts or need help.
