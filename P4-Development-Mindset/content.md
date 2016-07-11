---
title: "Development Mindset"
slug: development-mindset
---

This lecture covers the mindset you should have to become the most effective software developer.

![ms-video-youtube](https://www.youtube.com/watch?v=0wteoPtwwh8)

<!--<embed src="https://github.com/MakeSchool-Tutorials/SA-2016-Apps-Lectures/raw/master/P4-Development-Mindset/DevelopmentMindsetLecture.pdf" width="640" height="360" type='application/pdf'>-->

[Click here to download the slides](https://github.com/MakeSchool-Tutorials/SA-2016-Apps-Lectures/raw/master/P4-Development-Mindset/DevelopmentMindsetLecture.pdf)

#Notes

##Learn by Doing
- You may be feeling a bit lost, like you don’t know anything about developing apps or games.
- You don’t really learn things until you use them, sometimes until you use them multiple times.
- Fortunately, you can still build software.
- Most startups and products are built by people who don’t know what they’re doing.
- The key is to learn to learn on the fly, and learn by doing.

##Take Baby Steps
- It’s hard to tackle a big project, make life easier by breaking it down.
- The design doc made it much easier to approach your apps and games by breaking it down into classes.
- Similarly, break down a class into the methods you want to implement, break down scenes into components (user input, player movement, enemy spawning, enemy movement, collision detection).
- Make one piece work, test it thoroughly, then move onto another piece, then work on connecting the dots.
- If you try to do everything at once you’ll make it impossible to debug issues and will feel overwhelmed.

##Ship Early, Ship Often
- Build the base features of your app or game first, don’t get distracted by the bells and whistles (this includes menus / story / art / theme).
- Get the core app or game built, and ship it / show it off to people as early as you can.
- Iterate quickly on user feedback.
- Once the core features are done, move on to polish, delight, monetization, etc.

##Write code for users
- Don’t write code that’s easier to write, write code that’s easier to use.
- Spend the extra effort to make things intuitive.
- Think about how to make things intuitive before you start coding. This means you should make a plan before you start coding!

##User on-boarding
- User on-boarding is one of toughest and most important things to do right.
- Think about how to teach your user to play the game or use your app.
- If you add a tutorial / guide at the end of development, it will suck.
- If you have a “how to play” button, nobody will tap it.
- Think about how you’ll introduce people to the app or game and help them understand how to use it before you start developing.
- That way you can code the app or game to have onboarding built in instead of adding it as an afterthought.
- The on-boarding flow should feel like you’re playing the game or using the app, not being given instructions.
- Don’t reveal all features and complexity upfront, teach the user as little as possible at every step.
- Teach one action, and let the user master that action. Then move onto the next action.
- Design for low attention, people playing your game or using your app might also be watching TV or chatting with friends, so they won’t pay attention to everything.
- Design for low attention span, they’ll get distracted quickly and lose interest.
- Never have more than one line of instructional text on the screen, people want to "do" not read!
- The first minute of the app or game is the biggest factor in retaining users.

##Edge Cases
- Think through edge cases before you start coding, will save you loads of time.
- Think of ways the user is not supposed to interact with the app, will it break anything?
- What happens when someone tries to swipe and tap with two fingers at the same time, or use two power-ups at once, or use a hint after they've already solved a level, or close the app in the middle of editing something, etc...?
- Don’t design for the optimal case, design for all cases.
- Think through the assumptions you’re making, don’t get locked into how you think the user will behave.
- Make a list of edge cases and test them frequently!

##Pseudocode
- Pseudocode is a way of describing your code in english, that way you can worry about the logic without worrying about the syntax.
- If you feel a bit uncomfortable writing a piece of code, try writing pseudocode first.
- If you’re writing an algorithm or complicated logic, definitely write pseudocode first.
- Make sure your pseudocode covers all edge cases.
- Once you are comfortable with the logic, then translate it with the right syntax line by line.

		count number of neighbors
		loop through cells
			if cell is alive
				if num neighbors is less than 2 or greater than 3
				cell dies
			else if cell is dead and num neighbors is 3
				cell becomes alive
				
				
##Test Thoroughly
- You should be your own QA team.
- Test individual components of the project as you’re building.
- Test how things interact with each other.
- Test in ways the user is not supposed to interact with the product.
- Test through your list of edge cases.

##Utilize Resources
- Google
- Stack Overflow
- Online Tutorials
- Open Source
- Peers

- Chances are, someone else has faced the same problem that you’re facing or built the feature you’re looking to build.
- The software development community is built around sharing knowledge, use this to your advantage.
- When you can, take the opportunity to give back!

##Effective Googling is a Superpower
- Search the exact error minus project specifics
- Search what other people would search
- Try different phrasings like “how to” or “example”
- Add specific terms like "UIImagePickerController"
- View second page results, search again with new info
- Once you reach page 2 of the results, try a new search query!

##Good Debugging is a Superpower
- Set breakpoints to see whether code is being run
- Clean the project
- Use print to print out variable contents
- Break down long lines of code into pieces
- Consider effects of other parts of the program
- Isolate the problem

##Games Problem: Sprite isn’t showing up

###Basic Debugging Steps
- Check if sprite is added to sks
- Check if named correctly in sks 
- Compare didMoveToView to how it's done in the tutorials

###Deeper Debugging Steps
- Use breakpoints to check the object
- Print out position of object using print
- Explore impact of other parts of the program
- Update method
- Touch methods
- Physics engine

##Apps Problem: Makestagram timeline not showing some followed users’ photos

###Basic Debugging Steps
- Check whether you’re correctly following the users
- Are you calling the code to save new follows?
- Are the relationships showing up in the Parse Dashboard?
- Check whether you’re correctly querying for followed users
- Check whether the newly followed users have any posts
- **Use breakpoints for all of the above!**

###Deeper Debugging Steps
- Use breakpoints to check the responses from Parse
- Print out list of users you’re following
- Step through all the code that saves follows and queries for them
- Is every variable’s value always what you expect it to be?
- Is Parse ever responding with errors?
- Are you correctly determining whether a user has already been followed?

##Rubber Duck Debugging
- Often you can solve your problem just by talking it through.
- Talking through or writing down your problem will help you understand it better and catch your gaps in logic.
- Helps you think clearly when you’re frustrated and stuck.
- This tip comes from “The Pragmatic Programmer” — he would speak to the duck.
- For me, talking to my cats works really well. They always give me a look of "oh come on, you can figure this out. What are you missing?"

##Getting Help
*Before* getting help, you should ask yourself:
- What is the issue?
- What steps have you taken to debug?
- What line of code is the issue on?

##Becoming a Self Sufficient Developer
- Best developers in the world are self sufficient, they are comfortable teaching themselves anything they don’t currently know how to do.
- Language + syntax is not important, clarity in thinking + googling + debugging is important.
- Your goal is to become more self sufficient every week.
- This doesn’t mean don’t ask for help, but continue raise the threshold of when you ask for help. And maybe ask for different kinds of help.

##Hacker Mentality
- Be comfortable paddling in the dark
- Be relentlessly resourceful
- Love the cycle of failing then conquering
- Get it working, then make it good
- Never give up

“All the best things that I did at Apple came from not having money and not having done it before, ever. Every single thing that we came out with that was really great, I'd never once done that thing in my life.”
*Steve Wozniak*