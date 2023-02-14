<code>

## OBJECTIVE
1. How to identify the right tech stack?
2. When to use a state management system?
3. How to represent an in-depth block diagram ?
4. How to represent complete HLD / LLD ?
5. How to create a sequence diagram?
6. Consideration aspects for the use case.
7. Leveraging generic templating mechanism.
8. Component-based architecture design.
9. Connection to downstream services.
10. Instrumentation, tracking & logging

## DIAGRAMS
    > HLD (High Level Design)
    > LLD (Low Level Design)
    > Sequence

## Sample Question -
Design the frontend of a cryptocurrency exchange orderbook with buy and sell bitcoin
as the options to the trader.

## Interviewer's Expectations
1. Create a block diagram for the question given.
2. Ability to choose one tech stack over another.
3. Create API schema for backend communication.
4. Ability to identify the edge scenarios.
5. Ability to identify components in the UI.
6. Write pseudo code for potential imolementation.
7. Explain the approach along the way.
8. Confidence in the approach chosen.
9. Take account of testing, code quality & maintainability.
10. How are you deploying the frontend components

## HLD (High Level Design)
1. Signifies the overall system.
2. States concise functionality of each component.
3. Also called macro-level design.
4. Developed by Solution Architect.
5. HLD is created before the LLD.
6. Converts requirements into solution.
7. Necessary to understand the system.

## Considerations while creating UI components
1. Accessibility
2. Design consistency
3. Theming ability
4. Reusability
5. Customisability
6. Extendability

## Server side rendering
1. Faster page load
2. Better SEO
3. Increases complexity

## client side rendering
1. Modular architecture
2. Less complex
3. Low Response payload

## LLD (Low Level Design)
1. Describes the components of HD
2. States the logic of the components used.
3. Also called micro-level design
4. Developed by software developers.
5. Developed after HLD is completed.
6. Changes HLD into comprehensive solution.
7. Describes configurations & trouble shooters.

## LLD Sequence
1. Tech stack - What? Why?
2. Components - Name and identify the components
3. Data structure - Define API Schema
4. Pseudo code

## Before choosing frontend frameworks
1. Popularity - Community support
2. Core features
3. Flexibility
4. Ease of integration
5. SSR support (Server Side Rendering)
6. Mobile support
7. Community
8. Future support
9. Market Adoption

## Frontend libraries / frameworks in the market
React, Angular, and Vue.js are three of the most popular JavaScript libraries for building web applications. While all three libraries can be used to build modern, interactive applications, they have some significant differences that make them better suited for different use cases.

One key difference between these libraries is the way they handle data binding. React uses a unidirectional data flow, meaning that data flows from a parent component to its children, but not the other way around. This can make it easier to manage state in large applications, as it helps to prevent unexpected changes to the data. Angular, on the other hand, uses a two-way data binding system, where changes to the data in a component are reflected in the template and vice versa. This can be more convenient for smaller applications, but can also make it harder to track down bugs in larger applications. Vue.js uses a reactive data model, which allows components to automatically update whenever the data they depend on changes.

Another difference between these libraries is their approach to templating. React uses a declarative syntax called JSX, which allows developers to write HTML-like syntax directly in their JavaScript code. Angular uses a template-based syntax, where developers write templates in HTML and bind data to them using special Angular directives. Vue.js also uses a template-based syntax, but it is more flexible and allows developers to use a mix of template syntax and inline JavaScript if needed.

In terms of size and performance, React tends to be the smallest and fastest of the three libraries. Angular is larger and can have a slightly slower runtime, but it also includes a lot of additional features and functionality that may be useful for larger applications. Vue.js falls somewhere in between, with a smaller size and faster runtime than Angular, but more features and functionality than React.

## Choosing Frotend Technology
Choosing between React, Angular, and Vue depends on your specific needs and goals as a developer. Here are some points to consider when deciding which of these technologies to use:
    > If you are building a small or medium-sized application and want a lightweight and easy-to-learn solution, Vue.js may be the best choice.
    > If you are building a large-scale, enterprise-level application and need a robust and scalable architecture, Angular may be the best choice.
    > If you are building a web or mobile application and want a powerful and flexible tool for building reusable components, React may be the best choice.

