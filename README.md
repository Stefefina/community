#### Service Space

Welcome. This is a D3.js visualization of workshop participants and their quotes.

##### How to use:

Clone or download the files at this github: [Service Space repo] (https://github.com/Stefefina/community)

Open Terminal, find the directory/folder where you cloned or downloaded the files.
Use the following Terminal command to enter the folder
```cd```
Then check that you are in the correct directory by typing ```pwd``` in Terminal. This will print the the current directory/folder.
Making sure that you are in the proper directory, you will now run a server in order to see the visualization. In the Terminal
type the following ```python -V```
Here is a good reference in case: https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server

If your version of Python is anything starting with a 2.x then in the Terminal type ```python -m SimpleHTTPServer```
If Python version returned above is 3.X type ```python3 -m http.server```

Open a browser, and in the address bar type, ```localhost:8000```

You should now see the visualization in the browser.

#### How to update participant quotes list

Source for list is here: https://docs.google.com/spreadsheets/d/1IqV7vkQyIiQkLH3LjNUPZ61ceoyslpDrMcD_4tTlEuA/edit?ts=6098f932

1 In the Google Sheets document, all_profiles page, find the participant whose quote you want to use.
For that participant click on the checkbox on column "I", chosen quote.
Then copy and paste the desired quote to the cell on column J.
Example:
![Select participant quote](/documentation/select-quote.jpg "Select quote")

2) Switch to the sheet named participants_filtered.
 Exported participants_filtered as a CSV.
 ![Export quotes](/documentation/export-quotes.jpg "Export quotes")

3) Convert the CSV to a JSON file here: https://csvjson.com/csv2json
![Convert CSV to JSON](/documentation/csv-to-json.jpg "Convert CSV to JSON")

Copy and paste the content of the CSV and click on the "Convert" button.

4) Open the file participants.json, you will notice that this file is a JSON file. It contains an array called "children".
Paste the JSON array from step 3 above into this file.


