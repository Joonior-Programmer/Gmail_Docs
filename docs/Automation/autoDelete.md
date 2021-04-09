---
layout: default
title: Setting Up Auto Deletion
parent: Email Automation
nav_order: 2
---

# Setting Up Auto Deletion

Set up your inbox to automatically delete marked emails after a time period. If you don't feel comfortable working with code, then feel free to ignore this feature

---

## Setting Up The Script

1. Access <a href="https://script.google.com" target="_blank">Google Scripts</a>

2. *Left Click* on **New Project** in the sidebar

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/createScript.png?raw=true">

3. *Delete* the starting code and paste the code below into the file

    ```js 
    function auto_delete_mails() { 
            var label = GmailApp.getUserLabelByName("Delete Me"); // A label that signifies emails marked for deletion 
            if(label == null) { 
                GmailApp.createLabel('Delete Me'); 
            } else { 
                var delayDays = 2 // Number of days before messages are moved to trash 
                var maxDate = new Date(); maxDate.setDate(maxDate.getDate()-delayDays);
                var threads = label.getThreads(); 
                for (var i = 0; i < threads.length; i++) { 
                    if (threads[i].getLastMessageDate()<maxDate) { 
                        threads[i].moveToTrash(); 
                    }
                } 
            } 
            }
    ``` 

4. *Type* in some words between the quotation marks for the label name that marks them for deletion

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/scriptCode.png?raw=true">

5. *Type* in the number of days before a message with the label will be auto deleted in the red box below the label name

6. *Left Click* on "Untitled File" in the top left corner to change the name of the file

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/nameScript.png?raw=true">

7. *Type* in the name and *Left Click* **Rename** to save changes

6. *Left Click* **Triggers** in the sidebar

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/triggerScript.png?raw=true">

7. *Left Click* **Add Trigger** on the bottom right

8. *Set* the options to be the same as the picture shown below, or change to your liking if you understand their function. See the <a href="https://developers.google.com/apps-script/guides/triggers/installable">Official Google Documentation</a> for more information

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/scriptOptions.png?raw=true">

9. *Left Click* **Save** at the bottom (If you run into some errors in this step, refer to our troubleshooting guide)

---

## Deleting Scripts

1. Access <a href="https://script.google.com" target="_blank">Google Scripts</a>

2. *Left Click* **My Triggers** on the left sidebar

3. *Left Click* the **Three Dots** on the right of the trigger and then click **Delete Trigger**

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/deleteTriggerWarning.png?raw=true">

4. *Left Click* **Delete Forever** when the warning appears

---