Ultimately, the best choice will depend on your specific project requirements and your personal preferences as a developer. It may be helpful to try out each of these technologies and see which one works best for you.

The future of web development is likely to involve a number of trends and technologies that are already beginning to emerge. Some of the key trends that are likely to shape the future of web development include:
    > Increased use of artificial intelligence and machine learning: Web developers are likely to use more artificial intelligence and machine learning technologies to build intelligent and interactive websites and applications.
    > Continued growth of mobile development: As more and more people use their smartphones and tablets to access the internet, web developers will need to focus more on building responsive and mobile-friendly websites and applications.
    > Increased use of cloud computing: Web developers are likely to rely more on cloud-based services and infrastructure to build and deploy websites and applications, as this allows for more flexibility and scalability.
    > Increased use of virtual and augmented reality: As virtual and augmented reality technologies become more mainstream, web developers will need to learn how to build applications and experiences for these platforms.
    > Continued evolution of web design and user experience: Web developers will need to focus on designing and building websites and applications that are user-friendly, intuitive, and visually appealing in order to meet the expectations of users.

Overall, the future of web development is likely to involve the continued evolution and integration of new technologies and approaches that allow developers to build better and more engaging websites and applications.

## Logging Tech stack

## Testing stack

## Sequence Diagram

## SPA vs MPA

## Progressive Web Apps
Provides offline support and native like functionalities
Improved performance
PWA is best of both worlds (Capabilities and Reach)
Native Apps have better capacilities but less reach whereas Web apps have better reach and low capabilities

## Security Aspects of SPAs

## Platform selection
Choose the right target for the right impact & returns
• Are my users on mobile?
• Is my app an editor?
• Is my app targeted for business?
• Do I have resources with the skills needed?
• Do I need to provide a real-time service? e.g. editor
• How is the pricing model?
• Will my app be frontend heavy?
• Is SPA enough?
• Is a PWA needed?

## Search Engine Optimization (SEO)
HTML Tags like meta tags, title tags, semantic HTML
building links
open graph tags

## Open Graph Protocol (ogp.me)

## Workflow considerations
    > Imagine what the one user will do over the other because everyone tries to do some sort of workflow in the system.
    > After you analyze the workflows and after the happy, happy parts from the product managers, you
    have to sit down and draw some of the diagrams which lead to non happy parts, which may lead to corruptions.
    > Try to think of all the edge cases that can occur.
    > Try to think of the sum of the workflows which are not supported by our system or some of the workflows
    which depend on the upstream or downstream systems
    > Find out the dependencies with the other teams and then trying to figure out if something fails in that particular aspect, in their particular system, what will happen to my system? Is there a proper schema set up between these two systems?
        + What happens if the schema is invalidated?
        + What should I do with the schema is invalidated?
        + Where am I logging all these all these things?
    So all this going to different user workflows, different edge cases.
    > Document everything

## MVP
Need to ask which phase of development the application is in?
It could involve change in architecture, the direction in which we want to proceed or even sometimes the vision.
NOTE: It is ok to tweak the vision but not completely changed.
Advanced Features may involve change in architecture. Analyze optimal approaches and how to handle these advanced workflows?

## Identify Service Requirements
Try to figure out different apis that are needed in the system.

## Volume of operation
First think about development volume -
    - How many developers are there?
    - Their skill sets
    - component based or micro architecture?
    - How things can run parallely
    - How can i make it possible to scale the development in internal development teams?
Think about team's volume and the end users of your product.
After understanding the vision you would want to talk to the managers and team leaders to know about scale of operation outside of the team.
And finally, the scale of operation of the end users.

Ex. If we know about the volume of traffic i am about to get, we can run a stress testing, load testing 
So even do in order to analyze, you must have some sort of instrumentation built in the MVP itself.
For example, how many people are loading this page on some sort of analytics need to be there in the MVP itself to make this decision possible.
 - Helps you to analyze how the users are performing, what kind of workflows that they are doing, what
 - Kind of things that they are looking at, and the kind of law that you get in your product.
 - It has to be analyzed for further scaling up.

