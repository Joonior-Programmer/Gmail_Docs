---
layout: default
title: Setting Up Auto Deletion
parent: Email Automation
nav_order: 2
---

# Setting Up Auto Deletion

Set up your inbox to automatically delete unwanted emails after a time period. If you don't feel comfortable working with code, then feel free to ignore this feature

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
    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/scriptCode.png?raw=true">


4. *Type* in some words for the label name between the quotation marks to mark them for deletion

5. *Type* in the number of days before a message with the label will be auto deleted in the red box below the label name

6. *Left Click* **Triggers** in the sidebar

7. *Left Click* **Add Trigger** on the bottom right

    <img src = "https://github.com/Joonior-Programmer/Gmail_Docs/blob/master/assets/images/automationImg/triggerScript.png?raw=true">

---