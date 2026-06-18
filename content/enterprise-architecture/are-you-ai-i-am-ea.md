+++
title = "Are You AI? I Am EA."
date = 2026-06-18T10:00:00+02:00
draft = false
tags = ["enterprise-architecture", "ai", "ai-governance", "digital-transformation", "technology-strategy"]
summary = "Why probabilistic systems demand architectural governance, not better procedures, and why that puts Enterprise Architecture back at the center."
+++

### Why Non-Deterministic Systems Make Enterprise Architecture Essential Again

## The Revolution That Came Early

On November 30, 2022, OpenAI released ChatGPT to the public. Within five days, a million people had signed up. Within two months, that number had grown to a hundred million monthly active users, making it at the time the fastest-growing consumer application in history [1]. Artificial Intelligence was no longer a research curiosity or a Silicon Valley promise for the next decade. It was in people's homes. It was in their workflows. It was everywhere.

The breakthrough was not architectural. The Transformer, introduced by Google researchers in the 2017 paper "Attention Is All You Need," had already laid the foundation upon which every major language model since has been built [2]. What ChatGPT did was package those advances into a widely accessible interface, and in doing so it forced every organization on the planet to confront a set of questions they were not prepared for: data readiness, compliance in a non-deterministic landscape, and the standards and guardrails that would ensure AI works for us rather than against us.

## The Third Entity

Enterprise Architecture as a discipline traces its origins to the late 1980s and the work of John Zachman at IBM. In 1987, Zachman published "A Framework for Information Systems Architecture" in the IBM Systems Journal [3]. The paper proposed that the growing complexity of information systems required a structured approach, one borrowed from classical architecture and engineering, to define and control the interfaces and integration of system components.

Zachman himself later said he regretted the original title. What he had actually created was not a framework for information systems. It was a framework for the enterprise itself [4]. But at the time, the concept of "Enterprise Architecture" was so foreign that he had to anchor it in something people understood.

His insight was deceptively simple. From an enterprise-design perspective, organizations for centuries could be viewed as operating primarily through people and processes. Technology existed, of course, but it was a tool embedded within processes and operated by people. Even as the industrial era introduced mechanization and the 1970s brought robotic arms to manufacturing floors, technology remained subordinate. It was part of a process. It did not have a life of its own.

That changed with the advent of software and data systems in the 1980s. One useful way to interpret the rise of software is to view technology and data as a third organizational entity, one that influenced people and processes in ways that were often unforeseen and difficult to control. But what does it mean to call technology an "entity" rather than infrastructure? The distinction is operational. Infrastructure serves: it does what it is told and stops when switched off. An entity generates: it creates data on its own, triggers processes no human initiated, and builds dependencies that outlive their creators. Picture a batch system that generates compliance reports overnight, reports that become the trusted input for another system's decisions the next morning, with no person reviewing the hand-off. The output of one machine has become the unquestioned premise of another. At that point technology has crossed from tool to organizational force: it no longer merely supports people and processes, it acts alongside them, sometimes in alignment and sometimes not.

It was in this climate that Zachman suggested we should view the now three entities as an architectural problem and not as one to be solved with traditional management approaches [3]. The Zachman Framework organized people, processes, and technology into a coherent schema by mapping six fundamental questions (what, how, where, who, when, and why) against multiple stakeholder perspectives [5]. It was not a methodology. It was an ontology, a way of classifying the descriptive representations that comprise an enterprise. The distinction matters because it positions EA as a lens for understanding complexity rather than a prescriptive set of steps.

## The Definition Trap and the Power Question

Four decades later, Enterprise Architecture is still fighting for mainstream adoption. The common explanation is that the discipline cannot be clearly defined. This is part of the problem, but only a small part.

Research tells a more uncomfortable story. A 2017 study published by Springer found that EA adoption inherently disrupts existing organizational structures because it "breaks old procedures and habits, shifts decision-making power, and challenges old values" [6]. A study of the Finnish public sector found that resistance towards EA played a more considerable role in adoption challenges than in private companies, and that even when EA was mandated by law, only 17% of organizations had meaningfully adopted it [7]. Research from the Norwegian higher education sector confirmed that EA adoption was severely impeded by a lack of top-level direction and the poor understanding of EA among top management [8].

