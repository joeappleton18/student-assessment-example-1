# Github URL
https://github.com/Smadger1/WebDev-Assignment-1

# Hosted at 
https://smadger1.github.io/WebDev-Assignment-1/index.html

# Background
The problem I was attempting to solve with this project was to create a single place where all our meeting room bookings were available. We have several different venues throughout the borough where we offer bookings for people to hold events/meetings and there was no single place to access all this information.

# Wire Frames
**Main page wireframe**

This is a rough lookup of what I want my main page to look like when completed
![](https://i.imgur.com/8gdGRve.png)![](https://i.imgur.com/g9MnJmL.png)

**Information Page**

Here is an example of what I want one of my information pages to look like. There will be an enquiry page for every location with different text and pictures on each. However, the general layout for each will be the same.
![](https://i.imgur.com/0WCEj70.png)![](https://i.imgur.com/maMG1Ri.png)

**Enquiry Page**

This is what the enquiry page/form will look like when roughly laid out. This will be the form that a user submits to enquire about a booking.
![](https://i.imgur.com/ZmlSfc4.png)![](https://i.imgur.com/pozxzce.png)

**Enquiry Page after submission**

Here is the enquiry page with the modal I want to appear on top to show that the form has been submitted.
![](https://i.imgur.com/wREw0lQ.png)![](https://i.imgur.com/V0KHRn6.png)

I will explain further under the GDPR section as my pages for GDPR etc are all already on our main website (https://eastleigh.gov.uk) so I just link through to them directly as we want a single place to update in future if we change any of our privacy policies etc. Therefore, I didn't need wireframes for them as they already contained the information and I would have no involvement in them.
# Colour Choices

The colour choices for this website were easy to decide upon as this website had to fit in with our already existing theme (visible at https://eastleigh.gov.uk). The main colour throughout the website is white with all text other than the logo in black, this means it is easily viewable on all monitors regardless of any sight issues.

Then I used green as an accent colour just like our main website in order to keep the theming consistent.
# Accessibility

When it comes to Accessibility, I have tried my hardest to make the website as accessible to as many people as possible. All pictures have text alternatives in case a user cannot view the picture. Also, text is black on a white background with easily readable fonts and in a reasonably large size so anyone who has a trouble viewing small text or fancy fonts or clashing colours shouldn't have a trouble here. As well as this I have ensured that there is proper tab support so you can navigate the entirety of my website with only a keyboard, so you do not need a mouse. Finally, there is no auto scrolling content so users who are slower at reading or struggle with taking in information have as much time as they need to view the content.
# GDPR

I have tried my hardest when creating this website to ensure that I keep to the GDPR guidelines with specific attention paid to the 8 rights provided by GDPR.
One thing of note is that as this is going to be an addon to our already existing website I have linked to our Privacy policy in the footer of every one of the pages to ensure that every user has ample opportunity to read its content.
All eight rights are clearly explained in our Privacy policy and as the form currently does not submit anywhere, I do not have to implement any systems for automatic deletion of data etc. However, when we release this website the forms will submit into our backend Salesforce system where all of our automatic data deletion is handled for us so there was very little to do GDPR wise in this website.
# Distance Selling

Distance selling is a bit of a grey area on my website as I don't directly provide any way for a user to purchase anything as it is just an enquiry form. As well as this all the information should be provided when the user gets contacted by a member of staff about their enquiry. However, I still made sure to provide as much information when possible such as descriptions of the rooms and our business name, contact details and address.
# Evaluation

When developing this website, the hardest part was finding out a valid project to take on. I had to speak to many different people across my organisation and eventually came across this idea.

The first thing I did was create the basic wire frames taking inspiration from our parent website (https://eastleigh.gov.uk) along the way. I needed the look and feel of both websites to be identical so you wouldn't even know that you had gone from one to the other to ensure a solid user experience.

Once I had designed the wireframes, I started by creating the header and footer in the main page so I could get the look and feel I was after locked down. Once I had the header and footer made, I started work on the slideshow element of my main page. There were a few different versions of the slideshow before I eventually created the final version. I originally tried adding hidden and shown classes based on what next button you click but eventually found out that just manually changing the display style element to be the easiest.

Once I'd designed the slideshow element, I then created my content for my main page and then copy and pasted the layout for each of the "viewing" pages for each site. Here I then filled out the content for each of the pages and got pictures for the slideshows for each meeting site.

Then I designed the enquiry form for each of the different sites. Once I'd designed the forms, I added some validation to ensure that you couldn't submit without entering a valid email etc. Finally, I added the animated modal using the amazing https://sweetalert.js.org/ library.

Once I'd built my website, I went across it on my main PC going to each of the different pages and ensuring that all the content was correct, and everything worked as expected. I found a few bugs at this stage with silly things like spelling mistakes and copying and pasting of incorrect titles.

Once I'd fixed the minor bugs I then tested on my mobile phone (Pixel 3XL) to ensure that there weren't any unknown bugs when it came to being resized. Here I found a couple of bugs, the first being that the next and previous buttons would overlap the main title of the pages. This was an easy fix and adding a top margin to the context header div pushed it down far enough for it to not be a worry. Once I'd fixed this, I found out that the submit button was static at 910px instead of dynamically shrinking along with everything else on the page. This was an easy fix by setting the max width of the button to being 910px and making its width to 100%. This will ensure it's never any bigger than the desired 910px but if the page gets smaller it will shrink with it.

Other than those bugs that was really the only problems I encountered after I was finished development.

The only thing missing on the website is that the forms do not actually submit. The reason for this is that this was simply beyond what was desired for the project and would require major backend development in our Salesforce environment with process mapping and a whole new process and training. It simply wouldn't have been possible in the timeframe and we already have a form system which integrates with Salesforce so would want to use that instead of the form I designed.
