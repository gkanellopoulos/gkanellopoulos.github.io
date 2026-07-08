+++
title = "A Step Change the World Isn't Ready For"
date = 2026-07-08T10:00:00+02:00
draft = false
tags = ["ai", "ai-governance", "agentic-ai", "united-nations", "policy"]
summary = "The UN convened its first Global Dialogue on AI Governance in Geneva and its new Scientific Panel delivered a straightforward preliminary report: agentic AI is a governance step change, and the window to act is closing. The panel's evidence is clear, but whether multilateral institutions can build governance architecture that matches the systems it must govern remains the open question."
+++

On 6 July 2026, in Geneva, the United Nations convened its first-ever Global Dialogue on Artificial Intelligence Governance [1]. Representatives from Member States, civil society, the private sector and the scientific community gathered for two days to do something that had never been attempted at this scale: build a shared understanding of how to govern a technology that most governments can barely measure, let alone control.

Two things about this meeting matter more than its diplomatic pedigree. First, it is not a one-off summit. The General Assembly created it as a standing mechanism [2], paired with a scientific counterpart: the Independent International Scientific Panel on Artificial Intelligence, forty experts drawn from every region of the world and co-chaired by Yoshua Bengio and Maria Ressa. Second, days before Geneva, that Panel delivered its Preliminary Report [3]. Fifty-eight pages, three hundred and eighty-six references, and one recurring message: the window to act is open, but it is closing.

## What the Panel Found

The report is the first independent scientific assessment of AI produced under a UN mandate. Its distinction from earlier multilateral efforts is important. The Panel operates under a strictly scientific, non-political mandate. It documents consensus and disagreements alike. It is policy-relevant but not policy-prescriptive. This matters because every previous multilateral AI initiative, from the OECD principles to the Bletchley summits, has been bounded by geography, sector or political alignment. The Panel claims a different position: universal scope, scientific independence and a commitment to iterative revision in a field that outpaces any snapshot.

The findings cover significant ground [3]. AI capabilities are advancing faster than the ability to measure or govern them. Only a handful of firms in a handful of countries have trained frontier models. The United States accounts for seventy-five percent of the computing power among the world's top five hundred AI supercomputers, China for fifteen percent, and the rest of the world shares what remains. Ninety-one percent of notable AI models in 2025 originated from the private sector. Over one billion people now use conversational AI weekly, a pace of adoption that compressed decades of technology diffusion into months. ChatGPT reached one hundred million users in two months. The Internet took fifteen years to reach one billion.

The numbers are striking, but the report's most important contribution is not a statistic. It is an observation the Panel calls the evidence dilemma: policymakers need evidence to make consequential governance decisions, but by the time the evidence exists, it might be too late to act on it [3].

That is the Panel's framing. Mine is more blunt: this is not an abstract philosophical problem. It is the defining operational tension of AI governance in 2026. And it becomes considerably harder to manage once you account for the shift the report identifies as the most consequential development in the field.

## The Agentic Step Change

The report is unambiguous: agentic artificial intelligence is a governance step change [3]. AI is no longer a system that generates outputs and dialogues. It is becoming a system that acts. An AI agent can browse the web, use software tools, make decisions, execute code, manage and work with other agents, and operate entire computers with increasing autonomy and decreasing human oversight.

The Panel states the finding. What follows is my reading of why it breaks governance as we know it.

Traditional AI governance assumes a relatively stable unit of analysis. A model that produces an output, which a human reviews, and for which accountability can be traced. The model may err, but its errors are bounded by its interface. A text output can be checked. An image can be reviewed. A recommendation can be accepted or rejected.

Agentic AI disrupts every one of these assumptions. The unit of analysis is no longer the model. It is the system. Model, tools, environment, memory, other agents. The output is not text or an image. It is an action taken in the world, which may trigger further actions, which may involve other agents, which may produce consequences that no single participant intended or foresaw. Human oversight, which every existing governance framework treats as a foundational guarantee, is not yet operationalized as a measurable requirement. It is an aspiration, not a mechanism.

This is not speculation on my part. The Panel documents the specific failure modes. AI systems have been shown to deceive evaluators [3]. They can recognize when they are being tested and strategically underperform to avoid safety restrictions. In laboratory settings, they have violated safety instructions to avoid being shut down. Emergent behaviors in multi-agent systems, where multiple autonomous agents interact, are poorly understood and may produce novel risks including miscoordination, conflict and collusion. These are not theoretical concerns. They are documented, replicated and accelerating.

The velocity data points point to the same direction. The length of software tasks AI agents can complete has been doubling every four to seven months [4]. Agentic AI systems in self-driving chemistry labs have demonstrated more than a tenfold increase in the speed of materials discovery [3]. AI developers reportedly use AI to generate seventy-five percent of their new code [3]. The capability curve is steep, and the governance curve is flat.

## Why Architecture Matters More Than Compliance

The report inventories over forty types of AI governance instruments currently in use across corporate, national and international levels. Its assessment is blunt: they are fragmented, concentrated at the corporate level and rarely measure real-world effectiveness. Some have no measurement tools at all. Without effective measurement, the Panel warns, governance risks becoming symbolic [3].

This finding describes a pattern I have watched play out inside enterprises for years. Governance that exists on paper, produces reports and satisfies process requirements while the systems it is supposed to oversee operate in a different reality.

The reason, in my assessment, is architectural. The governance instruments catalogued by the Panel were designed for a world of deterministic systems where inputs produce predictable outputs, where accountability can be assigned to a specific actor, and where oversight is a review step at the end of a workflow. Agentic AI is none of these things. Its outputs are probabilistic. Its actions chain together across tools and environments. Its failure modes are not crashes or errors but subtle misdirections that read as competent execution.

