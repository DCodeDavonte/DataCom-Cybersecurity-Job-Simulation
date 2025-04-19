# 🧠 Risk Assessment Report Reflection

This task involved conducting a full risk assessment for a hypothetical small community health clinic. Unlike Task 1, which focused on threat actor research, this pushed me to take on a broader, more strategic cybersecurity perspective — one that’s grounded in consulting, communication, and real-world feasibility.

---

## 🔍 Initial Planning and Framing

The simulation didn’t provide much about the organization itself, aside from the fact that it had a fenced perimeter and a padlock. That gave me flexibility to design a realistic client profile. I decided to base my risk assessment on a **small, standalone health clinic** — the kind that might have a front desk, a couple of exam rooms, local data access, and perhaps a basic internal network. I kept it within this scope because it allowed me to ground my controls and threats in something plausible. It also helped me imagine the people involved — the kind of staff who might use shared workstations, have limited technical literacy, and rely on physical and digital security being quietly reliable in the background.

Before diving into risk scenarios, I needed to choose a structure. Rather than use a generic checklist or cut-and-paste scoring system, I built the risk matrix based on common formats I've seen across NIST frameworks and GRC documentation — using a **1 to 5 scale** for both likelihood and consequence. I also made sure to define how I interpret those scores, since qualitative reasoning is just as important as the numbers themselves.

---

## 🧩 Selecting Risk Scenarios

I wanted to approach this from different attack surfaces: one external, one physical, and one internal. That gave me:

1. **Phishing attack** – a common and highly scalable vector that threatens nearly every business regardless of size.
2. **Physical perimeter breach** – taking the scenario literally and imagining what happens if someone walks past the fence and gains physical access to devices.
3. **Insider access misuse** – often overlooked but potentially devastating, especially in smaller orgs where RBAC and offboarding procedures are often informal or inconsistent.

These covered social engineering, physical threats, and access control — three foundational pillars of any risk posture.

---

## 🧮 Scoring and Realism

When assigning initial risk scores, I tried to weigh each risk the way a consultant would: by asking not just “how likely is this?” but “what’s the real-world impact if this actually happened?” For example:

- The **phishing scenario** felt the most likely to occur and could affect the most systems. Even without technical complexity, one compromised credential could open the floodgates.
- The **insider access misuse** was trickier. It forced me to think about privilege creep and inherited permissions. In many clinics, access is granted for ease of workflow — not because it’s needed. That made me more cautious when scoring the consequence.
- The **physical breach** was an interesting challenge. I initially wondered if it even belonged in a digital-focused risk assessment — but realized quickly that **physical access is often digital access** if the perimeter isn’t segmented. I used realistic assumptions: there are probably no cameras or motion sensors, and once someone is in, they might have access to terminals or paper records. That justified keeping its consequence score relatively high.

I avoided downgrading a consequence score unless it was clear that mitigation would shrink the actual impact, not just delay it.

---

## 🛡️ Thinking Through Existing Controls

This part required nuance. I assumed the clinic had basic protections — antivirus, spam filtering, locked doors — but not much more than that. It wouldn't be realistic to assume they had full SIEM visibility or enforced RBAC reviews.

I evaluated the **effectiveness of those baseline controls** honestly: spam filtering works, but without MFA and training, phishing still succeeds. Fences deter, but don’t stop. Logins exist, but access is often over-provisioned.

Rather than assume the worst or best case, I made small, justifiable inferences based on what similar organizations might have in place — and rated them accordingly using “weak,” “moderate,” and so on.

---

## 🏗️ Designing Improvements

The second half of the task focused on **how to reduce those risks** in a practical way. Here’s where I leaned into my knowledge and preferences — because this is where problem-solving starts to feel creative.

I asked myself:
- What’s scalable?
- What’s cost-conscious?
- What improves visibility without overwhelming staff?

Instead of suggesting overbuilt solutions, I recommended controls that many organizations can implement incrementally: MFA, phishing simulations, EDR, role-based access reviews, vendor segmentation, and more. These weren't just theoretical — I thought about their impact if I were an IT admin inside that clinic, trying to balance security with simplicity.

The **physical security** measures were particularly interesting. Things like motion lights and cameras aren't just about stopping an intruder — they change how people behave. It was the first time I really thought about how **psychological deterrence and perception of risk** play into the threat model.

---

## 💬 Final Thoughts

This task helped clarify that I enjoy the analytical and communicative aspects of cybersecurity — especially the process of **translating technical concepts into leadership-aligned insights**. It pushed me to think beyond systems and consider behavior, environment, and budget.

It also reinforced that **GRC might be a strong future path for me**. I enjoy asking "what if?", mapping it to something measurable, and offering something that doesn't just look good on paper, but makes sense in context.

If I had more time, I’d probably expand this into a visual risk report with asset diagrams and impact chains. But for this scope, I’m confident that I built something thorough, reasoned, and practical — exactly the type of document I’d want to present to a client.

