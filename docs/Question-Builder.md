---
layout: default
title: Question Builder
nav_order: 20
---

# Question Builder

Users who can make changes in the Application Builder are also able to access the Question Builder while the Application Notice is in Draft format.  

To access the Question Builder click the 'Questions' or 'Item Questions' button beside the area you wish to maintain.  This will open a window that shows the Question Groups available to use for this area, with groups that have been selected for use on this document at the top of the page in sequence order.  The +/- beside the group name allows you to view the text of each entry and some details about it.

Any Question Group displayed can be selected for use on the current document, but only groups that have been selected for use on this document and are not in use on any other document can be altered here.

Clicking either 'Add Question Group' or 'Copy Group' opens a window where either a new group can be added or an existing group can be copied.  When the new group is created the main Question Builder page will refresh and the new group is available to select and then modify if desired.
Clicking the group's name opens a window where the name can be changed or the entire group deleted.  Clicking 'Add Question' or 'Edit' opens the Question maintenance screen.

The Question Maintenance screen is where questions can be added, edited, and deleted.
Selecting a Question Type from the dropdown shows only the fields that are relevant to that type of question and pre-sets some values to make adding the question simpler:  for example, selecting the 'Yes/No - Radio' Question Type allows the user to be sure the display will be radio buttons with the labels 'Yes' and 'No' while selecting 'Input Field - <= 64 characters' will display an input field that allows only 64 characters.

Some Question Types have additional information that appears in the HTML Misc field.  This text will over-write whatever is in that field when the relevant Question Type is selected. 
For the most part this text should not be altered, with the following exceptions:
 - Textarea:  the number of cols and rows can be changed, but be aware that making the field much wider (cols) or longer (rows) will impact the display and usability of the page.  The number value in the limitText javascript can be changed.  This is the number of characters this field will allow to be typed in.
 - Input Field:  the size and maxlength can be decreased but should not be increased.  Size should be the same as or smaller than maxlength.  This applies to all the 'Input Field' types.
 - Multiple-select checkbox:  columns2 and columns3 are supported.  This is the number of columns the entries will be divided between.  It is generally best if questions with more than 10-12 entries use columns3.

Some Question Types require a Linkvalue (Multiple-select checkbox, Dropdown, and Radio) to be selected.  This is the table that provides the options for the users to choose among.

The 'Other' Question Type is a special case.  This will be the selected option for questions that were created outside of this new facility and should only rarely be used otherwise, and only for question types that do not fit any of the usual types used for the Applications.

The Question Types in the dropdown have been ordered by the apparent frequency of use in the current Discretionary Applications, but can be re-ordered if desired.
