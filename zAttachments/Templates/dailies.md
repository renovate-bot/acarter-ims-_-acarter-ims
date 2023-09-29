---
tags:
  - dailies
---
## <% moment(tp.file.title, "YYYY-MM-DD").format("dddd Do MMMM YYYY") %>
<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>]] >>
> [!Quote]+ Quote of the Day
> <% tp.web.daily_quote() %>


```dataview
Table without ID L.text As "Today's Goals"
From #dailies 
FLATTEN file.lists As L
WHERE meta(L.section).subpath="Action Plan" and file.name= "<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>"
```
---


> [!tip]+ Habit Tracker
> Sleep:: 0
> Reading:: 0
> Exercise:: 0
> Meditation:: 0
> Writing:: 0


> [!abstract]+ What am I grateful for?
> - 1
> - 2
> - 3
