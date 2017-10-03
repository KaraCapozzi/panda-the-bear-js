

1.  document.querySelector("img")
<img src=​"images/​self-portrait-grassbg.jpg" alt=​"Self Portrait" title=​"Self Portrait" class=​"profile-image">​

images = document.querySelectorAll('img')

document.querySelector("img")

profileImage = images[0]
profileImage.src = "http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"
"http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"



2.  heading = document.querySelector('h1')
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading.innerText = "Kara Capozzi"
"Kara Capozzi



3.  titles = document.querySelectorAll('.info-title')
(3) [h3.info-title, h3.info-title, h3.info-title]


titles[1].innerText = "Work"



4.  body = document.querySelector('body')  
body.style.background = 'blue'


5.  Change the colour of each element using the highlight class. Use a for loop to do this.

6.  Change the font family of the h1 to 'monospace'.

heading.style.fontFamily = 'monospace'
"monospace"


7. left = document.querySelector('aside')

var bigIcons = document.querySelectorAll('.action-icon-bg')
undefined
bigIcons[0]
<a class=​"action-icon-bg" href=​"#">​…​</a>​
big = bigIcons[0]
<a class=​"action-icon-bg" href=​"#">​…​</a>​
big.style.background = 'yellow'


8.  title = document.querySelectorAll('.bio-info-title')
(3) [span.bio-info-title, span.bio-info-title, span.bio-info-title]
title[0].innerText = 'Identify Yourself'
"Identify Yourself"


9. **** Change the placeholder attribute of the message field to "state your business".

message = document.querySelectorAll('textarea')
[textarea#message]


10.  
Give the name field a "value" attribute of "your nemesis".

11.  Change the value attribute of the email field to "koalathebear@gmail.com".

12.  Change the value of the submit button on the contact form to "En garde!".

13.  We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

14.  We should help Panda protect their privacy by erasing their personal details from the sidebar.
