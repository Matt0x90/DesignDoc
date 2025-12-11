# DesignDoc

* Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?
  
The Gaming Room is a game development company with an existing Android app called "Draw It or Lose It", which is a multiplayer puzzle game where teams compete to guess images that are progressively revealed over 30 seconds. They want to expand to a cross-platform web app, that can be accessed on all desktop and mobile devices. Some of the key requirements included unique identifiers for games, teams, and players, a singleton pattern for game instance management, and support for multiple concurrent games.
  
* What did you do particularly well in developing this documentation?

Analyzing different operating platforms such as Mac, Linux, Windows, and Mobile for server-side and client-side uses, as well as development tools. I provided clear justification for the final Linux recommendation, tying the technical decisions back to business requirements and accessibility. 

* What about the process of working through a design document did you find helpful when developing the code?

The design document helped clarify the entire process by thinking through the constraints and architecture before approaching the code. I defined the domain model (Entity, Game, Team, and Player classes), as well as their relationships and data structures. And I identified requirements like unique name validation, singleton pattern, etc.
  
* If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

The recommendation for memory management section could be expanded further. It briefly goes over both server-side and client-side concerns, but could include more specific approaches.
  
* How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?

The user needs were interpreted by analyzing all of the possible requirements, then translating those into technical decisions. For example, unique names, multiple teams/players, cross platform, low latency, responsive image reveals, and handling disconnections. As well as WebSockets for real time sync, CDN for image delivery, and Redis for session persistence. Considering user needs is critical to ensure what is delivered is accurate and solves their problems without creating more issues.
  
* How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?

I gathered and attempted to clarify the requirements, though this did bring about some questions related to the design. I had to identify constraints such as latency, cross-platform, and scalability concerns. Then I had to evaluate platform options, create a domain model using UML, and map requirements to specific technical recommendations. Some future strategies would be to clearly identify scalability concerns and high risk areas of development. Incorporating user feedback and clarifying design needs are helpful too. 
