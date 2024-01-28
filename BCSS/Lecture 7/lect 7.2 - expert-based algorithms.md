**Summary: Expert-Based Algorithms for Virtual Coaches**

**Definitions:**

- **Virtual Coaches/Conversational Agents:** These are digital systems designed to communicate with users, often providing guidance or suggestions based on certain algorithms.
- **Algorithm:** A set of rules or instructions that a computer system follows to complete a task or solve a problem.
- **Expert-Based Algorithm:** An approach where the decisions made by an algorithm are derived from the expertise and feedback of specialists in a particular field.

**Key Points:**

1. The focus is on a category of algorithms that uses expert feedback to guide the responses of virtual coaches.
2. *Illustrative Example:* 
    - Consider a scenario with a user named Laura, with known factors like the time of day (morning) and gender (female).
    - Experts are consulted to provide feedback on the appropriateness of various messages the virtual coach could send, based on combinations of time and gender.
    - Different messages are rated by experts for their suitability to be sent at specific times and to specific genders.
3. *Algorithm Implementation:*
    - Experts' ratings are converted into decision rules.
    - The virtual coach uses these rules to decide which messages are suitable to send to the user.
4. *Requirements for Expert-Based Algorithms:*
    - Experts: Professionals whose knowledge influences the algorithm's decision-making rules.
    - User-State or Traits Data: Information about users (e.g., gender, time of day) to tailor messages appropriately.
    - Selection of Characteristics: Identified based on behavior change theories, previous studies, or expert opinions.
5. *Outcomes and Characteristics of Expert-Based Algorithms:*
    - Effectiveness: Remains constant over time; does not adapt or learn from usage.
    - Explainability: If feedback is structured, the algorithm's decisions are clear and based on predetermined criteria informed by experts.
    - Predictability: With known criteria (e.g., gender, time), which messages to send can be reliably forecasted.

The summary encapsulates the concept and functionality of expert-based algorithms within virtual coaching systems, emphasizing the significance of incorporating expert knowledge to ensure relevance and appropriateness of automated interactions.

## Transcript

Welcome to the next video. In this video, we are looking at virtual coaches or conversational agents that derive their decisions in some way from experts. So looking again at the big overview, we are now located in the second column, and we are looking at part of the algorithm by Horst Freil, which I have no idea if I pronounced correctly, as illustration. Let's say we are again given our example person, Laura. And this time, we also know two other things. We know that it is in the morning, and we know Laura's gender, which is female. And before we are now deploying our algorithm, we've actually done something else, which is that we have talked to experts about this algorithm. So we have presented experts with different scenarios, scenarios based on the time and the gender of the person that is to be persuaded. And we've asked these experts how appropriate the different messages are for the different combinations of time and gender. For example, the experts may have said that this purple message cannot be sent in the morning, maybe because it asks people to reflect on their day. The experts have said that it is okay to send the message in the evening, and that it is okay to be sent to both genders. And similarly, the experts have told us how appropriate the other two messages are in the different situations. And now based on this feedback from experts, and the information we have about Laura and her situation, we can arrive at the conclusion that we cannot send the purple message, that the other two messages, the green and the yellow one, can be sent. So what is the idea? Well, the idea is that you talk to experts and derive decision rules from them, that then your conversation agent or virtual coach uses to make its decisions. And as with the previous algorithm core, it's useful to look at what we need for an algorithm like this. So of course, we need experts. And then whether you need data on the user state or user traits really depends on what kind of characteristics you are wanting to tailor to. We, for example, consider the gender, which would be more important than to figure out from people. But there might be other characteristics. And how you choose these characteristics might be that you base them on behavior change theories, on the results of other studies you've read about in papers, or that you've talked previously already to experts to see what they would consider important to account for. And besides what we need, we also want to look at what we get. And just as with the theory-based algorithm, this type of algorithm doesn't change its effectiveness over time. It's as effective at the end as it was at the start. For the explainability, well, that, of course, depends how exactly you elicit the feedback from experts. But if you do it in a structured manner, and with these kinds of scenarios that I explained that, for example, differ with regards to two variables, you can also very clearly explain how the decisions were made by the algorithm based on these kinds of criteria and the experts' feedback for these criteria. And lastly, it's also predictable in a similar fashion. So if we have these criteria, like for us, for example, the time and the gender, then once we know the time and the gender, we can say which kind of messages can be sent. So this concludes our video on expert-based algorithms. See you in the next video.