Create documentation and it should be reviewed.
You cannot neglect all these things because a lot of feedback will be given based on based on your designs, on your architecture that you have laid down, running through different stakeholders in the system, get their approval and not just a verbal approval.

And it is a characteristics of a good architect to take this valuable feedback and convert it into refined requirements or refined or technical designs.

Collaborating with other stakeholders as well as the product managers is there is a very important factor.

## Performance optimization
Page load + Smoothness of operation

Smoothness of operation
Smoothness = UX E.g. Adding animations to avoid jerk/ stutter 
How analogus your system is?
Make it appear to be smooth.
E.g. motion blur like in IOS, navbar hiding with a clear indication where it is hiding

Fast load
Data prefetch
caching

Prioritise the performance improvement tickets in your sprint board if a call has not been taken already.

## Techniques to achieve performance optimization
- Caching
- Pagination / Infinite scroll
- SSR Initial data feed
    => NOTE: In case of SSR the number of API calls increases
- First contentful paint
    => Initial data/ content/ placeholders that user sees before the actual content is loaded
    => The user gets an idea that the page of the page is actually started loading and nothing is stuck
    => Gives the impression that things are happening so that user will stay on the page.
    => Grabs user attention
- First menaningful paint
    => It is when the actual assets load.
    => So first meaningful paint is the paint, after which the biggest above the fold layout change has happened and web fonts have loaded.
    => The page is finally becomes useful.
- First CPU idle time
    => The lowest time needed to provide a minimum user interactive ability is the actual first CPU idle time.
    => It measures how long it takes a page to become minimally interactive.
    => A page is considered minimally interactive when most but not necessarily all UI elements on the screen are interactive and page responds on average to most user inputs at a reasonable amount of time.
- Meaningful animations

## Optimizing Images
- Name your images descriptively in a plane language so that SEO can grab the information about the image and show it at different places.
- Optimize your alt attributes
- Choose your image dimensions and product angles wisely. If the images are getting resized this may take time.
- Use compression techniques
- Reduce the size of your images to so compression and choose the right file type for those images.
- Use image site maps, beware of decorative images, use caution while using content delivery networks like CDNs.
- Make sure that these are appropriately loading.

## Handling APIs
- Polling
    => Data that does not need to 100% real time and can be fetched periodically
- Web sockets
    => Real time data fetching
- Batching of requests
    => In cases we want to bundle our requests 
- GraphQL
    => If BE alread supporting it 
    => Helps concatinating and segregation of requests on the fly
    => Reduces number of requests
    => Helps you determine what you want
    => BEWARE: it may be overkill
- Caching GET APIs

## Buffer Overflows
Buffer overflows (overruns) occur when an application does not properly manage access and inappropriately writes to memory.
- A buffer overflow condition exists when a program attempts to put more data in a buffer than it can hold or when a program attempts to put data in a memory area past a buffer. In this case, a buffer is a sequential section of memory allocated to contain anything from a character string to an array of integers. Writing outside the bounds of a block of allocated memory can corrupt data, crash the program, or cause the execution of malicious code.

Impact:
A buffer overflow flaw arises when a program does not check the length of data assigned to a variable before storing it on this buffer.

- If we defined an array of char[500], the compiler will allocate 500 bytes on the stack.
- If the user input exceeds the length of the buffer, say 550 bytes, it may have some unintended impacts on the program. For example:
- Corruption of other program data (data integrity compromised)
- Corruption of program control structures (program may end up following unintended paths)
- Termination of the program (application / system crash)
In the worst case, an attacker can also craft an input that can execute any arbitrary command on the host outside of the application. This can lead an attacker to take over the computer or worse - the entire network.

## Injection attacks
- Injection attacks allow an attacker to alter queries (against databases, documents such as XML, etc.) or commands to execute unintended functionality or access protected data
- There are 2 Types - SQL Injection and OS Command Injection.

