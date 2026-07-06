### Hi, I'm Chandana

I build production AI systems for healthcare at Solix Technologies: multi-agent
orchestration, RAG pipelines, LLM fine-tuning, and the backend that holds it
together. That work lives on company infrastructure, so it is not here.

What is here is the work I do to think through hard problems on my own time,
mostly around safe AI for network operations. These projects share a thesis I
care about: an LLM should propose, a formal tool should verify, a human should
approve, and the system should prove that what it claimed would happen actually
happened. AI where it earns its keep, determinism where determinism matters.

A few I would point you to first:

- **[closcall](https://github.com/ChandanaNandi/closcall)** —
  evidence-grounded incident command for a containerized SR Linux datacenter
  fabric, and the fullest expression of the thesis above. A 312-incident fault
  corpus collected under live traffic shows classical detection is structurally
  blind to gray faults (AUROC 0.500) while temporal learned models recover them
  (~0.91) — every published number generated from one content-hashed run.
  Remediation is human-approved through a browser console whose approve button
  and executor share a single digest-bound gate: the UI cannot claim more safety
  than the executor enforces, and a test proves there is no side door.

- **[sonic-intent-agent](https://github.com/ChandanaNandi/sonic-intent-agent)** —
  natural language to verified network config on a SONiC switch, with a local
  LLM, Batfish pre-apply verification, and structural post-apply checks. Built
  in seven phases, each gated by a working demo.

- **[neuronoc-network-ops-assistant](https://github.com/ChandanaNandi/neuronoc-network-ops-assistant)** —
  a safety-first NetOps console: anomaly detection, a LangGraph analysis
  workflow, LLM root-cause explanation, and admin-approved remediation that is
  plan-only by construction. No execution path exists in the code, and a CI scan
  enforces it.

- **[evpn-vxlan-frr-lab](https://github.com/ChandanaNandi/evpn-vxlan-frr-lab)** —
  a containerized leaf-spine fabric: eBGP underlay, BGP-EVPN type-3 control
  plane, VXLAN data plane, with a Python validator on FRR and Docker.

I came to AI from Aircraft Maintenance Engineering, a field where systems fail
loudly and safety is not optional, then an MS in Data Science. That background is
why my projects are honest about their limits and built to be verified rather
than trusted.

Open to conversations about healthcare AI, agentic systems, and ML infrastructure.

- MS Data Science, University of the Pacific
- 📍 Dallas–Fort Worth, TX
- [LinkedIn](https://www.linkedin.com/in/chandana-nandi-3339bb1a5/)
