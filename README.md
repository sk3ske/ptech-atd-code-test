# ptech-atd-code-test
Code test for potential Prodtech Assistant TDs

Please fork this repo and issue a pull request. The repo contains a .pickle file containing data to be used, and .py files needing to be updated for 2 of the questions. When you have completed all 3 questions, commit your 1 new file, and changes to the 2 existing .py files and push them back to github for review.

2) basic_dialog.py currently defines a PyQt4.QtGui.QDialog with only an ok and cancel button that returns no information. Install PyQt4, then add the following 4 widgets to the dialog:

- A QLineEdit labelled Name
- A QComboBox labelled Type with the options A, B, C
- A QDateWidget labelled Need By - This should default to one week in the future, and the user should not be able to enter a date in the past
- A QTextEdit labelled Notes

Then update getValues to query the widgets for their values, and return a dictionary where the keys are the widget labels, and the values are the information currently entered into the widgets.