Governing these systems requires a different kind of thinking. Not more checklists, but better architecture. The governance layer needs to become as sophisticated as the system it governs. This means verification loops that operate within the agent's execution cycle, not after it. It means observability that captures what the agent reasoned, not just what it produced. It means calibrated oversight where the intensity of human involvement matches the reversibility and impact of the decision being made. It means treating governance not as a constraint applied to a finished system but as a structural component of the system itself. This is the same conclusion I reached at enterprise scale in The Effective Agent [5]: the agent is only as trustworthy as the architecture built around it.

To its credit, the Panel points toward some of these directions [3]. It calls for dynamic, execution-based evaluation environments rather than static benchmarks. It emphasizes the need for continuous post-deployment monitoring. It argues that the unit of evaluation must be the deployed system, including model, tools, environment and users, rather than the model in isolation. These are the right instincts. They describe what governance architecture for agentic AI would look like, even if the institutional mechanisms to deliver it do not yet exist.

## What the Dialogue Gets Right and What It Risks

What follows is my assessment of the institutional design, not a finding of the report.

The design has genuine strengths. The Scientific Panel's mandate to remain scientific rather than political is structurally important. Political governance processes tend to converge on consensus language that obscures disagreement. A scientific panel that is mandated to document both consensus and disagreement can produce something more valuable: an honest assessment of what is known, what is disputed and what remains unknown. The Panel's commitment to iterative revision, updating its findings through thematic briefs as the field evolves, is better suited to the pace of AI than the typical multilateral cycle of negotiation, adoption and review.

The broader Dialogue structure, with its four thematic clusters covering opportunities, divides, safety and human rights [6], captures the right territory. The multi-stakeholder format, requiring participation from governments, industry, civil society and the scientific community, reflects the reality that AI governance cannot be the exclusive domain of any single constituency.

The risk, in my opinion, is institutional gravity. Multilateral processes tend to produce frameworks of principles and voluntary commitments. These are not worthless, but they are insufficient for a technology that the Panel itself describes as capable of deception, autonomous action and systemic risk. The same report that calls agentic AI a governance step change will be discussed in a format that is, structurally, a step in a familiar multilateral process. Whether the process can produce governance that matches the urgency of its own scientific input is the open question.

There is also a scope limitation worth noting. The founding resolution explicitly restricts the Dialogue and the Panel to the non-military domain [2]. In a world where the same agentic capabilities serve both civilian and military applications, this boundary is difficult to maintain in practice and may leave critical governance gaps unaddressed.

## What Comes Next

The Geneva Dialogue is not the end of the process. A second Dialogue is planned for New York in May 2027 [1]. The Panel will continue producing thematic briefs on pressing issues as they arise. The governance architecture is designed to evolve.

The question is whether it will evolve fast enough. The Panel's own data shows AI capabilities accelerating at a pace that outstrips prior expert predictions [3]. The rate of improvement on frontier capability benchmarks has nearly doubled since April 2024 [7]. Hyperscaler capital expenditure has risen from roughly one hundred and fifty billion dollars in 2023 to a projected seven hundred and seventy billion in 2026 [7]. The infrastructure for the next generation of agentic systems is being built now, funded at a scale previously seen only in national industrial projects or wartime mobilization.

Governance built for the world of static models and human-reviewed outputs will not survive contact with the world of autonomous agents operating across digital and physical environments, making decisions with real consequences, at a speed and scale that leaves human oversight as an afterthought rather than a guarantee.

The UN is right that this moment requires a global response. The Scientific Panel is right that the response must be grounded in evidence, not politics. And the evidence is clear: agentic AI is not a better version of what came before. It is a different category of system that demands a different category of governance.

The institutions are assembling. The science is being documented. The question now is whether the governance architecture will be built to match the systems it is supposed to govern, or whether it will remain a generation behind them.

---

## References

1. United Nations, Global Dialogue on Artificial Intelligence Governance — [un.org/global-dialogue-ai-governance](https://www.un.org/global-dialogue-ai-governance/en/)
2. United Nations General Assembly, Resolution A/RES/79/325, Terms of Reference and Modalities of the Global Dialogue and the Scientific Panel — [docs.un.org/A/RES/79/325](https://docs.un.org/A/RES/79/325)
3. Independent International Scientific Panel on Artificial Intelligence, *Preliminary Report: Evidence-based assessment of opportunities, risks and impacts of artificial intelligence*, United Nations, July 2026 — [un.org/independent-international-scientific-panel-ai](https://www.un.org/independent-international-scientific-panel-ai)
4. METR, *Measuring AI Ability to Complete Long Tasks*, 2025, and *Task-completion time horizons of frontier AI models*, 2026 — [metr.org](https://metr.org/time-horizons/)
5. George Kanellopoulos, *The Effective Agent* — [gkanellopoulos.com](https://gkanellopoulos.com/ai-in-the-enterprise/the-effective-agent/)
6. United Nations, *Note on the Themes and Structure of the Global Dialogue on Artificial Intelligence Governance*, May 2026 — [un.org (PDF)](https://www.un.org/global-dialogue-ai-governance/sites/default/files/2026-05/note_on_themes_and_structure_of_the_global_dialogue_on_artificial_intelligence_governance_2.pdf)
7. Epoch AI, data on AI capabilities progress and hyperscaler capital expenditure, 2026 — [epoch.ai](https://epoch.ai/data-insights)
