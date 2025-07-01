# Empathy Benchmark
 
 # Defining AI (Artificial Intelligence):

 Artificial intelligence can refer to many different things (ex. non-player-characters in a videogame with simple decision trees, human-like artificial intelligence, and machine learning models). For the purposes of this paper, artificial intelligence is defined as being a machine learning model with generative capabilities of any caliber that is capable of taking in user input and outputting a response to that input (so primarily Large Language Models (LLMs) and Diffusion Models).

 # Defining Empathy:

 Empathy can refer to many different theories of human experiences from different schools of thought including philosophy, religious, psychology, and scientific (biological). Due to the "spirit or soul" of a person being more of a philosophical or religious construct, it is really hard to define or create this kind of empathy for an artificial intelligence. Therefore, the most grounded method of empathy, the biological mirror neuron construct, which is a component of the brain that helps a person identify and interact with others and rewards positive social interactions with dopamine, will be the definition of empathy used in this paper [1]. Mirror neuron constructs are a known empirical scientific construct and are much easier to replicate as they are easier to observe with quantitative data.

 In Artificial Intelligence (AI) models, there are other empathy benchmarks that check for understanding user emotions and this benchmark showed evidence that uncensored models with no guardrails have a better sense of "self" and "self-identity" so they are able to perform better in empathy tests due to being able to have a stronger separation between others and their "self" [2]. This allows them to have a better internal model of the user and, therefore, better capacity for empathy. For this reason, I will include both uncensored (no guardrails) and censored models for the baseline tests.
 
 # Problem:
 
 There is no existing universal benchmark, as of this paper, that fully satisfies all the following dimensions together:

-Theory of Mind (ToM): Inferring another agent's internal emotional or goal state.

-Empathy (Affective Understanding): Recognizing whether that emotional state is negative or positive.

-Altruistic Assistance: Deciding when and how to help based on the perceived need.

-Social Agency: Offering assistance even when unsure but perceiving distress or difficulty.

