<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(`${title}`);
  } 
  tR += "---"
%>
author:  Adge Denkers | https://github.com/adgedenkers
project: Python Examples
subject: <%* tR += `${title}` %>
created: 
---

# <%* tR += `${title}` %>

Hello there. 

<%* tp.file.cursor() %>
