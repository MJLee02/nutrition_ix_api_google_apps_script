# nutrition_ix_api_google_apps_script
A Google Apps Script that allows you to pull nutritional information from NutrtionIX in Google Sheets. Tutorial on how to use this script is contained in the README file

# Here is how to set up this function in Google Sheets:
1. Open Google Docs
2. Navigate to Apps Scripts (Extensions > Apps Scripts)
3. Delete everything in the file and copy & paste the contents of getNutritionLabel.txt into your editor
   - How to get to the editor: This should appear when you first get into Apps Scripts
   - If you accidentally navigate out, hover your mouse over the "<>" icon on the far left side of the screen
   - Click Editor and then Code.gs (Editor > Code.gs)
   - Now proceed with Step 3
4. Save the file (Mac: Command + S; Windows: Ctrl + S)
5. Run the code (this step is a bit more involved):
   - Hover over the toolbar on the far left side of the screen (this contains the "<>" icon)
   - Click "Triggers"
   - Click "Add Triggers"
   - Make sure the information in the pop up window matches the following (see image.png for reference):
     - Choose which function to run: getNutritionLabel
     - Choose which deployment should run: Head
     - Select event source: From spreadsheet
     - Select event type: On edit
     - Failure notification system: Notify me daily
   - Click save
   - Login with your Google Account
   - If you are NOT a verified Google App Developer (which is very, very likely) do the following:
     a. Click "Advanced" (its in the bottom left corner of the pop-up window)
     b. Click "Go to Untitled project (unsafe)" <- Note that this is perfectly safe.

# Now you're done! You can call this function using =getNutritionLabel() to pull data from NutritionIX

# Note that this will output serving size (g), calories, calories from fat, total fat, saturated fat, trans fat, cholesterol, sodium, total carbohydrates, dietary fiber, sugar, and protein IN THIS ORDER. If you want different information, feel free to either edit the script or ask ChatGPT to make changes. ChatGPT tends to be very good at writing Google Apps Scripts.
