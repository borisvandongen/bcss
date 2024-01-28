### Summary: Adaptive Algorithms

**Topic Covered:**
Adaptive algorithms – algorithms that adapt based on online data.

**Example Used:**
A study with Baxter, a robot coach, using an adaptive algorithm to motivate individuals (Laura) during exercise by using one of four actions:
1. Showing motivational gestures
2. Giving rewards
3. Saying something encouraging
4. Doing nothing

Initially, each action is equally valued at 0.25. If an action seems ineffective, values are adjusted: the ineffective action's value is decreased while others are increased.

**Results of the Baxter Study:**
- Three scenarios were tested: no encouragement, random action, and learned action (adaptive algorithm).
- The number of mistakes did not vary significantly between groups.
- Fewer people made more than three mistakes in the learned condition.
- However, the data included only individuals for whom Baxter successfully learned the best strategy (23 out of 50 in the learned group).

**Critical Note on the Study:**
There's a concern about fairness and representation as 20 individuals were excluded because Baxter could not learn an effective strategy for them, and 17 were excluded because they made no mistakes.

**Algorithm Requirements:**
- Online data is crucial.
- Incorporation of states or user traits may vary by situation.
- Offline data, behavior change theories, or expert input can enhance initial effectiveness.
- Effectiveness from start is unlikely with only online data.

**Considerations:**
- Risk assessment (e.g., potential harm from incorrect persuasion).
- Explainability and predictability are challenging since the algorithm is dynamic.

**Conclusion:**
While good in concept, adaptive algorithms might not show significant benefits over random or no actions. The effectiveness and explainability of such algorithms depend on additional data and techniques.

*Next Steps:*
The discussion continues in the next video, delving further into adaptive algorithms and their applications.

## Transcript

Hello again. In this video, we will talk about adaptive algorithms, so algorithms that make use of some sort of online data. So our virtual coach now makes its decisions at least partially based on online data that is gathered. In our overview, we are now located in the fourth column, and we are looking at an algorithm by Roy to illustrate this notion of using online data. So, no surprise, we have here Laura again. And Laura is here together with Baxter. And they are in this kind of setting where Laura is asked to do some sort of exercises, and Baxter is trying to motivate Laura or help Laura to do these exercises by encouraging her in some way. And Baxter has four different actions he can take. One is to show, express some sort of motivational gesture. Second one is to give Laura a reward. Third, Baxter can say something encouraging or motivating. And lastly, Baxter can also do nothing at all. And at the start, we now don't really know which action is more effective, so we assign a value of 0.25 to each one of them. Then now, let's say that Baxter shows, expresses a motivational gesture to Laura. And then we observe that Laura does not succeed at her task. So now we think that probably showing motivational gestures is not that effective. And how we deal with that is that we increase the value for the three other actions. So we add 0.01 times 0.25, where 0.01 depends on the learning rate, to each of these three. And then if we now compute the sum, we see that the overall value is lower for this gesture action than for the other three actions, which means that we have a lower chance of applying or using this action in the setting with Laura. The authors have applied this kind of algorithm to the teaching of pattern tasks. And if you here now look at the number of mistakes that people made in three conditions, so there was one condition where Baxter didn't show any kind of encouragement in any form. Then in the random condition, Baxter showed a random action. And in the learned condition, Baxter would try to learn which type of action to show to which person. And you see that the number of mistakes seems kind of similar in the three conditions. The variability is maybe a bit lower for the learned condition. But it doesn't seem that this learning algorithm causes people to do fewer mistakes. And then the authors also separately looked at the number of people with more than three mistakes. And they compared it along the three conditions. And here you see that, well, in the learned conditions, there are fewer people who make more than three mistakes. And they actually found a significant difference comparing the people in the condition with no sort of motivation by Baxter and the learned motivation. So the learned motivation was significantly better. But what is often important is to look at which data was actually used in this kind of comparison figures that people have in their papers. So here, for example, when you read carefully, you see that the learned condition only included people for whom the agent was able to learn the best strategy. So for 20 people, the agent wasn't able to learn the strategy. And the authors mean that the agent couldn't really identify the one best strategy that would work for these people. So these 20 people were excluded from the analysis. The authors also excluded 17 more people for whom the agent never had to do anything because they never did a mistake. Because the point of Baxter was that it would only motivate people in the case a mistake was made. So overall, only 23 out of 50 people in the learned condition were used in the analysis. So yeah, you might think about whether this is really a fair comparison, or whether the authors are maybe just trying a bit too hard to see whether they can find a way in which their algorithm worked. And overall, again, you see, well, it was a good idea for an algorithm. But yeah, well, maybe we don't see that much of an effect compared to doing nothing or just choosing something random. What do we need for an algorithm like this? Well, we again, need definitely, well, we need online data. Not again, but for the first time now we need online data. And whether we need information on states, or user traits, depends, again, on the situation. Here now, with the example of Baxter, we didn't really consider anything else. So we didn't consider, so we didn't consider, for example, the mood, or how old people were, or how good they were at tasks in general, or something. So nothing like that was considered. But you could, of course, do that. And well, if you really only use online data, then your algorithm might not be very effective from the start, as we'll talk about later when we talk about what we get. So usually, you want something else that makes you, or that helps you make a decision at the start when you don't have any data yet. So this can be offline data, but it can also be behavior change theories or experts. Whether you need to do that depends a bit, as we'll also see later on when we talk about how suitable algorithms are for a certain situation, depends on how risky it is to fail. So is a person going to die if you have the wrong persuasion type, or is it just that you maybe make a little bit less profit in your online store, or something like that? So what we get, as I said, effectiveness from the start might not be there if we don't use anything besides the online data. So it might be a good idea to use something else, depending on the consequences of failing to persuade people. And the explainability and predictability can be quite tricky now, because, well, your algorithm keeps changing over time. And explaining that to a non-expert, say a doctor, a psychologist, might be quite difficult. But of course, there are also explainability techniques to try to make such algorithms more explainable. This concludes our video on adaptive algorithms or algorithms that make use of online data. See you in the next video.