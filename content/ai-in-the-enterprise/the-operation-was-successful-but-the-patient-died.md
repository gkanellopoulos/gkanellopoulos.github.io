+++
title = "The Operation Was Successful, But The Patient Died"
date = 2026-06-26T09:22:03+02:00
draft = false
tags = ["ai", "ai-governance", "llm", "evaluation"]
summary = "The term hallucination creates a dangerous false impression in enterprise settings. A simple expert-driven framework for evaluating LLM outputs on two axes: completeness and accuracy."
+++

No term has dominated the GenAI conversation more than "hallucination". We adopted it without questioning what it implies: that LLM errors are dramatic, obvious, and immediately recognizable. They are not. And that misunderstanding is shaping how enterprises evaluate their AI solutions.

Across enterprises today, GenAI solutions pass their evaluations while the business outcome suffers from subtle, undetected errors. The operation is successful. The patient dies.

## The Wrong Metaphor

Researchers have challenged the term on anthropomorphic grounds. By calling these errors "hallucinations", we imply the model experiences and perceives things as a human would [1]. We encourage users to assign cognitive processes to what is, at its core, statistical pattern completion [2]. We anthropomorphize the machine, which carries its own risks [3].

Researchers have proposed alternatives. The term "confabulation" has appeared in scientific literature as a more accurate description [4][5]. Its definition, the *"unintentional creation of false narratives that the speaker believes are true, filling gaps in memory,"* maps closely to how a language model actually errs.

## Automating the Problem Away

When the industry realized that the "hallucination" problem was not going to go away anytime soon it did what it always does: old solutions applied to new problems. Automated metrics like BLEU, ROUGE, METEOR and BERTScore offered surface-level similarity checks but correlated poorly with human judgment. As LLMs grew more capable, a new idea emerged: use an LLM to judge another LLM.

It is still automated. It still misses the subtle mistakes. Human subject matter experts agree with LLM judges only 64 to 68% of the time [6]. LLM judges can only reliably evaluate responses on questions they themselves can answer correctly, a circular dependency that defeats the premise [7]. They also exhibit systematic biases. Change the order of the answers and the judgment flips. Make an answer longer and it scores higher, even when it is wrong. Use a model to judge its own outputs and it favors them [8][9].

Research suggests that hallucination is an inevitable property of large language models [10]. If every automated approach keeps failing at the same task, perhaps the task itself requires something other than automation.

## The Devil in The Details

Human evaluation is widely acknowledged as the gold standard, yet dismissed as costly, time-consuming and unscalable. The existing critique focuses on linguistic accuracy and philosophical framing. What has gone unaddressed is the operational damage.

The word "hallucination" creates a dangerous false impression in enterprise settings. It implies LLM errors are dramatic, obvious, and absurd, like a person seeing things that aren't there. But a language model is equally convincing whether it is right or wrong [11].

Consider an LLM summarizing a technical document. The summary reads fluently, uses the correct terminology, follows the expected structure. One figure is wrong. Automated evaluation passes it. An LLM judge passes it. Only a domain expert with access to the source material catches it. The real threat isn't fabricated facts but convincingly false reasoning [12]. The word "hallucination" primes people to look for the wrong kind of error.

More often than not, the errors are subtle, minor, and read as authoritative. This mismatch between the connotation of the term and the reality of the errors leads teams to underestimate the difficulty of evaluation.

## Small Hinges Swing Big Doors

There is a simpler approach. It is manual, it requires domain expertise, and it works.

### Assemble a Team

The first requirement is a team of domain experts. Their role goes beyond evaluating outputs. They define the thresholds under which an output is accepted or rejected.

### The Axes

Evaluation happens along two axes: Accuracy and Completeness. Each is scored on a simple scale (e.g. 1 to 5), and the key insight is that the thresholds are independently tunable based on the risk profile of each solution.

A compliance report for a regulatory body might require five out of five on both axes. A customer service tool might require five out of five on accuracy but accept three out of five on completeness: accurate information, but not exhaustive. That distinction matters. It means the same framework adapts to fundamentally different risk profiles without changing its structure.

### The Corpus

The third component is a corpus of test data against which the domain experts will validate the solution outputs. The test data should be pre-selected carefully and should reflect the challenges the solution will face in non-deterministic scenarios of interaction not only at the current moment but also in the future.

### The Cycle

Once the stakeholders have all the pieces in place the evaluation cycles can begin. The solution produces outputs based on the test corpus, the team of domain experts grades them against the pre-defined scales of the Accuracy/Completeness axes and lastly a determination is made of whether or not the output is acceptable.

When outputs fall short, the engineering team, domain experts and business stakeholders review together what needs to change. The adjustment might be at the prompt level, the context level, or in the evaluation criteria themselves. Then the cycle repeats. Each iteration produces information that is valuable to all parties, not just the engineers.

## A Worked Example

