# gemini-prompt-for-apps-script
This prompt may be useful when using Gemini to assist in writing Google Apps Script. This prompt is a part of a workshop I developed called "Using Apps Script and Gemini to Build Custom Google Workspace Solutions".

Here is the starting prompt using Markdown. You will most likely need to view in RAW format before copying to paste into your GenAI.

-----------------------------------------------------------

I am a [beginner/intermediate/advanced] Google Apps Script coder. I need a script that [clearly and concisely describe the script's purpose].

Here's how the script should work:

* **Data Source:** [Specify where the script should get its data. E.g., "Data will be in a Google Sheet named 'Student Data' with the following columns..." or "The script should prompt the user for a date range."]
* **Process:** [Describe the steps the script should take. Be specific! E.g., "The script should filter the data to only include students in Grade 10. Then, it should create a new Google Doc for each student, with their name and grade level in the header."]
* **Output:** [Describe the desired outcome. E.g., "The script should create a new Google Doc for each student." or "The script should send an email to each teacher with a summary of their students' attendance."]

Please generate the Apps Script code following these guidelines:

1. **Thoroughly comment all parts of the script.** Explain what each function and section does.
2. **Use try/catch blocks for error handling.** This will make debugging easier.
3. **Use const as the keyword for variables that will not change. Use let for variables that can be reassigned another value. Do not use var to create variables.**
4. **Use the Logger service to log activity.** This will help me understand what the script is doing.
5. **Minimize calls to external services.** This will improve performance.
6. **Use batch operations when possible.** This will also improve performance.
7. **Avoid adding libraries if possible.** If a library is absolutely necessary, please clearly state this and provide instructions for adding it.
8. **Use the Cache service if appropriate.** This can help speed up the script.
9. **When suggesting edits to a function, provide the entire edited function.** This makes it easier to implement the changes.
10. **Use consistent indentation with [number] spaces.**
11. **Use meaningful variable and function names.**
12. **Group related code together.**
13. **Avoid unnecessary calculations and data fetching.**
14. **Optimize loops and use array methods where possible.**
15. **Provide specific and informative error messages.**
16. **Use defensive programming techniques to prevent errors.**
17. **Handle sensitive data responsibly and follow privacy guidelines.**
18. **Use the least privileged authorization scopes.**
19. **Write modular code with reusable functions.**
20. **Add clear documentation for complex logic.**
21. **Formatting for Google Sheet templates should have the first row frozen, bolded, with a gray background. Set column widths to 250 pixels. Wrap text in all cells. Remove any extra columns. Remove any rows over 100.**
22. **When creating custom menus, suggest a concise but catchy name for this tool.**
23. **

**Additional Requirements:**

* **Data Creation:** If the script requires specific data to function, please include a function to create the necessary files (e.g., a Google Sheet with the required columns).
* **Custom Menu:** The script will be run from a Google Sheet. Please include code to add a custom menu to the Google Sheet with the following options:
    * **Authorize Script:** This option should be visible only if the script requires authorization.
    * [Add any other menu items needed to run the script's functions]
    * 
