# página 20 — de nist-ai-rmf-100-1.pdf

NIST AI 100-1
AI RMF 1.0
Employing safety considerations during the lifecycle and starting as early as possible with
planning and design can prevent failures or conditions that can render a system dangerous.
Other practical approaches for AI safety often relate to rigorous simulation and in-domain
testing, real-time monitoring, and the ability to shut down, modify, or have human inter-
vention into systems that deviate from intended or expected functionality.
AI safety risk management approaches should take cues from efforts and guidelines for
safety in fields such as transportation and healthcare, and align with existing sector- or
application-specific guidelines or standards.
3.3
Secure and Resilient
AI systems, as well as the ecosystems in which they are deployed, may be said to be re-
silient if they can withstand unexpected adverse events or unexpected changes in their envi-
ronment or use – or if they can maintain their functions and structure in the face of internal
and external change and degrade safely and gracefully when this is necessary (Adapted
from: ISO/IEC TS 5723:2022). Common security concerns relate to adversarial examples,
data poisoning, and the exfiltration of models, training data, or other intellectual property
through AI system endpoints. AI systems that can maintain confidentiality, integrity, and
availability through protection mechanisms that prevent unauthorized access and use may
be said to be secure. Guidelines in the NIST Cybersecurity Framework and Risk Manage-
ment Framework are among those which are applicable here.
Security and resilience are related but distinct characteristics. While resilience is the abil-
ity to return to normal function after an unexpected adverse event, security includes re-
silience but also encompasses protocols to avoid, protect against, respond to, or recover
from attacks. Resilience relates to robustness and goes beyond the provenance of the data
to encompass unexpected or adversarial use (or abuse or misuse) of the model or data.
3.4
Accountable and Transparent
Trustworthy AI depends upon accountability. Accountability presupposes transparency.
Transparency reflects the extent to which information about an AI system and its outputs is
available to individuals interacting with such a system – regardless of whether they are even
aware that they are doing so. Meaningful transparency provides access to appropriate levels
of information based on the stage of the AI lifecycle and tailored to the role or knowledge
of AI actors or individuals interacting with or using the AI system. By promoting higher
levels of understanding, transparency increases confidence in the AI system.
This characteristic’s scope spans from design decisions and training data to model train-
ing, the structure of the model, its intended use cases, and how and when deployment,
post-deployment, or end user decisions were made and by whom. Transparency is often
necessary for actionable redress related to AI system outputs that are incorrect or otherwise
lead to negative impacts. Transparency should consider human-AI interaction: for exam-
Page 15