Consider a solution that summarizes regulatory documents for a compliance team. The stakes are high. The domain experts set the acceptance thresholds at five out of five for accuracy and four out of five for completeness. A summary that misses a minor procedural detail is tolerable. A summary that misstates a regulatory requirement is not.

In the first cycle the solution produces summaries for twenty pre-selected documents. The experts score each one. Twelve pass. Five score well on accuracy but fall short on completeness. Three contain factual errors. The team reviews the failures together. The engineers adjust the prompt and the retrieval context. The domain experts refine the test corpus to include edge cases the first round exposed. The second cycle runs. Fifteen pass. By the fourth cycle, eighteen pass and the two remaining failures are in documents with ambiguous source material that the team decides to flag for manual review rather than automate.

No automated metric would have caught the three factual errors in the first round. No LLM judge would have known that a regulatory requirement was misstated. The domain experts did, because they knew what the documents were supposed to say.

## Reflective Emergent Benefits

Each cycle brings the solution closer to trustworthy outcomes. But there is a less obvious benefit.

In traditional software delivery, business stakeholders define requirements and engineering teams build to spec. With deterministic software, this works well enough because the spec describes a predictable outcome. With GenAI, no one can fully predict how the solution will behave. When automated testing is the only feedback loop, stakeholders remain disconnected from reality until the solution fails in production.

Under this framework, stakeholders collaborate continuously. They see the outputs, discuss the scores, and shape the evaluation criteria alongside the engineers. The result is not only a better solution but more informed business stakeholders and domain experts. Continuous collaboration between builders, evaluators and sponsors throughout the lifecycle of a solution is something the software industry has pursued for decades. This framework makes it a structural requirement rather than an aspiration.

## Time is Constant

The proposed approach might seem time consuming and costly. But a poorly made solution creates technology debt. The time saved building it is spent fixing it. Now consider how this gets magnified when the outcomes are non-deterministic and the user knows they are interacting with AI. Users approach AI solutions with a readiness to distrust that traditional software rarely faces. The time you save on evaluation you will spend on remediation, reputation repair, and rebuilding trust. Time is a constant. It is better spent before the solution reaches the user than after.

And the consequences go beyond lost time. Legal exposure and compliance misalignment, once rare edge cases, become real threats when a confident, fluent, subtly wrong output reaches the wrong audience.

## The Patient Needs to Live

The car you drive has been crash tested for months, sometimes years, before you ever touch the steering wheel. The manufacturer does not know if you will collide with a truck or a train. It only knows that if you do, you need to survive. That is what evaluation is for.

The same is true with GenAI. The stakeholders will never know what the user interaction will look like. They have only one option. Build and evaluate the solution so that it is at the very least usable in most circumstances.

Stop treating evaluation as a tooling problem. Start treating it as an expertise one. Pick one solution. Assemble a small team of people who actually understand the domain. Define what "accurate enough" and "complete enough" mean for that specific use case. Run one evaluation cycle. You will learn more in that single cycle than in a year of automated benchmarks. The patient needs to live.

---

[1] E. M. Bender, Mastodon post calling "hallucinate" a "terrible word choice...suggesting as it does that the language model has *experiences* and *perceives things*," November 2022. Available: https://dair-community.social/@emilymbender/109355539906866849

[2] M. Shanahan, "Talking About Large Language Models," *Communications of the ACM*, vol. 67, no. 2, 2024. Preprint: arXiv:2212.03551.

[3] G. Smith, "An AI that can 'write' is feeding delusions about how smart artificial intelligence really is," Salon, January 1, 2023. Available: https://www.salon.com/2023/01/01/an-ai-that-can-write-is-feeding-delusions-about-how-smart-artificial-intelligence-really-is/

[4] "Hallucination or Confabulation? Neuroanatomy as metaphor in Large Language Models" (PLOS Digital Health, 2023).

[5] "Confabulation: The Surprising Value of Large Language Model Hallucinations" (ACL, 2024).

[6] "Limitations of the LLM-as-a-Judge Approach for Evaluating LLM Outputs in Expert Knowledge Tasks" (ACM IUI, 2025).

[7] "No Free Labels: Limitations of LLM-as-a-Judge Without Human Grounding" (arXiv 2503.05061, 2025).

[8] "Can LLMs Replace Human Evaluators? An Empirical Study of LLM-as-a-Judge in Software Engineering" (arXiv 2502.06193, 2025).

[9] J. Gu et al., "A Survey on LLM-as-a-Judge" (arXiv 2411.15594, 2024).

[10] "Hallucination is Inevitable: An Innate Limitation of Large Language Models" (arXiv 2401.11817, 2024).

[11] "Can AI Chatbots Reason Like Doctors?" (IEEE Spectrum, 2026).

[12] Van der Meer, "When Probable Words Mislead: Reframing LLM Limitations as a Decision Risk" (The Economy, 2026).
