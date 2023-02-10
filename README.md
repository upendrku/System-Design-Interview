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


</code>