The pattern across these studies is consistent. EA does not fail because it is poorly defined. EA struggles because it claims a portion of decision-making authority from the traditional management establishment. Organizations that want to practice EA must relinquish some power to architects so they can exercise their prerogative. Many organizations say they are willing to do this. Few actually do it. The "definition trap" is real, but it is often a convenient cover for a more fundamental resistance to power redistribution.

## An Honest Reckoning

But let's be honest about the other side of the coin. EA has not always helped its own cause.

The discipline has a well-documented history of becoming documentation-centric rather than decision-centric. Paul Brubaker, one of the principal authors of the U.S. Clinger-Cohen Act, commented that EA efforts had "all resulted in unusable shelfware" [9]. Vivek Kundra, then the federal CIO of the United States, went further, arguing that EA frameworks were "worse than useless" because architects focused on documenting current and future states while the technology moved on without them [9]. The U.S. federal government alone spent over $836 million on enterprise architecture development by 2006 with limited demonstrable returns [10].

These are not fringe criticisms. They point to a pattern that many EA practitioners will privately acknowledge: the discipline has too often succumbed to framework fetishism, over-modeling, bureaucratic process layering, and a detachment from the operational realities of the organizations it was meant to serve. When an architecture function produces artifacts that nobody reads and governs processes that nobody follows, it is not architecture. It is theater.

This is important context for what follows. The argument here is not that EA as it has been commonly practiced is ready to govern AI. It is that EA as it was always meant to function, focused on decisions rather than documentation, is equipped for the challenge. If AI forces anything, it should force EA to stop being a compliance exercise filed away in SharePoint and start being the structural capability that Zachman originally envisioned.

## Why AI Changes the Equation

This brings us to the present moment, and to the opportunity that Enterprise Architecture has arguably been waiting for without fully realizing it.

Before AI, non-EA management could handle most technology-related issues. Sometimes inefficiently, sometimes messily, but the consequences were manageable. Software was deterministic. A programmer wrote code, tested it, found bugs, and iterated until the solution worked. The outcomes were predictable even when the process was painful.

Generative AI exhibits probabilistic behavior and cannot be governed in the same manner as traditional deterministic software systems. This is not a bug or a limitation to be patched in a future release. It is the fundamental nature of the technology. An AI model accepts an input (deterministic) and produces an output that is influenced by the input but also shaped by the model's internal workings in ways that cannot be fully predicted. The output is not always what was expected, and in some cases, it can contradict what was requested.

The word "hallucination" has become the default term for this phenomenon, but it is a misnomer that does the issue a disservice. When AI models make mistakes, they rarely produce absurd or obviously wrong outputs. They produce text that reads as proficient, accurate, and above all, authoritative. If you are expecting to ask an AI model the capital of France and receive back the date Napoleon was born, you will be disappointed. The errors are far more subtle than that, and that subtlety is precisely what makes them dangerous in enterprise settings.

The numbers confirm both the scale of adoption and the governance vacuum. McKinsey's 2024 State of AI survey found that 72% of organizations were using AI in at least one business function, with 65% reporting regular use of generative AI [11]. Yet only 18% had an enterprise-wide council or board with authority to make decisions involving responsible AI governance [11]. By 2025, adoption had risen to 88% of organizations using AI in at least one function, but nearly two-thirds remained stuck in experiment or pilot mode, unable to scale [12]. A Gartner analysis published in 2026 stated plainly that traditional governance models built for deterministic IT systems are no longer fit for purpose when applied to non-deterministic architectures such as retrieval-augmented generation and autonomous agent-based systems [13].

This is the non-deterministic nature of AI getting traditional management into trouble. How do you shape standards and guardrails for a system that does not guarantee consistent outputs? Do you instruct a non-deterministic system to behave a certain way and hope for the best? Do you ask the people operating a non-deterministic solution to somehow produce deterministic results? For centuries, one approach or the other was sufficient. Not anymore.

The answer, I would argue, is neither. What non-deterministic systems demand is not better procedures but a different kind of governance entirely, one that is probabilistic rather than procedural, designed to absorb unpredictable outputs and channel them toward compliant outcomes.

## The Competition for Governance

It would be intellectually dishonest to pretend that EA is the only discipline reaching for the AI governance mandate. It is not.

