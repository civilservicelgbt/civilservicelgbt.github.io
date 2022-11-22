---
layout: manual
title: Managing email alerts and registration information
excerpt: This guidance explains how to send an email alert using GOV.UK Notify,
  and how to maintain the email lists.
meta-info: "false"
---
## Adding someone to the email alerts list

C﻿ivil servants can register for email alerts by completing a form at [www.civilservice.lgbt/email-alerts](https://www.civilservice.lgbt/email-alerts)

T﻿he visible form on the website is linked to a [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe_x2T2kG1vEhlca2dvYlv7c_EnmaC8EmWiFX43mzgh7ZA28Q/viewform) that is linked to the Civil Service LGBT+ Network's Google Workspace account. T﻿he Google Form is linked to a [Google Sheet](https://docs.google.com/spreadsheets/d/1V5hQQ_ejKvwZVDO1viFL3SwKmbE3VLj9VczGjmShHJ4/edit#gid=1174852171) document in the Civil Service LGBT+ Network's Google Drive. Every time someone submits the form, a row is added to the Google Sheet.

{:.warning-text}

> **Do not change the content of the registration form.**
>
> ﻿ The form that appears on the website was custom coded so that it looked consistent with the rest of the site. If you change the Google Form, the website registration flow might break.
>
> ﻿ If you want to make changes to the forms, you should ask a developer familiar with HTML, CSS and Javascript to help you.

## Removing someone from the email alerts list

You must remove someone from the email list if they request it. 

To remove someone from the list.

1. [Open the Google Sheet](https://docs.google.com/spreadsheets/d/1V5hQQ_ejKvwZVDO1viFL3SwKmbE3VLj9VczGjmShHJ4/edit#gid=1174852171)
2. Go to the `Members` tab
3. Search for their email address
4. Highlight the row and delete the row from the spreadsheet

**Never act on a request if you cannot confirm the user is who they say they are.** Before you take action on their request, you should check that the person making the request is the same person that registered. You can do this by checking the email address from which the request was sent against the emails we hold.

## A﻿mending someone's information

**N﻿ever amend someone's details on the email lists directly.** It is very easy to make a mistake that might accidentally reveal personal data. 

I﻿f you receive a request from someone to amend their data:

1. Inform them that we do not amend existing information to ensure the integrity of people's data
2. Inform them that you will delete their existing information
3. Ask them to register again via the online form with their updated details

## C﻿leaning the email lists

You should regularly review the email list for SPAM. These are usually identifiable by incomprehensible strings of characters in the Members tab of the Google Sheet. If you find any, delete them.

## S﻿end an email alert

W﻿e use GOV.UK Notify to send email alerts to people on the lists. You can use the [tools on the Civil Service LGBT+ Network website](https://www.civilservice.lgbt/tools) to generate the content of an email alert.

**E﻿mail alerts are not the same as newsletters.** GOV.UK Notify is designed for "transactional" email – these are emails that are automatically generated in some way to \_notify\_ the recipient of activity they might care about; like new blog posts, a password reset email, and so on. Newsletters from staff networks tend to be discursive and informal. Email alerts are structured content that is sent in a semi-automated way. You must not send informal email via this system or you may be removed from the system.

**Email alerts must only contain information that is available publicly.** Essentially, if it isn't a published post or event on our website, you can't include it in the email alert. You also can't send images or attachments – meaning anything you want to include must be linkable to somewhere on the internet. The tools that generate the content of an email alert on our website will help to ensure your content is compliant with GOV.UK Notify norms and rules.

Before you send an email alert, decide who you need to send it to. This could be:

* everyone on the email alerts list
* a﻿ subset of people on the email alerts list, filtered by region, nation or interest

Once you have decided who your audience is:

1. [Open the Google Sheet](https://docs.google.com/spreadsheets/d/1V5hQQ_ejKvwZVDO1viFL3SwKmbE3VLj9VczGjmShHJ4/edit#gid=1174852171)
2. G﻿o to the `Choose data` tab
3. Select the audience you want from the drop down menu
4. Go to the `Data to export` tab
5. Select `File > Download > Comma-separated values (CSV)`

T﻿his will download the names and emails of the people you will send the alert to on to your local machine. Rename the file to something descriptive – like "25 Nov 2022 – All members alert.csv".

U﻿se [the email alerts tools](https://www.civilservice.lgbt/tools) to generate the content of your email alert; select the type of alert you want to generate, then choose the updates and events you want to include by selecting the tick-boxes next to each item. Use the step by step instructions on the tool page to send the email.

{:.warning-text}

> **Only recent items appear on the tools**
>
> ﻿ Blog posts and publications from the last 2 months, and events taking place in the next 2 months will appear in the tool. If you want to include something further out, you'll need to amend the content of the alert before you send it.

### After you've sent an email alert

After you have sent an email alert, you will see a report about whether the email was successfully sent or not. This includes a number of 'failed' deliveries. You should check the failed list each time you send an email. If any email fails, you should remove it from the email alerts lists we hold.

You will also receive one or two requests to be removed from the list each time you send an email – this is normal. If this occurs, follow the process from removing someone from the list above.