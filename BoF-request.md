Name: HP-WAN (High Performance Wide Area Network)
Description
High-Performance Wide Area Networks (HP-WANs) are WANs that are engineered to meet the stringent demands of high-speed, low-latency, and ultra-high-volume applications in environments such as research, academia, and large-scale data processing. These networks must efficiently handle high-throughput transmissions (particularly for large transactions), optimize available bandwidth, and ensure resilience, often where minimizing latency is critical.

Previously, HP-WAN practices have commonly relied on dedicated resources and over-provisioning of network capacity to meet these demands, for example in private networks deployed for the purpose. In the case of the most prominent example in the research and education (R&E) networking community, the Worldwide Large Hadron Collider Computing Grid (WLCG), multiple PB are moved on a daily basis through a multiple-tier infrastructure spanning over 170 sites in over 40 countries. The infrastructure is a mixture of dedicated optical private networks (LHCOPN), a layer 3 overlay (LHCONE) and shared, general R&E links.

The thrust of the BoF will be to bring together interested parties, including those operating R&E infrastructures, to discuss existing practices, what works, what does not work. The output of the BoF would be to document requirements for such infrastructures, and then identify potential avenues for IETF work to improve transport protocols to make large-scale data transfers more effective over wide-area, high RTT, potentially lossy paths, where the physical (inter-continental) infrastructure may be shared between multiple research and science communities.

There are established general best practices around local network architectures for end sites, data transfer node tuning, and effective software tools as documented by the ESnet Science DMZ model, but the question of optimising transport protocols for the "hp-wan" paths remains open, with ongoing experiments (for example) with BBRv3, jumbo frames (9000 MTU) and packet pacing. The BoF would aim to discuss such optimisations, and whether new IETF work could be applicable.

In shared networks there may be a mix of data flows - general email or web browsing, time-sensitive media, and larger bulk data transfer flows. Managing elephant flows (in the terabyte-to-petabyte range), which may have defined transmission schedules and durations, frequently pushes the limits of current technologies. Network nodes may benefit if they could have fine-grained awareness of HP-WAN connectivity services.

While advancements in scheduling and routing technologies have been made, examples in the R&E space including SENSE and NOTED, the most pressing challenges remain at the transport layer.

The HP-WAN Non-Working Group Forming BoF aims to collect state-of-the-art experience from previous and current deployments, show current best practice and highlight gaps and transport protocol mechanism improvements needed:

It will discuss key use cases and existing transport-related techniques (including QUIC, DCTCP, L4S, IPv6, Jumbo frames, CONEX and ROCEv2) currently used for localised high performance computing (HPC) scenarios but often with limitations;

Identify the gaps in existing WIT transport mechanisms for high-volume data congestion control, queue management and flow monitoring;

Provide an analysis of existing transport mechanisms and determine whether additional extensions or modifications to transport protocols are required to support HPC over shared WAN infrastructure.

Presentations at the BoF will be led by from those who operate private HPC networks and NRENs, as well as operators from Internet providers who seek to deliver HPC services over shared infrastructure. The intention of the this Non-WG Forming BoF was to seek advice from the IETF on what improvements could be made to existing WIT techniques and why.

Required Details
Status: Non WG Forming
Responsible AD: Zaheduzzaman Sarker (zahed.sarker.ietf@gmail.com)
BOF proponents: Daniel Huang (huang.guangping@zte.com.cn),Kehan Yao(yaokehan@chinamobile.com), Tim Chown (Tim.Chown@jisc.ac.uk),Daniel King (d.king@lancaster.ac.uk),Chris Rapier <rapier@psc.edu>
Number of people expected to attend: 120
Length of session : 2 hours
Conflicts (whole Areas and/or WGs)
Chair Conflicts: TBD
MUST avoid: QUIC, TSVWG, CCWG, NFSv4, v6ops and maprg
Technology Overlap: WIT Area, INT Area, OPS Area
Key Participant Conflict: Daniel Huang, Kehan Yao, Quan Xiong, Daniel King, Tim Chown
Scheduling: given expected remote participation from North America and Asia, prefer early afternoon session
Information for IAB/IESG
To allow evaluation of your proposal, please include the following items:
- There are intensive discussions in the hp-wan mailing list with significant interests from various vendors as well as operators and research & education institutions across Asia, Europe and North America. Rough consensus about use cases, problems and requirements is starting to emerge in the hp-wan community. The BoF aims to focus the discussion towards specific actions.
- Any protocols or practices that already exist in this space: Congestion control algorithms like BBR/CUBIC etc, RDMA/iWARP/RoCEv2 related issues
- Which (if any) modifications to existing protocols or practices are required: None identified so far - this is a purpose of the BoF
- Which (if any) entirely new protocols or practices are required: To be identified with the ongoing discussions.
- Open source projects (if any) implementing this work: None identified so far

Agenda
Chair introduction
Private HP-WAN state of the art implementation (2-3 presentations)
Public HP-WAN use cases, problems and requirements (1-2 presentations)
Gap analysis of the existing technologies
Open discussions
Polls (about use cases, problems, requirements and scope)
Links to the mailing list, draft charter if any, relevant Internet-Drafts, etc.
hp-wan mailing List: https://mailarchive.ietf.org/arch/browse/hp-wan/
State of the art hp-wan implementations and deployments: https://datatracker.ietf.org/doc/draft-kcrh-state-of-art-hp-wan/
Use cases, problems and requirements: https://datatracker.ietf.org/doc/draft-xiong-uc-problem-req-hp-wan/
