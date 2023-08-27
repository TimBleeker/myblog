---
share: true
layout: garden_entry
type: _garden
excerpt: "Picking the right deliverables"
---
I know that, as a UX designer, I'm supposed to say that what I love best is to improve the lives of my users through thoughtful research and design. The truth, though, is perhaps a little geekier than that. My favorite thing about design is nailing a design hand-off. 

When I was first learning the ropes of designing in a professional context, I placed great emphasis on the production of pixel-perfect designs of every single part of a feature. Through trial and error I learned that, when working on an existing and agile product team, this is hardly the most effective solution. I still see many designers run into challenges around collaboration with developers and other stakeholders. The overview below has helped me and many of my design teammates collaborate better with engineers.

I keep this list to remind myself of the things that could be necessary to deliver a solid design hand-off to one or more developers. This list focuses solely on the technical design aspects, and ignores anything related to research, prioritization or other product-related questions.

### User story / epic
- When writing user stories or epics, I make sure to include:
	- Job story (epic) or user story
	- Link to design file
	- Any design-related acceptance criteria that are not covered by the solution design
	- Any details in the solution design that may otherwise be overlooked
	- Metrics
		- New events that should be tracked, including the associated properties
		- Existing events that need to be modified, including properties or other changes
	- Gherkins

### Design file
I like to work with design files that function not only as solution designs but also as good forms of documentation. For the past few years, I've been using [this Figma template](https://www.figma.com/file/G7Gy93hGI0lGugkAyPf0xZ/Zinzy's-feature-template?node-id=301%3A1361&t=S62mjl25fcXE1Tms-1) to kickstart any feature design:


![Zinzy's feature design template on Figma](https://res.cloudinary.com/dbi2zounq/image/upload/v1681718222/zinzy.website/feature-template_dt3rzs.png)


The file consists of several pages detailing the various aspect of a design cycle:
- **What & why** provides general information on the job story, as well as links to the epic or user story, the research repository, and the designers who worked on the project
- **Existing solution** may contain any screenshots of the current implementation as well as the current workarounds or folk interfaces users might have in place
- **Best practices** is the place where I store inspiration, both from competitors and general UX heuristics and best practices. It's the place where I begin to loosely formulate what should improve about the way things currently are
- **Drafts** is where design iterations take place. I organize my possible solutions here, and request feedback from various kinds of stakeholders. I use post-its to group questions by the type of stakeholder, and I've found that this helps stakeholders give informed feedback.
- **User testing** contains any qualitative user test efforts that might be involved in the project.
- **Solution** is where the final design lives as soon as it has received full sign-off. This page is also the link I provide to the developers.

### Choosing design fidelity
Because I work on long-term projects revolving around existing products, I very rarely need to deliver a pixel-perfect full user flow as part of a feature design project. Rather, I design only what is needed to help a user test answer our questions, or to help developers get the job done. I've noticed that explaining accurately how I make these decisions can be a bit tricky, and that's probably because I don't have a mnemonic device in place. Roughly, here's how I approach picking design fidelity:

- If I designed new styles / components that change across the flow, and if copy affects the UI in non-standard ways across the flow, I created a clickable, high-fidelity prototype of every part of the flow
- If the above is true, but styles / components don't change across the flow and copy doesn't affect the UI in non-standard ways, I create a high-fidelity prototype of the new elements, and create a wireflow for any flow-related parts of the solution
- If there are no new styles or components, but there are various elements of the flow that behave in a way not alrady covered by a design system, I created a wireflow
- If there's no particular flow to the solution, but it's instead about adding an existing element somewhere in the product, I'll create a wireframe, and describe behavior in the user story with gherkins

### Don't miss states
One point of concern engineers may have about a design hand-off is a lack of states. I often see the more visually-oriented designers struggle with this. Just to be sure, if you're working on a flow, don't forget to cover:

- Default (enabled but inactive) state 
- Empty state
- Active state
- Unavailable state
- Filled state
- Success state
- Error state
- Loading state
- Partial state