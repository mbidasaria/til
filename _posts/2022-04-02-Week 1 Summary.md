---
layout: post
title:  "Week 1 Summary"
---

Some Markdown using **tables** and **headings**

# Largest

___

### Third Largest

***

###### Smallest

---

| Header 1 | Header 2 |
|---|---|
|Spaces|before|
|or|after|
|pipes|is|
|optional|here|

http has 4 labels - one for each of CRUD:

post (for Create)
get (for Read)
patch (for Update)
delete (for Delete)

But HTML only has post and get so we get around that by using (only in .erb files)

`data-method="delete"` (method="delete" won't work)
`data-method="patch"`

But need **vanilla-rails** (has JavaScript to make above work) instead of **base-rails** 

---

Outside of forking repos from App Dev I/II, will use:

> mkdir dir-on-desktop-etc
> 
> cd dir-on-desktop-etc
> 
> open .
> 
> rails new app-name-here (once you install rails on computer, will general whole rails app w/ folders including public/log/config/bin/app + Gemfile, ReadMe, RakeFile)

**vanilla-rails** is above + niceties
**base-rails** is above - bunch of stuff taken out to simplify

Repo names above aren't industry standard, nor are RCAV, etc 

---

URL paths shouldn't have CRUD (e.g. `/create-exit`). All 4 should be `/exit`

---

Standalone button is just link with CSS (outside of a form)   

---

render statements can remove .html.erb (and will still work). Other extensions must be added.
 - Can include a different layout file (instead of application) using ... `:layout => "custom"` ... added to render hash

---

rails/db (where you'd normally type /git) gives you nice visual of database table
rails/info, rails/info/routes (shows routes I've defined as well as gems have defined)

---

`resources(:table_name)` - this one line will write the standard RESTful conventional 7 routes (1 create, 4 edits, 1 update, 1 delete). See rails/info/routes to see list. This types out routes, but not controllers, views obviously.

---

To use **instance variables** (`@variable`) need to use `render`, not `redirect`

---

Everything in Ruby is true except "false" and "nil". This includes 0, [], {}, "".
