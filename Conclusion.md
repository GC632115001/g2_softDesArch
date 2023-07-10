## Conclusion

these are the main problems and solution that we found out and summarize

# Problem 1: Complexity

- solution 
1. Simplify event interactions, refactor components, leverage event-driven frameworks, prioritize simplicity over flexibility, and ensure clear documentation and communication.

2. Enhance logging, monitoring, and tracing capabilities for comprehensive visibility and issue resolution in event driven architectures. Establish clear contracts and schemas between microservices for reliable event handling and data consistency, while leveraging dedicated debugging tools like distributed tracing and event replay for efficient problem identification and resolution. 

3. Implement effective monitoring and observability practices in the large event-driven system by utilizing centralized logging, distributed tracing, and metrics collection. 

4. Event-Driven Choreography enables decentralized decision-making, promotes service autonomy, and simplifies the management of complex distributed processes by allowing services to interact asynchronously through events, eliminating the need for a centralized orchestrator. 

5. implement distributed and decentralized architectures.

6. receive only the necessary data. 

7. Use tools. 

8. Utilize established design patterns. 

9. use an event store to maintain the complete history of events. 

# Decision Driver

- Mitigate complexity, improve system understanding, and enhance the overall stability and reliability of the event-driven architecture. 

- Mitigate risks, improve system reliability, and enhance the overall performance and stability of the event-driven architecture. 

- Enhance system understanding, facilitate troubleshooting, and ensure efficient management of the event-driven architecture at scale. 

- scalability, agility, and fault tolerance in complex distributed systems. 

- risky, complex, costly, and time-consuming

- Demand for real-time.

- Faster implementation.

- Reduce complexity and interdependencies.

- Flexibility and agility.

- Availability and scalability.

- Less resource utilization.

# Reference

- https://medium.com/wix-engineering/event-driven-architecture-5-pitfalls-to-avoid-b3ebf885bdb1
- https://serverlessland.com/event-driven-architecture/visuals/common-issued-with-eda
- https://danoncoding.com/event-driven-architecture-part-1-pros-and-cons-with-examples-a2e5161fbcbd
- https://www.neebal.com/blog/advantages-and-disadvantages-of-event-driven-architecture
- https://serverlessland.com/event-driven-architecture/visuals/common-issued-with-eda
- https://danoncoding.com/event-driven-architecture-part-1-pros-and-cons-with-examples-a2e5161fbcbd
- https://www.neebal.com/blog/advantages-and-disadvantages-of-event-driven-architecture

# Problem 2: Queues 

1. Implement a combination of ordered queues, distributed processing optimizations, and service-level monitoring to mitigate the challenges of managing system state in event-driven architecture, accounting for potential delays and out-of-order messages.

2. Implement a delayed queue mechanism that maps dependent events, validates dependencies, and uses a back-off strategy like exponential back-off to manage wait times and retries, ensuring proper sequencing and satisfying event dependencies in a chain-like structure.

3. Design a fault-tolerant and resilient event driven architecture by implementing compensating actions, sagas, and idempotent operations. Utilize event sourcing, versioning, and comprehensive testing strategies to ensure data consistency, handle failures, and resolve issues effectively.

4. Implement an event-sourced system that incorporates an additional promise status. When an event is received with missing dependencies, save it with a promised/pending status and proceed with processing once the dependencies are fulfilled. This approach eliminates the need for extra queues and retries, but requires careful design and management of promise/pending states in the code.

# Decision Driver

- Mitigate risks, improve system reliability, and enhance the overall performance and stability of the event-driven architecture.

- Address the specific challenges related to ordered queues, delayed queues, and managing system state, with a focus on ensuring proper sequencing, handling dependencies, and simplifying the architecture where possible. (s04)

# Reference
- https://www.equalexperts.com/blog/tech-focus/event-driven-architecture-the-good-the-bad-and-the-ugly/
- https://medium.com/@prabhu.seshadri/handling-out-of-order-events-in-a-event-driven-systems-93349bd20c26

# Problem 3: Difficulty in discovery, tracking, and debugging

- Solution
1. Document events and use visual aids to aid discoverability.

2. Use observability tools to monitor and trace events throughout the system. Provide ongoing education and resources to the team.

3. Implement a comprehensive set of monitoring tools and practices to give visibility into the event flow, allowing for better error handling and troubleshooting.

4. Utilize reliable third-party tools for monitoring and debugging event flows. Implement robust error handling mechanisms and invest in comprehensive logging and monitoring systems.

# Decision Driver

- identifies key areas of misunderstanding or poor management in event-driven architectures.

- seeks to educate readers about the key concepts of event-driven architecture, how it differs from traditional systems, and what to consider when implementing it.

- help readers understand the potential advantages and drawbacks of adopting EDA in their microservices-based applications.

# Reference

- https://serverlessland.com/event-driven-architecture/visuals/common-issued-with-eda
- https://danoncoding.com/event-driven-architecture-part-1-pros-and-cons-with-examples-a2e5161fbcbd
- https://www.techtarget.com/searchapparchitecture/tip/Event-driven-architecture-pros-and-cons-Is-EDA-worth-it

# Problem 4 constant tension from many different angles, and it’s often hard to discern which dimensions of the design should get more weight and which should get less , Basically don't know what to pioritize.

- Solution

1. Use the use cases, desired outcomes, and constraints as guide lines.

2. start by asking the future users lots of questions to figure out what dimensions of the project or more important and which are less important.

3. it’s about people, do something that your team can support and work together.

# Decision Driver

- Many Choice to make not sure which is the correct/right one to do.

- Don't want to make mistake that will make the company loose money.

# Reference

- https://www.quora.com/What-are-some-real-life-challenges-of-software-architects

# Problem 5 software isn’t scalable

1. Patches may alleviate some of the early issues, but patches add complexity.

2. Invest time in requirements gathering.

3. Break down tasks and set realistic deadlines.

# Decision Driver

- Scalability.

- User experience.

- time allocation.

# Reference

- https://www.conceptatech.com/blog/importance-of-scalability-in-software-design
- https://www.mezmo.com/blog/scalability-worst-practices