## Insecure Cryptographic Storage
Insecure Cryptographic Storage refers to misconfigurations and errors related to secure / encrypted storage of data

## Encoding
An alternative representation of data that does not transform the data and provides no confidentiality or access restriction.

## Encryption
A reversible way of making data secret so it can only be converted back to an understandable form with a known secret value.

## Role Based Management
Recognize the different types of users who would be using the system, like, for example, system administrators.
There could be normal administrators, there could be developers, test engineers, other product managers or other team members or different org members.

So, go through all of the roles that are displayed that are decided for this particular product and then finally figure out the different permissions for these roles.

Specifically determine the high level permissions and also the technical low level permissions as well. E.g. who has permission to build, who has permission to approve requests, who has permission to deploy, along with who has permission to use which feature in your project etc.

## Governance
Controlling the workflow and protecting the assets
E.g. JIRA processes for code level governance
Talk with project manager regarding this.

## Instrumentation
Measurement and tracking are key for a stable system

E.g. logging system
Properly identify different phases or blocks of modules where the load will hit in run time and implement logging
so that it can be debugged easily.

Use tracing techniques
Using tracing technique, we can gather information about code execution at runtime, tracing information can be used for troubleshooting an application after it is deployed. It gives an idea of how the data is flowing, from where the data is flowing and in what stages the data is being affected or in what phases.

When it comes to performance, you might want to add some more tests in the project. 
Add performance counters wherever it is needed to identify how much time it is taking for one particular workflow to happen or one particular api to respond.
It is to measure the performance at individual places or points in the actual complete execution.

Event logs
Handling of events gracefully to make sure that the system is very stable and it is also executing properly and performing as expected.

## Versioning
Preventing historical versions avoids disasters and helps to rollback.
Apart from dependencies we need to take care of our own product version.
Design system such that user is able to roll back or revert to a specific version of a document, 
It should log user whoever has altered it.
It's also storing whoever is modifying this document, what is being added?
What is a diff being created with this document?
All those metadata is being stored in our database in the logs when this metadata is mapped to certain blob.
So the actual data will most likely be in the blob and the metadata will most likely be in the in a different database.
And by storing historical versions, it creates a backup of the artifact.

This also applies for even code.
Helps in disaster recovery.

## Localization/ Internationalization
Localization - it talks about adoption of application to meet cultural and other requirements of a specific target market.
It can entail customization related to numeric data formats, use of currencies, keyboard usages, collision sorting symbols, icons, colors, varying legal requirements and in many cases and text and graphics containing.
Some countries don't want to display certain graphics based on the countries and their culture.
We need to define the standards of localization as the developers start working on it.
Localization may even on the data, comprehensive rethinking of logic, visual design or presentation
It might affect the way of doing business or the accepted program for learning in a given locale different substantially.
referred as i10n

Internationalization - internationalisation is the design and development of a product application or document content that enables easy localization. referred as i18n

Consideration:
This includes such as, enabling the use of Unicode or ensuring the proper handling of legacy characters, encodings where appropriate, taking care of the concentration of string's, avoiding dependency, code and user interface, string values etc. Typically, this involves incorporating predefined localization data and features deriving from existing
libraries of user preferences.

## Accessibility
The practice of making your website usuable by as many as possible.

## Quality Assurance & Control
Quality Assurance (QA) is a combination of activities throughout the manufacturing process that ensures the quality of the product. 
Consequently, Quality Control (QC) is a set of processes used to secure that the product meets the quality requirements.

Various levels of testing
    - Git hooks
    - Linters/ static analyzers
    - Unit Testing -> left shift approach (Testing being pushed to developers before right(testers))
    - Workflow testing
    - Same org Integration testing
    - Cross org Integration testing
    - Automation suite - e.g. cypress

## Future Roadmap
A strategic plan that defines a goal or desired outcome
Product Vision and quaterly plans
    - Serves as a communication tool
    - A high-level document
    - Articulates the strategy
    - Vision needs to be well defined
    - Milestones needs to be called out
    - Every quarter should have a goal
    - Need not consider team capacity
    - It is not a list of features
    - It is not a product backlog

</code>