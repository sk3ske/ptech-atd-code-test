# ptech-atd-code-test
Code test for potential Prodtech Assistant TDs

#Instructions
Please fork this repo and issue a pull request. The repo contains a .pkl file containing data to be used, and .py files needing to be updated for 2 of the questions. When you have completed all 3 exercises, commit your 1 new file, and changes to the 2 existing .py files and push them back to github for review.

**1)** Write a script that exports the data in a Python dictionary to Microsoft Excel in spreadsheet format. The dictionary is the result of a database query and is provided to you in pickle file called test_data.pkl. The spreadsheet should include columns for Task Name, Set Part Name, Parent Build Name, Start Date, and End Date. The data should be sorted by earliest Start Date first. If a Due Date has already passed, shade the entire row red in Excel.

You'll need to install and use an external Python library to handle the Excel import. Two options that we use are xlsxwriter and xlwt, both available for free online.

The database returns unfriendly key names for some fields. We map these keys to the above listed human-readable fields in the following way:

Task Name = 'content'

Set Part = 'entity'

Parent Build = 'sg_parent_build'

Start Date = 'start_date'

End Date = 'due_date'

**2)** basic_dialog.py currently defines a PyQt4.QtGui.QDialog with only an ok and cancel button that returns no information. Install PyQt4, then add the following 4 widgets to the dialog:

- A QLineEdit labelled Name
- A QComboBox labelled Type with the options A, B, C
- A QDateWidget labelled Need By - This should default to one week in the future, and the user should not be able to enter a date in the past
- A QTextEdit labelled Notes

Then update getValues to query the widgets for their values, and return a dictionary where the keys are the widget labels, and the values are the information currently entered into the widgets.

**3)** email_gen.py is a Python script that parses the same pickle file from Test 1 and generates an email body string which is printed to the terminal. There are three bugs in the script. Find and fix all three bugs. Describe the bugs and how you fixed them in comments.

..
...