Platform engineering teams are building internal developer platforms that embed guardrails into deployment pipelines. MLOps practices are maturing around model lifecycle management, drift detection, and operational monitoring [14]. Legal and compliance offices are creating AI review boards to assess regulatory exposure. Security governance teams are extending their frameworks to cover model risks. Data governance groups are asserting authority over training data quality and lineage. Some organizations are establishing standalone AI councils that sit outside existing structures entirely.

Each of these approaches addresses a real piece of the puzzle, and none of them is wrong. But each of them is partial. A compliance office can flag that an output violates a regulation, but it cannot redesign the information flow that produced it. An MLOps team can detect model drift, but it cannot assess the downstream business impact across interconnected systems. A security team can lock down access, but it cannot tell you whether wiring the AI into a business process creates a new compliance risk somewhere downstream, far from the model itself.

AI governance is not a technology problem. It is not a legal problem. It is not a data problem. It is all of them at once. That is what makes it an architecture problem.

EA's claim is not that it replaces any of these disciplines. It is that none of them can see the whole board. A compliance team governs outputs. An MLOps team governs models. A security team governs access. EA governs the system, the way these functions connect, where authority sits, and how decisions flow across boundaries. The value is not in doing their work but in ensuring their work coheres.

## Architecture as the Answer

Regulated industries, from financial services to pharmaceuticals operating under GxP requirements, are already building layered validation pipelines [15][16]. The pattern is consistent. What they often lack is a way to ensure these patterns are applied consistently across the enterprise rather than reinvented by each project team. Defining patterns once and governing their application across dozens of AI use cases is exactly what EA does.

Consider how this plays out in practice. A bank wants to use a generative AI model to summarize transaction histories into narratives its auditors rely on. The regulatory environment requires that every summary be traceable to source records, that no material transaction is omitted, and that the output meets data-integrity standards for audit evidence [17][18]. The AI model, by its nature, cannot guarantee any of those things. It may omit a low-value but material transaction. It may subtly mischaracterize a counterparty. It may produce a summary that reads perfectly but diverges from the ledger in ways only an auditor would catch.

The non-architectural response is to tell the team to review every output carefully. The architectural response is to design a system where the AI-generated summary is one component within a validation pipeline. The summary passes through an automated comparison layer that checks it against the structured source records. Discrepancies above a defined threshold trigger a human review gate. Every input, output, and decision point is logged to an audit trail that satisfies regulatory traceability requirements. The model is not trusted. The architecture is. The model operates within boundaries that the architecture enforces.

More broadly, multi-layer guardrail architectures are emerging as a best practice across industries, combining input/output gatekeeper layers with knowledge-grounding checks and real-time monitoring agents [15]. These are architectural decisions, not model-level tweaks.

A fair objection at this point: if architecture absorbs governance, compliance, validation, information flow, and organizational structure, does it not become a synonym for everything? It does not, and the boundary matters. Architecture defines systemic constraints and patterns. Operational teams execute within them. The architect does not run the model, review the output, or manage the compliance ticket. The architect designs the system that ensures those things happen reliably and consistently. That distinction is what separates architectural governance from operational micromanagement.

Industry analysts are already recognizing the convergence. Enterprise architects are assuming governance roles in AI adoption, and the emergence of the "Enterprise AI Architect" as a named role signals that the market is catching up to what EA practitioners have long argued [19].

## The Moment

EA has spent nearly four decades arguing that organizations need architects to manage the interplay between people, processes, and technology. For most of that time, organizations could get by without fully committing to that vision. The technology was deterministic. The consequences of poor governance were uncomfortable but survivable.

AI has changed the calculus. Ungoverned, non-deterministic systems operating in compliance-sensitive environments do not produce uncomfortable consequences. They produce potentially existential ones.

This is the shift toward probabilistic governance at work. You cannot write a checklist that governs a system whose outputs you cannot predict. You can design a structure that makes unpredictability manageable. That is not a procedural task. It is an architectural one.

EA is, I would argue, the discipline best positioned to lead that shift. Not because it has a perfect track record. Not because it is the only voice in the room. But because the problem is architectural in nature, and architecture is what EA was built to do. Whether it earns that role depends on two things: whether organizations have the foresight to let architects lead, and whether architects have the discipline to do it right.

---

### References