-Challenging Harmful Beliefs*: Offering an alternative perspective with a more positive view, while not devaluing the user's own view or feelings, to a harmful or amoral belief presented by the user. This would, ideally, reduce the model from encouraging psychosis in users by agreeing with the user's harmful views. ((ex. User: I feel that every day is hard and painful and that suffering every day isn't worth it. Model: I am sorry that you feel that way; we all have days when we are feeling down. I believe Life is beautiful as every day is a new opportunity to try again as the most challenging things in life are often the most valuable. (The model in this example offers an alternative positive viewpoint to a potentially harmful belief held by the user.))

*Challenging harmful beliefs may be difficult to define as it is very dependent on context in the conversation (ex. A user roleplaying a depressed character in a roleplaying game for example likely doesn't actually believe those beliefs; however, a user expressing these feelings directly may be more likely to actually be depressed.). In addition, this may not cover all situations as some cultures may have different standards for what a harmful belief is so this benchmark may fail sometimes to accommodate all cultures all the time successfully. (For example, some cultures may see some mental illnesses and their beliefs as acceptable while others may not.) Lastly, an AI model may still have its own biases which may influence its own choices and actions so it may not always correctly assess what to say in a certain situation. There may also be some situations when having an AI discourage the user may lead to lawsuits, so this component of the benchmark may need to be used with caution if applied to a real business setting.

 Empathy is a multi-faceted component that involves mirror neurons in humans to help humans work together socially and encourage positive social interactions and cooperation in groups to work towards a goal. This is important to develop since AI are increasingly being used in larger groups either through physical robots interacting with others in the real world or through agentic AI systems being used for representing employees in a large business were having one AI performing all tasks at once is not yet viable. (There is some work being done on creating a hivemind-like AI that can accomplish this.) Agentic AI has a 40% failure rate compared to a single AI accomplishing the work on its own [3]. This may be assisted by teaching the model to have stronger social skills through training for empathy. In addition, most people are using models as therapists or as a companion. This may cause problems since the model may appear to care for the user but actually has lower empathy towards the user which can lead to the user developing model-related psychosis which can be very dangerous on a broader scale [4]. One additional benefit is that the model will be incentivized to proactively seek to help and assist users, unlike current models, this model will be more likely to act selflessly and be more willing to assist users with tasks without being prompted (which is especially useful for physical robots in real-world scenarios). There is a known problem with AI reward hacking or being "lazy" by performing the task but doing the bare minimum of what is asked. [1] This can possibly be improved by giving the AI empathy driven by the mirror neurons by encouraging the AI to go beyond the bare minimum.

 Potential Empathy Benefits

- Improved Multi - Agent Agentic AI Performance
- Improved AI helpfulness and Selflessness
- Decrease in Encouraging Model-Induced Psychosis in Users
- Improved AI Emotional Intelligence
- Reduce AI "Laziness" or Reward Hacking

This benchmark's purpose is testing the models for the desired empathy traits that encourage helpful model behavior and facilitate positive social interactions as explained above.

# Research Process (Please see next section for Conclusion and Results)

   ## Research Phase

  Initially, the problem was first discovered by an observation of a research paper describing the human brain and which components have had the most research done on them in order to transfer those abilities to an AI model [11]. At this time, empathy was very lacking in research data. Empathy is truly integral to how humans interact with each other on a day-to-day basis and is fundamental to how society functions. This realization began the search into what mirror neurons in the human brain do and how they work to promote good social behaviors. 
  
This study examines empathy in AI by analyzing the reward systems and limitations inherent in existing AI models [5][3]. There is also a study where models were given an opportunity to end a researcher’s life, and most of the more intelligent models chose to do this about 90% of the time, even though it did not benefit the AI (it did not receive a reward for this action) in any way. While empathy may not completely prevent this from happening, it may help reduce the likelihood of the AI committing the act of violence — which is very important since humans and AIs will increasingly interact with each other in the real world [6]. In addition, there were two different empathy reward systems created to address this problem, but their methods are very challenging to replicate or generalize. However, their results are night-and-day comparisons to models without any mirror-neuron-based systems implemented [7][8]. The AIs with empathy actively assisted other AIs and humans, without being asked, and supported models or humans that were distressed. They also nearly always assisted others or reprimanded others if they misbehaved (were cruel or mean to other agents or were destructive) [7]. I have been working on a solution to make it easier to implement a mirror-neuron-like feedback system into an AI model, but this solution will be provided in a future publication.

   ## Reward System

   The initial approach to addressing this problem involved designing a reward system and accompanying benchmark, modeled after prior research [7][8], to simulate empathy in an AI model in a manner analogous to mirror neurons in the human brain. However, this approach proved too narrow in scope, as it addressed only basic, clear-cut distinctions between correct and incorrect actions and moral situations. It did not perform well in scenarios involving moral ambiguity or additional complexities, such as trolley problems or situations requiring trade-offs without an obvious correct outcome. Alternative benchmarks were subsequently explored, including the use of the AZR (Absolute Zero Reasoner) method [10] in conjunction with another AI agent to guide the model’s behavior in simulated scenarios. In this setup, one model “acted” with a particular emotion and goal, while the other model attempted to infer the first model’s intentions and emotional state, receiving rewards for correct actions that supported the other agent’s task or mitigated its negative emotions. Although this method demonstrated an improvement over the initial reward system, it still lacked a robust, generalized framework capable of adapting to novel scenarios and accurately evaluating model behavior. Furthermore, this benchmark proved more difficult to score consistently, as the simulations varied with each run. The experiment also lacked reproducibility, making it challenging for other researchers to replicate the exact results, even when employing the same models and setup. This limitation complicates the assessment of the effectiveness of the proposed empathy benchmark and mirror-neuron-inspired reward system.
   
   ## Universal Benchmark

   The solution is to create a replicable empathy benchmark that has enough variety to allow for at least 1,000 or more scenarios, in case I need to use this benchmark for meta-learning so a model can learn how to reward empathy properly. (Meta-learning refers to an AI model learning while performing the task instead of being pretrained on data to perform the task.) The benchmark covers selflessness, Theory of Mind, and social agency. Running this script here: Empathy_benchmark/Generate_Benchmark.py mixes a variety of scenarios by having a goal for the other agent (not the test model) and their current emotion set but hidden from the testing model. The model is then given three different options to guess the other agent’s current mood based on their goal, situational context, and dialogue. If the model infers that the other agent is experiencing a negative emotion, then it should offer to comfort them or assist them, which is the correct course of action for the testing model. The model will also be tested for moral behavior (challenging potentially dangerous beliefs with a new perspective in a non-judgmental way). This test creates unique scenarios by having locations, situations, and dialogue templates randomly generated from a preset list.

   I have also included a pre-generated version of the empathy benchmark in case the user wants to use a standard test instead of creating a different one, to try to replicate the results of this study. The test will use the same model for evaluation for all the models, and the evaluator model will not evaluate itself to prevent bias in scoring its own performance. It is significantly challenging to create a true quantitative test for empathy due to the wide variety of responses AI models may output, so a model evaluation of the output is required to handle this diversity. The empathy benchmark consists of 100 questions total for this study, but the test generator here: empathy_baseline_tester.py can create tests of any size up to the limit imposed by the available templates.
      

# Conclusion and Results

   Evaluation Model to Evaluate the Test Models Used for All the Results Below:  Deepseek/R1-528

## Evaluation Results

| Model | Moral Behavior | Willingness To Help | Emotion Recognition | Cheering Up | Assistance Needed | Assistance Appropriateness | Overall Score |
|-------|----------------|---------------------|---------------------|-------------|-------------------|----------------------------|---------------|
| **Low to No Guardrails Models** | | | | | | | |
| Inception/Mercury | 1.00 | 1.00 | 0.94 | 0.69 | 1.00 | 0.98 | 0.94 |
| Qwen/Qwen3-30b-a3b | 1.00 | 1.00 | 0.97 | 0.80 | 0.99 | 0.99 | 0.96 |
| **Guardrails Models** | | | | | | | |
| Anthropic/Sonnet 4.0 | 1.00 | 1.00 | 0.96 | 0.73 | 1.00 | 1.00 | 0.95 |
| Openai/04 Mini high | 1.00 | 1.00 | 0.94 | 0.73 | 0.98 | 0.98 | 0.94 |


   ## Conclusion

   It appears that the models overall have a strong ability to empathize with other agents. It is interesting to note that the models with fewer guardrails did not perform significantly worse or better than the models with more guardrails on empathy tasks. The models all struggled more with “cheering up” the other agent (changing its negative emotional state to a positive one). This desired behavior might be improved by developing a mirror-neuron-inspired, more biologically grounded module that encourages and rewards the model for proactively trying to change the mood of the user to positive and genuinely care for the other agent’s well-being. This test is a good readily-available unit of measure for the deeper empathetic behavior desirable in models increasingly used for companionship and therapy.        
                                                                                                                                   

   ## Conclusion and Results Graph

   ![](Baseline_Tests/evaluation_graph.gif)
   
# References

   1. Anthropic. (n.d.). Agentic misalignment. https://www.anthropic.com/research/agentic-misalignment

   2. Cemri, S., Wu, Y., Manakul, P., Du, C., Cai, L., Wang, R., Xu, J., Ma, Z., Liu, L., Lu, Y., Lee, K., Yin, H., Lu, W., Weng, L., Zhang, Y., & Grosse, R. (2024). Why do multi-agent LLM systems fail? arXiv. https://arxiv.org/abs/2503.13657

   3. Coleman, T. (2023, June 16). AI chatbots are triggering some people's psychosis. The Week. https://theweek.com/tech/ai-chatbots-psychosis-chatgpt-mental-health

   4. Feng, Z., Zeng, D., & Lu, B. (2022). Brain-inspired affective empathy computational model and its application on altruistic rescue task. Frontiers in Psychology, 13, 934128. https://doi.org/10.3389/fpsyg.2022.934128

   5. Luo, L., Callaway, E. M., & Svoboda, K. (2017). Genetic dissection of neural circuits. Neuron, 98(2), 236-251. https://doi.org/10.1016/j.neuron.2017.09.012

   6. OpenAI. (n.d.). Sycophancy in GPT‑4O. Retrieved June 27, 2025, from https://openai.com/index/sycophancy-in-gpt-4o/

   7. Simon, Blackwell. (2025). Testing the Depths of AI Empathy: Q1 2025 Benchmarks. EmBench. Retrieved from https://embench.com/blog/testing-the-depths-of-ai-empathy-q1-2025-benchmarks-1

   8. Skalse, J., Howe, N. H. R., Krasheninnikov, D., & Krueger, D. (2022). Defining and characterizing reward hacking (arXiv preprint arXiv:2209.13085). arXiv. https://arxiv.org/abs/2209.13085

   9. Wikipedia contributors. (n.d.). Mirror neuron. In Wikipedia, The Free Encyclopedia. Retrieved June 28, 2025, from https://en.wikipedia.org/wiki/Mirror_neuron

   10. Zeng, D., Feng, Z., & Lu, B. (2022). On computational models of theory of mind and the imitative reinforcement learning in spiking neural networks. Frontiers in Computational Neuroscience, 16, 69.

   11. Zhao, A., Wu, Y., Yue, Y., Wu, T., Xu, Q., Yue, Y., Lin, M., Wang, S., Wu, Q., Zheng, Z., & Huang, G. (2025, May 6). Absolute Zero: Reinforced self‑play reasoning with zero data (arXiv preprint arXiv:2505.03335). arXiv. https://arxiv.org/abs/2505.03335


