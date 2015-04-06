1. Title
The title of the course.

2. Welcome
Welcome people to the course, introduce yourself.

3. History (optional)
If needed, can give a history of where ____ came from, how it got started, why we are using it now.

4. Final State of App
Start the course off by showing what you are going to create by the end. Explain the app at a very high level and click through it a bit. If this is not the first section, then here is where you often will show the state of the application where we left off.

5. Problem

  - list of steps
  - mini problems (have Jon explain more)

6. Concept
7. Solution
8. Wrap Up

5-6-7 can repeat
6 is optional and used when the problem is complicated enough that showing it at the conceptual level would be helpful for students to understand what's going on


Users, like players on game board, must be guided.

We guide Users through, what could be treacherous User Experience waters, to what hopefully is, a beautiful, calming and successful experience.

On the Interwebs, we have things like CSS Animations to help aide us in guiding Users.

For example, on our WYSIT game site, our Users will have multiple goals set out before them — Understanding the game, Purchasing the game, and communicating with other game players.

It is our job as the web designer to distinguish *which* of these goals are most important to our User and create a UI that will guide them to that goal.

Purchasing the Game is top priority. IF the User does not own the game, how can they play it or commun with other players?

We can Use CSS Transitions to make buying the game a prominent call to action on our page. Then once they have selected that call to action, we can again use CSS Transitions to bring the purchase form on screen smoothly and with a subtle flair.

Using animations on a site not only guides the user and gives them feedback, but it also adds personality to a site. If you can bring a spark of joy or wonder to a User — or even perhaps a small smile, you have won. They will be more open to ideas and more forgiving to bugs. There is no better place to have a User.


So let us begin -

## USing CSS Transitions to create a Prominent CAll to Action
## USing CSS Transitions to bring a form on screen
## USing CSS Transitions to bring an overlay

## Form things at this point


1. title
2. welcome
3. final site we are building
(transition) but we need to start small
4. product pg with a CTA (problem)
- at this point animations are not there (Why)
- we need to call the users attention to the main call to action and also provide them feedback that this is clickable
5. Solution change color of btn on hover
- when we are changing transitions we are changing values from one value to another
- `.button { transition: background-color 2s; }`
  - animated arrows come in and explain syntax
6. Another example
7. In fact this follows the syntax you will see here with transitions
8. we just looked at three things that can be trans. what all properties can be transitioned
- exp. how to determine on your what can be transitioned
- check out whatever.com to see the up to date list
last. now if you went searching for transition you might notice this last opt propterty called delay, not the best idea why

List of Constraints
Level 1 need:
- My example: CTA on a product page
everything will be ok though as long as I have:
- Distilled [drawing attention to the element as the user interacts with it]


- pngs
- svg
- show the power of animating an svg vs png


History: might fit in well with the SVG level


---

hi!  Sorry I'm just linking to this now, it was a very long afternoon of meetings for me.  Here's that "constraints" document we talked about today for Front-end Foundations https://github.com/codeschool/FrontEndFoundationsCourse/blob/master/content-book/site_reqs.md

For each level, I broke it down into an Overview of what the site would need to contain at a minimum for that level, and then I also split it into Stages, which was just my word for saying "in general, here's the order that I'll introduce this stuff"

it was sort of a wild guess at that point though, and if you compared this to what the final version of the course ended up being there's a few differences.  One of the big ones is that at this early stage I was thinking that Level 1 was an intro to HTML + CSS, but in the final course Level 1 was just HTML and Level 2 was just CSS.

so yeah, just one example of one way to communicate with front-end/design teams so they understand what you need and a really quick "why"

I was looking for examples of that "mini problem" thing we were talking about earlier too and I found one or two other things to point out

first, I found a pretty good mini section in Try jQuery that kind of illustrates what we were talking about.  If you check out Slide 3, the problem is introduced in a little video with some dialogue like "we want to be able to click the Get Price button and have the button replaced with the actual selling price, let's look at how we can do that with a jQuery event handler..."

Then slide 4 starts solving the problem by introducing two concepts with syntax - the first concept is the document.ready, and the second one is the on() function for event handling.  Then slide 5 combines the two together to say "add the on() handler when the document is ready", and then Slide 6 solves the remainder of the problem (append and remove were covered in a previous section)

finally Slide 7 shows the full working example again and the section is over

so yeah, just an example of a pretty natural way that you can sort of combine concepts and syntax together and reveal them one after another over a few slides to solve a problem
try-jquery-example-1  
file:///Users/alyssanicoll/Downloads/try-jquery-example1.pdf

here's the slides I'm talking about:

Next, here's another example that sort of matches up with what I was calling the "mini problem"
try-jquery-example2.pdf  
file:///Users/alyssanicoll/Downloads/try-jquery-example2.pdf


the overall problem here is "how to implement filters for on sale now/expiring soon", and by the end of these 6 slides that problem is solved

but along the way, slides 4 and 5 sort of introduce these smaller separate problems (how do you filter a single element, and how do you chain two methods together) that help with the solution to the overall problem

sorry for the giant wall of text, but check it out tomorrow and let me know if have any quick questions about it!  If you want to talk about it in more detail I should have some time on Friday afternoon after lunch/town hall

----- Yesterday April 2nd, 2015 -----
