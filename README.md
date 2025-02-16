# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to the `innerHTML` property in HTML.  The bug showcases how repeatedly setting `innerHTML` can lead to unexpected results and potentially introduce security vulnerabilities if used improperly.

The bug occurs because setting `innerHTML` overwrites the entire content of an element.  The example initially adds a paragraph, but the subsequent `innerHTML` assignment completely replaces it. This behavior differs from appending, where we might expect to add to the existing content.  This can cause issues in more complex scenarios, especially when manipulating dynamic content.   This is less common than other `innerHTML` related vulnerabilities like XSS but is still crucial to understand to build robust, maintainable code.