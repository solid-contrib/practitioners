# Solid Practitioners

## Meeting Date

- 2025-10-16, 15:00 UTC

## Details

- call https://meet.jit.si/solid-practitioners
- chat https://matrix.to/#/#solid-practitioners:matrix.org
- repo https://github.com/solid-contrib/practitioners
- recordings https://spectra.video/c/solid_practitioners/videos

## Facilitator

- Jeff Zucker - dubzed@gmail.com

## Scribe

- Zachary Grider

## Participants (please add yourself)

- [elf Pavlik](https://elf-pavlik.hackers4peace.net)
- [Luke Dary](https://w3c.social/@lukedary)
- Stephen Taylor
- Tom Byrd
- Zachary Grider
- Theo @thhck
- [Michal](https://id.mrkvon.org)

## Agenda

### Administrative

- Call to add self to hackmd
- Call for Scribe
- Objections to recording the session?

### New Member Check-in (brief intro, current work)

### Announcements

- Upcoming meetings :
  - Nov. 6 - Food Distribution & Short Supply Chains
  - Nov. 20 - Practitioners' roadmap & feedback to ODI
  - Dec. 4 - Access Controls & Community Content Standards, see https://hackmd.io/@dtb23/SyWsIvljll

### Presentation: Decentralized Archive Project

- Jacob Daniel will present on a North Kensington Social Justice Archive (demo pilot)
- https://nksja-demo.northkensingtonlibrary.org/
- topics to include : ownership, access, preservation
- video of presentation at https://spectra.video/w/pPpFS5s3MVJioVKncFKWGE
-

### solid-contrib ownership

https://github.com/solid-contrib/.github/pull/2

### Discussion

shorthands: jz - Jeff zucker, jdr - Jacob D Rety (presenter), wrt - with respect to, ep - elf Pavlik, CSS - community solid server, mc - michal, jw - jesse wright, zg - zachary g, TBL - tim berners-lee

jz: will circle back to things from last meeting later
jdr: web dev, interested in solid, decided to pursue archival ability of solid with funding from his local conference. discussed the difficulty of communicating what exactly solid "is".
jdr: asked people and they decided a nice user interface for those archival data. number of technical concerns regarding archiving and decentralized technology which contradict ... (pulling up notes)
jdr: claims no expertise in solid but archiving is an interesting use case regarding domain specific approaches of social archiving wrt a decentralized technology like Solid.
jdr: benefits of solid with allowing people to maintain ownership over things while allowing stewardship wrt others and the role it can play. can solid play a positive role for users
jdr: and technical experts in the archiving area? could be as simple as control of access, and preservation is very important wrt archiving. how can solid interact with preservation tools?
jdr: council has a very basic digital archive: scanning documents and pdfs to preserve them, but wants to extend and has funds to allow the growth of this digital archive. the council has had
jdr: issues with finding the tools for digital archiving despite funds availability. (opens the floor to questions)
jz: (opens the floor for questions)
ep: (chat) asks for demo
jdr: starts presentation (PPT LINK GOES HERE) (starts email)
jdr: part of the "save our library" campaign in his local township. slide 1 - image of North Kensington library, has the Friends of North Kensington Library image
jdr: shows landing page and UI (https://github.com/Jacob-Daniel/solidpod), has a Solid project logo and the "God Save The Library" image
jdr: created a react app for brevity, and the backend is built with strappy(?), users are stored as forms of WebIDs to reference their work
jdr: released it to few friends in the area, unfortunately no one has used it yet, however he is hoping this will generate interest
ep: if the user logs in, is there any extra functionality to the website at this point in time?
jdr: running own CSS locally to not introduce any complexity to a user at this time
ep: if a user has an existing Solid/CSS account on a separate server, can they still useyour application or is configured to registration on your own server?
jdr: not something thought about yet, something to think about for future
jdr: page where you can login and upload a word doc, a pdf, or a similar text document.
jdr: (demonstrates account creation and signup capabiltiy using CSS to interact with web application, ep helps coaching, successfully logs in, shows basic landing page and dashboard)
jdr: (dashboard lets you select a category, add a title, other fields, to upload documents. also has functionality to edit your profile)
ep: is the profile page something that edits your WebID directly or does it set an application-specific profile?
jdr: i believe the application sets an application specific profile, pretty sure I am not editing the WebID document directly
jdr: unsure if the profile is set up correctly in the way Solid intends
jz: can you show us some of the categories?
jdr: yes, just wanted to get a working example - it isn't practically correct but just showing the boilerplate for how an archivist would possibly align things
jdr: (fills title, description field, choosing image and document file, sets permission to public and allows annotations by other users)
jdr: not able to see it live right now because it is a static site builder - it isn't configured to rebuild the page (hot reload is not active right now)
jz: have you - in terms of categories - looked at different ontologies which would be used to construct these categories? for example, if other archivists have used separate ontologies?
jdr: i have not, i belive that is something better suited to the archivists
jdr: my next step is to work on the saving of materials but wanted to look at collaboration on documents and annotations. for example a researcher might come and want to create a piece
jdr: which collaborates on work that exists in order to create new work. hopefully it is perceived as both novel and exciting
jz: asks for questions
ep: since i asked about the profile, there is a way your app is supposed to be working, there is currently no consensus on how WebIDs are supposed to be used. there are also security implications
ep: with WebIDs, especially since they are big security anchors.
mc: how do users find the documents? where do they go? what works when you upload them? interested in the sociality and networking aspect of the different archival topics
jdr: all resources currently exist on the one server. that doesn't have to be the case and you should be able to access and maintain pods yourself. the interface itself as shown
jdr: shows the available files on the server.
mc: when you upload the documents, does it go to a personal pod or to the server's pod?
jdr: it depends on how you authorize
jz: to clarify - there is no central pod where every resource which is uploaded gets stored?
jdr: all the pods that currently interact with the webapp are located on my server.
jdr: clarifies that the archives are stored in the users' own pods
ep: how does your application aggregate information which has been uploaded from the specific user?
jdr: the app has 3 parts - frontend, backend which is responsible for layout, and the Solid portion
jdr: i did the Solid portion within a content management system. instead of storing tables, I stored the WebIDs
ep: from the WebID how do you actually discover the resources which someone has uploaded to your webapp?
jdr: happy to look at my code, but i have not yet finalized how this aggregation would work. i was focused more on how this would work for archivists
ep: it's all okay, good stuff so far
mc: its good
ep: is your code open source?
jdr: yes
ep: great, we can look ourselves
jz: (links his linked-bookmarks repo) project i worked on which allows you to browse different subsets of archived material
jz: users can store material in their own pods and has a servies of categories, and your archival sets can be shared
jz: example: someone looks for sets of animals and can find two sets of uploaded resoruces regarding alligators and birds - both of those would be retrieved under the "Animals" category
jz: so jdr - questions for us? blocked on something? unsure of approach to something?
jdr: yes, did not expect this level of interest.
jdr: one issue we are having right now is "what is Solid's role". right now an organization might have an existing set of resources. in terms of ownership do they want to control access or completely own it? do they store
jdr: materials in a server they own? we are somewhat confused about how much ownership and granularity?
jz: any further questions for jdr?
jz: thank you for your presentation, very good. we hope to see future stuff

** moving to solid-contrib **
jz: discussing ownership of the solid-contrib organization which is on GitHub and consists of many different projects
mc: ODI wants to take ownership of solid-contrib and i think it would be valuable for the community if these projects were instead distributed amongst the members in the community
mc: and importantly, for practitioners it is the home of the #solid-practitioners group. i would like to see ... we would not need to reach out to ODI to move and add and edit repositories
jw: the context why the PR was made: the lack of governance was made in a call with jz and ep. i drafted a piece of text in the specific way with ODI maintaining the solid-contrib repository
jw: because the solid-contrib repository projects could be separate from the core solid libraries to prevent noise from being added to the main solid repository but i am unsure of the specifics of this
jw: when ODI took stewardship of solid, we would take on stewardship of the solid-contrib. we are not trying to take control of solid-contrib but clarifying the governance
jw: i am happy to take suggestions on what the governance of solid-contrib should be if GitHub allows it. the ODI can be advisors and a maintainer of solid-contrib is separate
ep: i wanted to clarify what is "we" - is it solid practitioners chairs?
mc: this was not discussed in detail but it is my personal preference
jz: can we have multiple admins from the working group, odi, practitioners, to ask any of them to create a repository requires one vote, but archiving or deleting would require 2+ votes?
jw: the document proposed makes it that in order for something to be archived or removed it would be up to the owners of the repository. ODI, practitioners, or community group would therefore not have
jw: some level of power over that until the maintainer wishes to hand it off
mc: code ownership is not a thing. organization owners have all the decision making power. at jeff: it could be an option to have a shared ownership as peer owners but not peer maintainers of a repository. it is
mc: important for the previous owners to have some level of decision making wrt their code. it is important to have continuity with maintaining solid-contrib libraries. with understanding that the library owners act with consensus
jz: im not sure if i want to be personally involved but i like the idea of having more than one administrative source. if archiving is up to each maintainer, the two things that an administrator does is monitor for
jz: code of conduct violations. the other is allowing people to create repositories on behalf of a submitted project.
ep: there are 80 repos but less than a dozen have active edits in the past year, and of those most of them are archiving or updating READMEs.
ep: should be searchable but it is mostly unusable which are abandoned, so what do we want to do?
mc: i want to mention that part of the autonomy for repos is the ability to move away. the document doesn't mention anything about right to leave?
jw: i can add that in
mc: how do you see possibility of ownership not in ODI?
jw: im not sure about roles but i am suggesting that ODI has an "admin" role over the repo
ep: it is owner
jw: owner and member, is there a way to give members the ability to create repos? i am asking because if the CG group changes then I do not want a CG chair to go rogue and delete everyone as an admin
jw: i want CG and PG to be able to create repos but I do not want the risk of an admin going rogue and deleting all other admins
mc: this is an issue of GitHub permissions structure. it would probably need to be resolved legally. not sure how GitHub would act. it is important for the highest level of ownership should be at the community level.
mc: kicking people out should be illegal. it is very much appreciated ODI wants to steward the project
ep: i think we should consider just moving the active repositories away from solid-contrib and leave the rest of them in the dust
jw: legal accountability doesn't practically pan out here because we all live in jurisdictions and it is full of individuals not companies so the only accountability is reputation
mc: there are people who have been handling solid-contrib for years while ODI has not been around that long, and ODI has not yet earned the trust of the community. for me personally i want the community to have more autonomy.
zg: GitLab is possibly an option
ep: michal you need to clarify on what community means because you are speaking for yourself but you claim to be speaking for the community
mc: someone needs to speak up here and i think i can represent the community which are people who have been involved in the solid community for a time but not with ODI
jz: CG and practitioners do not represent the whole community, but anyone can join and make a statement about things with respect to those communities, and the chairs of those groups should brings those concerns and statements to ODI
jz: we do not speak for the whole community but we are representatives of the community anyone can come to our meetings and give their opinion which we as a group can pass on to ODI
ep: people working on ODI are long time solid community members, so these people are not new people who have no experience with Solid. TBL passed stewardship of the entire Solid project to ODI
jz: lets talk less about community and more about open-source. difference between OS, imec, inrupt, ODI, and others. OS devs need representation as well because they are separate from the business entities
ep: can we make a list of realistic options on the GitHub and from the existing options we say "okay what can we do with these options" and see if we can resolve this dilemma? we need to close this conversation so we can move on
mc: i would be interested in hearing from ODI on how they can image a shared ownership structure or leadership structure which also takes the community into the account. i like stewardship but i do not want them to take care of
mc: everything. there has been this large $3M grant which has made no commitment to sharing these resources yet while many developers are doing this in their free time or begging for funding like that such as noel de martin but
mc: they have to take day jobs because their is not much money in the Solid community. i do not feel that ODI is acting honestly with the community and it is important for us to have a boundary with ODI. sorry i ranted a bit
ep: solid was not thriving when stewardship was passed to ODI. i have been participating here for at least 5 years and been following it for over 10 years, and I have different ideas about the movement of Solid. "Let ODI cook"
ep: i think ODI is very encouraging because they are trying to work with us while still implementing things.
mc: i want ODI to include people more rather than keeping the $3M grant for themselves. it would be better if they created positions for people who have already been involved with the community for quite some time and
mc: have shown a long term time investment in the community. it feels dishonest to pay people to do work when the work was already being done by community members for free. if we are not happy with ODI, it would be better
mc: to have some autonomy rather than hand over all the resources to ODI. i am finished ranting
ep: everything is open so if someone wants to fork it then they can. ODI will not have full control of the specs or resources in the community. community direction issues will arise without fail, and ODI went out to get a small
ep: team of people to bring them to the whiteboard to figure out where to start. it is not perfect but ODI can help drive Solid because it appeared to be stagnating. it could be good to have them to help drive Solid forward
ep: i understand the concerns about ODI but it feels idealistic rather than addressing how the community is at the current point in time
jdr: thanks for allowing me to present
jz/ep/mc: thank you for presenting
