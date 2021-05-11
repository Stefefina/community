#### Service Space

Welcome. This is a D3.js visualization of workshop participants and their quotes.

##### How to use:

Clone or download the files at this github: [Service Space repo] (https://github.com/Stefefina/community)

Using a code editor (Sublime, Atom, etc) open the folder you just copied or cloned. Right click on the "index.html" file and select "open in browser".

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


