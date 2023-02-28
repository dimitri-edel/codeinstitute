I started with basic layout of the page, icluding responsive behavior.
Right off the gate I encountered a problem when testing the media queries in the browser using dev tools suite.
Found solution by googling : "chrome devtools device media query doesn't match the width".
Stackoverflow.com "Chrome Device Mode Emulation Media Queries Not Working"

Turns out that certain meta information for the viewport needs to be included in the head of the htmls file.
<meta name="viewport" content="width=device-width">
<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
From the meta information I take that the browser needs to know how to interpret the width parameter in the query.
So, it is necessary that it match the device screen width, or something like that.
