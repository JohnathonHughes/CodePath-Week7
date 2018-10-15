# CodePath-Week7
Gifs and Readmes associated with wordpress 4.2 vulnerabilities

Exploit 1: Authenticated Stored Cross Site Scripting

1. Steps: 
  As a contributor or author level account with page editing/posting privledges, inserted formatted HTML on a page of post. When executed by an admin, the attack continues to server-side execution. On the newly editted page, a link appears that creates an alert on mouse hover.
  
2. Type of Vulnerbility: 
  Cross Site Scripting
  
3. Affected Versions: 
  All version up to and including 4.2.2
  
4. Source Code: <img src="exploit1.JPG" width="800">

5. Gif of exploit: <img src="gif1 XSS.gif" width="800">
      


Exploit 2: Authenticated Stored Cross Site Scripting in Youtube URL Embeds

1. Steps:
  Similar to the previous method, we abuse embeded shortcodes. In this case, the source link tried different regular expressions to find the appropriate one for the provided source link. Using flaws in the regular expression used with parsing youtube links, we can embed an HTML expression that passes through the autoembed method call to ultimately send an alert.
  
2. Type of Vulnerbility:
  Cross Site Scripting
  
3. Affected Versions:
  4.0 - 4.7.2
 
4. Source Code: <img src="exploit2.JPG" width="800">

5. Gif of exloit: <img src="gif2 XSS.gif" width="800">
