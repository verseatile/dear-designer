# Dear Designers

### Intro

Dear Designer, this document is for you. The hopes are that as engineers that work on the front-end (mobile & web) we can communicate our expectations through this writing, and in turn remove any surprises or most unexpected asks of you during a project.

### Handoff

When handing off designs in a tool like Figma, there's a few things you need to consider:
- link to the most recent designs
- pass off an export of what the final file is supposed to be (.fig)
    - this may seem duplicative, but it isnt. handoff means that there aren't any changes left that isn't from internal feedback.
- Designs should be accounting for the smallest size of a breakpoint
    - this ensures that a design can account for the smallest device that falls within a breakpoint category.  
- Place designs for multiple breakpoints beside each other.
    - this allows for easy searching for the entire design for a specific screen or flow. Engineers are slowed down massively by having to scramble across your Figma file to find the pieces of what makes a single view.


### Breakpoints

Say this with me:
> "I will not design toward a specific device, as I will design for a range of devices".

**Figma does not offer breakpoints.**
I'm serious. Do not use the default artboards/frames offered by Figma. Remember that this is a tool for a general set of users, and that is not the purpose of those templates. For our purposes, your artboards should reflect the sizes that are being designed for.

##### Who decides the breakpoints in use?

A variety of people. The general ranges being accounted for are often defined in contract agreements, but breakpoints should be assumed to account for all devices regardless. Breakpoints are not to be decided solely by design. This should be the result of a discussion between design and engineering. If you find yourself unclear as which breakpoints to use, here's a good starter:

##### Mobile

Mobile can be understood and your smallest size up until the start of tablet. Since the smallest device commonly supported has a width of 320px (iPhone 4, 4S, 5, 5s, SE Gen 1). A good standard for the largest mobile size is 579px. This covers all mobile devices with room for comfort including large ones such as any Pro Max model iPhones, Samsung phone, Pixel XLs, etc.

##### Tablet

When referring to the Tablet breakpoint, this often confuses many due to the shifts in physical tablets in recent years. There's now small tablets, medium size tablets, and some share the size of desktop screens (looking at you 12.9" iPad Pro). To safely cover this range, use the following:
- Tablet Small (580px - 767px) (optional)
- Tablet (768px-1023px)

##### Desktop

I need to be incredibly clear here - desktop does *not* begin at 1440px. A few import things to consider here:
- a majority of users do not have their browsers full screen during use.
- the average desktop display is not a Macbook Pro with high pixel density. 13" Macbook Pro's can't even reach 1440px unless the pixel density is increased.

### Internal Design Review

Before designs reach a client, there should be an internal design review with the greater team. Those in attendance are usually product, an engineering representative (frontend or architect if unable), and of course design. Project management should be present to take notes and if not, need not be there.

This meeting allows everyone including engineers to be aware of how the product is evolving over time. Engineering input is crucial here, as it provides an opportunity to discuss feasibility and promote product alignment. If requested changes are necessary, this meeting should occur enough time in advance to give designers a healthy amount of time to make adjustments before facing the client.


### General Project Communication
Although I completely understand the temptation, it is in everyone's (including yours) best interest that you do not work in a silo. You are a member of a team, and it is important that you communicate as much as possible about the state of your work. 

Design is often the start of the delivery cycle, so chances are that you're one of the first individuals to experience the client and their ways of working. It is necessary to the team to hear your input, experiences, and level of comfort regarding how things are going. It is best to take an iterative approach to solving initial problems, and pushing for client approval on features and visuals in sections.

### Know Your Platform
> Are you building a web application? A mobile application? Is it a web application embedded into a mobile application? Something completely different?

It is absolutely crucial that as a designer you understand the platform that you are designing for. For each platform, you are expected to understand the basic behavior of its native elements and some of the limitations presented there. 

There's often overlap between mobile and web, but the two platforms are different. Many mobile paradigms do not translate over to the web. Any common built in modules that are seen within a mobile device should be understood as not available in a web environment. When crafting designs for these platforms think about feasibility, the impact it has for the user, and the impact on the project. If you are unsure, discuss with your engineering team!

### Documentation

> "Working software over comprehensive documentation"
>  -Agile Manifesto

> "Documentation is only as useful as the value it provides to its intended audience".

Design documentation has always been a heavily debated topic, but let me be clear - overdocumenting always harms the intended output. Modern vector design tools (Sketch, Figma, etc.) have reduced the need for documenting many details about designs.

##### Spacing

Just select a layer and hold down `Option` to its spacing relative to another element. As long as the spacing is consistent across designs, there's no need to overdocument spacing across projects.

##### Type Styles

This one's easy. Use an artboard to lay out the various type styles used in the document, and use consistent naming so that it is easy to follow throughout. Ensure engineers have access to all fonts used throughout.

##### Colors

Again, easy. On an artboard, display a group of shapes (commonly rectangles) that contain a color, and beside it add relevant details about the color including name and hex value. 

**If using Figma, ensure that your colors are not gradients.**

##### Larger Components/Modules

The use of these within designs should be enough in most cases. If these contain interactivity, those should be represented somewhere. Engineers refer to the information that drive the interactivity as `state`. Make sure that your module properly accounts for the various states in the design, and where the state that drives the module should come from if needed.


### Useful Reading

**Lean UX: Applying Lean Principles to Improve User Experience**
*by Jeff Gothelf and Josh Seiden*
[Amazon](https://www.amazon.com/Lean-UX-Applying-Principles-Experience/dp/1449311652)
This book is fantastic, and represents clear established approaches to working in project structures that call for speed, flexibility, and unpredictable requirements. Although I must point out that some approaches do not match ML's team structure or approach to client's it is important and very necessary to understand. This book should serve as a reference when projects feel "out of whack" or one is curious about how to convey a topic to another team member in another discipline. Also, it is short!