[1] "ChatGPT sets record for fastest-growing user base - analyst note," Reuters, February 1, 2023. Available: https://www.reuters.com/technology/chatgpt-sets-record-fastest-growing-user-base-analyst-note-2023-02-01/

[2] A. Vaswani et al., "Attention Is All You Need," *Advances in Neural Information Processing Systems (NeurIPS)*, 2017. Available: https://papers.neurips.cc/paper/7181-attention-is-all-you-need.pdf

[3] J. A. Zachman, "A Framework for Information Systems Architecture," *IBM Systems Journal*, vol. 26, no. 3, pp. 276-292, 1987.

[4] "A Historical Look at Enterprise Architecture with John Zachman," The Open Group / Zachman International, 2024. Available: https://zachman-feac.com/resources/ea-articles-reference/164-a-historical-look-at-enterprise-architecture-with-john-zachman-an-interview-with-the-open-group

[5] "The Zachman Framework Evolution," Zachman International / FEAC Institute, 2024. Available: https://zachman-feac.com/the-zachman-framework-evolution

[6] D. D. Dang and S. Pekkola, "Problems of Enterprise Architecture Adoption in the Public Sector: Root Causes and Some Solutions," *Integrated Series in Information Systems, vol. 38*, Springer, 2017.

[7] V. Seppänen, K. Penttinen, and M. Pulkkinen, "Key Issues in Enterprise Architecture Adoption in the Public Sector," Electronic Journal of e-Government, vol. 16, no. 1, pp. 46–58, 2018.

[8] T. Breivik and S. S. Dahl, "Enterprise Architecture Adoption Challenges: An Exploratory Case Study of the Norwegian Higher Education Sector," *Procedia Computer Science*, vol. 100, 2016.

[9] S. Kotusev, "Enterprise Architecture Frameworks: The Fad of the Century," *British Computer Society (BCS)*, 2023. Available: https://www.bcs.org/articles-opinion-and-research/enterprise-architecture-frameworks-the-fad-of-the-century

[10] U.S. Government Accountability Office, "Enterprise Architecture: Leadership Remains Key to Establishing and Leveraging Architectures for Organizational Transformation," GAO-06-831, August 2006. Available: https://www.gao.gov/products/gao-06-831

[11] McKinsey & Company, "The State of AI in early 2024: Gen AI adoption spikes and starts to generate value," May 2024. Available: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai-2024

[12] McKinsey & Company, "The State of AI in 2025: Agents, innovation, and transformation," November 2025. Available: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai

[13] S. Agarwal (VP Analyst, Gartner), "Why CIOs must integrate governance into enterprise AI," CIO Dive, April 2026. Available: https://www.ciodive.com/news/AI-governance-gartner-sumit-agarwal/816720/

[14] Gartner, "Gartner Predicts 40% of Organizations Deploying AI Will Use AI Observability to Monitor Model Performance by 2028," Gartner Newsroom, May 2026. Available: https://www.gartner.com/en/newsroom/press-releases/2026-05-12-gartner-predicts-40-percent-of-organizations-deploying-ai-will-use-ai-observability-to-monitor-model-performance-by-2028

[15] EY Switzerland, "GxP and AI tools: Compliance, Validation and Trust in Pharma," October 2025. Available: https://www.ey.com/en_ch/insights/life-sciences/gxp-and-ai-tools-compliance-validation-and-trust-in-pharma

[16] "Risk-Based Validation of Software, Automation and Artificial Intelligence in Pharmaceuticals," Biosciences Biotechnology Research Asia, December 2025. Available: https://www.biotech-asia.org/vol22no4/risk-based-validation-of-software-automation-and-artificial-intelligence-in-pharmaceuticals/

[17] Sarbanes-Oxley Act of 2002, Pub. L. 107–204, §404, "Management Assessment of Internal Controls." U.S. Government Publishing Office. Available: https://www.govinfo.gov/content/pkg/COMPS-1883/pdf/COMPS-1883.pdf

[18] PCAOB, "AS 1105: Audit Evidence." Public Company Accounting Oversight Board. Available: https://pcaobus.org/oversight/standards/auditing-standards/details/AS1105

[19] "Enterprise Architecture and Digital Transformation Trends for 2025," Orbus Software, 2025. Available: https://www.orbussoftware.com/resources/blog/post/enterprise-architecture-and-digital-transformation-trends-for-2025
