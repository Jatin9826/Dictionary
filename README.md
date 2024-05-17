# Dictionary
Dictionary using html , css  , java-script

![Screenshot 2024-05-16 201321](https://github.com/Jatin9826/Dictionary/assets/167497208/f95094d7-df92-4b18-86d5-df4bd3ffa0cd)


#logic 

1. **Retrieve Input Elements**:
   - Get references to the input, button, and display elements from the DOM.

2. **Set Up Event Listeners**:
   - Add a click event listener to the search button to trigger a search when clicked.
   - Add a keyup event listener to the search input to trigger a search when the Enter key is pressed.

3. **Define the Search Function**:
   - Extract and trim the search term from the input field.
   - Check if the search term is empty. If it is, alert the user and return.

4. **Fetch Dictionary Data**:
   - Define an asynchronous function to fetch data from the dictionary API.
   - Try to fetch data from the API using the search term.
   - Handle errors by alerting the user if the fetch fails.

5. **Handle API Response**:
   - Parse the JSON response from the API.
   - Pass the parsed data to the function that handles displaying the results.

6. **Display Search Results**:
   - Show the result container.
   - Extract relevant data (word and meanings) from the API response.
   - Populate the result container with the word and its meanings, including part of speech and definitions.

7. **Add Event Listener for Audio Button**:
   - Add a click event listener to the audio button to trigger speech synthesis when clicked.

8. **Define the Speak Function**:
   - Extract and trim the search term from the input field.
   - Check if the search term is empty. If it is, alert the user and return.

9. **Speech Synthesis**:
   - Create a new SpeechSynthesisUtterance instance with the search term.
   - Set the language, volume, rate, and pitch for the speech.
   - Use the Web Speech API to speak the word.

10. **Error Handling**:
    - Alert the user and log errors to the console in case of issues during data fetching or other operations.
      


note: const response = await fetch(`https://api.dictionaryapi.dev/api/v2/entries/en/${searchTerm}`);    
# this is the main to connect the dictionary with api in java-script

 
note:<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA==" crossorigin="anonymous" referrerpolicy="no-referrer" />   
# this is the main line in html for the audio 
