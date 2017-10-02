

document.querySelector("img")
<img src=​"images/​self-portrait-grassbg.jpg" alt=​"Self Portrait" title=​"Self Portrait" class=​"profile-image">​

images = document.querySelectorAll('img')


Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

document.querySelector("img")

profileImage = images[0]
profileImage.src = "http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"
"http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"



Select the heading that says "Panda the Bear" and change it to your own name.

heading = document.querySelector('h1')
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading.innerText = "Kara Capozzi"
"Kara Capozzi





Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)


titles = document.querySelectorAll('.info-title')
(3) [h3.info-title, h3.info-title, h3.info-title]


titles[1].innerText = "Work"

Change the colour of the body.

Change the colour of each element using the highlight class. Use a for loop to do this.

Change the font family of the h1 to 'monospace'.

Find a way to select the round icons in the sidebar and then change their colour.

Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

Change the placeholder attribute of the message field to "state your business".

Give the name field a "value" attribute of "your nemesis".

Change the value attribute of the email field to "koalathebear@gmail.com".

Change the value of the submit button on the contact form to "En garde!".

We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

We should help Panda protect their privacy by erasing their personal details from the sidebar.
