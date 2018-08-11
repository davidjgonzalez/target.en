---
description: Information about the global mbox, a name used to refer to the single server call made at the top of each web page in your Target implementation.
keywords: global mbox;implement mbox.js;implement at.js
seo-description: Information about the global mbox, a name used to refer to the single server call made at the top of each web page in your Target implementation.
seo-title: Understanding the Global mbox
solution: Target
subtopic: Getting Started
title: Understanding the Global mbox
topic: Standard
uuid: 978bd562-92e5-4175-a866-b2a8825f67bc
index: y
internal: n
snippet: y
translate: y
---

# Understanding the Global mbox

By default, the global mbox is named [!DNL  target-global-mbox]. It can be renamed for your account, if necessary. 

There are several differences between a regular mbox (non-global mbox) and the global mbox, including: 



<table id="table_D849378A87FE478487DA11581D274F61"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Regular mbox </th> 
   <th colname="col2" class="entry"> Global mbox </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>A regular mbox typically wraps around content with a <span class="codeph"> &amp;lt;DIV&amp;gt; </span> tag. </p> </td> 
   <td colname="col2"> <p>The global mbox is "empty" and does not wrap around any content. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Content from only one activity can be delivered in a regular mbox. </p> </td> 
   <td colname="col2"> <p>Content from multiple activities can be delivered in one response to a global mbox. </p> </td> 
  </tr> 
 </tbody> 
</table>

If multiple activities are delivered via the global mbox or via multiple regular mboxes, [!DNL  Target] [ determines the priority ](c_priority.md#concept_1780C11FEA57440499F0047DD6900E0F) by which the activity (or activities) are delivered to a web page. 

Additional page-level data can be sent to [!DNL  Target] along with the global mbox by using the ` targetPageParams` function. This is similar to the mbox parameter functionality. For more information, see [ Passing Parameters to a Global mbox ](c_pass_parameters_to_global_mbox.md#concept_33362A04146C4E3C8E7089B65F38B5E5). 