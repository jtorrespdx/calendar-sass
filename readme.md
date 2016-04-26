Implementing bug fixes:
1. move these scss files to their correct directory.
2. Change the date/time format:
    1. On psoriasis.org (homepage), scroll down to the events listing. Hover your mouse over the first event, near the date, and click on the wheel (cog). Select "Edit view".
    2. Under "Fields", select "Content:Date and Time".
    3. Beneath the dropdown menu for "Choose how users view dates and times", select the blue link "Date and time settings."
    4. Select Formats.
    5. Select "+Add format"
    6. In the format string enter the following:
        <code>l, M j, g:ia</code> the first character is a lower case L, if you are wondering.
    7. Select "Save format".
    8. You should now be back in the "Date and time" page. Select "Types" and then "+Add date type"
    9. Under Date type, name it "Medium Abbreviated"
    10. Select the format that looks as follows, and be sure to save the configuration.
        >Monday, Apr 25, 4:30pm

    11. From the drupal admin bar, select Structure>views
    12. search for "homepage-event-calendar", and select edit.
    13. Under "Fields" select "Content:Date and Time"
    14. Under "Choose how users view dates and times:" select
    >Medium Abbreviated (Monday, Apr 25, 4:30pm)

    and then select "Apply".
    15. Clear all your caches.

    If you return to the homepage, you'll see that date and time has been fixed to be better accommodated within its allocated screen size.
