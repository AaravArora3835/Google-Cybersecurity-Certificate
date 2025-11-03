## Week 1: Oct 27 - Nov 2, 2025

### What I Built/Learned

**Course Progress:**
- Completed Google Cybersecurity Course 1, Modules 1-2 (100%)
- Started Module 3: Protect Against Threats (~40%)
- Overall course progress: ~20%

**Key Technical Concepts Mastered:**
- **CIA Triad:** Confidentiality, Integrity, Availability as the foundation of all security controls
- **Cybersecurity Evolution:** How threats evolved from Morris Worm (1988) to modern ransomware and APT attacks
- **Risk Management Framework:** Risk = Likelihood × Impact; prioritize mitigation based on business context
- **Defense in Depth:** Layered security using multiple controls at different levels
- **Threat Landscape:** Attack surfaces, zero-day vulnerabilities, and threat actor motivations

**Major Parallel Project - Ubuntu Dual-Boot:**
- Successfully installed Ubuntu 24.04 LTS alongside macOS on 2019 MacBook Pro (T2 chip)
- Configured firmware-level security (Secure Boot, SIP, EFI partitions, rEFInd bootloader)
- Troubleshot Apple T2 hardware compatibility (Broadcom Wi-Fi, internal keyboard/trackpad drivers)
- Created comprehensive 50-file public documentation repository with installation guide, troubleshooting docs, and security analysis
- Total Ubuntu project: 7 hours across 3 days (Oct 30-Nov 2)

**SecureScholar Platform Development:**
- Designed Module 2 (Phishing Defense) curriculum with 4-lesson structure
- Wrote Lesson 1 complete draft (248 words + 169-word personal Aarav's Note)
- Established 8-week writing schedule aligned with certification study
- Total SecureScholar: 3 hours

---

### What Was Hard

**Challenge 1: Time management during intense launch week**

Balancing 18 hours of roadmap work with school, homework, and life was significantly harder than planned. The original 5 hrs/week estimate didn't account for the complexity of parallel projects.

**What made it hard:** Weeknight 1-hour study blocks weren't enough for deep focus. Context-switching between Coursera videos, Ubuntu troubleshooting, and SecureScholar writing fragmented my attention.

**Solution moving forward:** Week 2 will return to 7.5 hrs/week maximum. Shifting to longer 1.5-2 hour blocks fewer days per week instead of daily 1-hour sessions. Protecting Saturday 9-11 AM as primary deep work window.

**Challenge 2: Apple T2 chip firmware complexity**

Understanding the relationship between Secure Boot, System Integrity Protection (SIP), EFI partitions, rEFInd, and GRUB required reading multiple technical docs from Apple, T2 Linux community, and Ubuntu forums. The security architecture is deliberately restrictive.

**What made it hard:** Apple's official docs don't explain how to *bypass* T2 protections - they're designed to prevent exactly what I was trying to do. Community documentation was fragmented across Reddit, GitHub issues, and wiki pages.

**What I learned:** This forced me to understand *why* each security layer exists before deciding to disable it. Module 2's risk management framework became immediately applicable - I documented likelihood, impact, and compensating controls for each firmware modification.

**Challenge 3: Making SecureScholar content authentic**

Writing "Aarav's Notes" that feel genuine and educational (not forced or fake) is harder than technical content. First drafts sounded like I was trying too hard to be relatable.

**Solution:** Wrote from actual experiences (almost clicking school phishing email, setting up password manager after friend's account was compromised). Authenticity > perfection. Rewrote Aarav's Note 3 times until it sounded like how I actually talk.

---

### What I'm Proud Of

**1. Shipped a production-ready Ubuntu dual-boot environment in 3 days**

Turned troubleshooting notes and firmware configs into a complete, professional repository with:
- 50+ documented files across 4 directories
- 27 timestamped screenshots proving every step
- Complete installation guide (Guide.md) that others can follow
- Troubleshooting documentation for 6 common T2 Mac issues
- Security analysis connecting firmware decisions to CIA Triad and defense in depth

This is portfolio-ready work demonstrating system administration, hardware security, and professional documentation standards.

**2. Connected theory to practice across all three tracks**

- **Coursera → Ubuntu:** Module 2's risk management framework directly informed my Secure Boot disable decision. I didn't just disable it blindly - I documented risk = likelihood × impact, accepted the tradeoff, and implemented compensating controls (firmware password, physical security, disk encryption).

- **Ubuntu → SecureScholar:** The "hover over links before clicking" habit from Phishing Lesson 1 is the same verification mindset I used checking firmware download checksums (SHA-256 validation). Teaching forces deeper understanding.

- **Coursera → SecureScholar:** CIA Triad concepts from Module 1 will inform how I explain password security (Confidentiality), 2FA (Availability + Integrity), and phishing defense (all three pillars).

This is exactly why I built the roadmap with parallel tracks - theory, practice, and teaching reinforce each other instead of competing.

**3. Maintained quality under time pressure**

Even though Week 1 was 2x the planned hours (18 vs 9), I didn't cut corners:
- Every repo follows v4.9 standards (proper file naming, commit prefixes, folder structure)
- Every screenshot properly timestamped and referenced
- Every reflection written honestly with specific details
- All documentation complete before moving to next task

**4. Proved I can execute a complex technical project independently**

The Ubuntu installation required:
- Reading firmware documentation and community wikis
- Troubleshooting hardware compatibility issues without step-by-step guides
- Making informed security tradeoffs with documentation
- Testing, verifying, and documenting every change

No one told me exactly what to do. I researched, tested, failed, debugged, and succeeded. That's the definition of real technical work.

---

### Connections Across Projects

**Google Cert ↔ Ubuntu (Risk Management):**
- Module 2 taught: Risk = Likelihood × Impact, with mitigation strategies
- Ubuntu applied it: Disabling Secure Boot = Low likelihood (physical access required) × Medium impact (bootkit possible) = Acceptable risk with compensating controls

**Google Cert ↔ Ubuntu (Defense in Depth):**
- Module 2 taught: Multiple security layers protect better than one strong control
- Ubuntu applied it: Even with Secure Boot disabled, I maintain: firmware password + disk encryption + physical device security + documented audit trail = defense in depth

**Ubuntu ↔ SecureScholar (Verification Mindset):**
- Ubuntu: Verified ISO checksums (SHA-256) before trusting downloaded files
- SecureScholar Lesson 1: "Hover over links to verify URLs before clicking"
- Same principle: Don't trust, verify. Applicable to firmware downloads AND phishing emails.

**Google Cert ↔ SecureScholar (Teaching = Deeper Learning):**
- CIA Triad is abstract when you just memorize it
- Writing Lesson 1's Aarav's Note forced me to explain *why* the phishing email almost fooled me (urgency + authority + stress)
- Teaching psychology of attacks > just listing attack types

This is proof that parallel tracks work. Each project makes the others stronger.

---

### Next Week Preview

**Course Goals (Week 2: Nov 3-9):**
- Complete Module 3: Protect Against Threats
- Start Module 4: Tools of the Trade - Linux and SQL
- Use Ubuntu dual-boot for any Linux CLI labs
- Target: 5 hours Coursera (sustainable pace)

**SecureScholar Goals:**
- Write Module 2 Lesson 2 draft: "Types of Phishing" (250 words)
- Write Lesson 2 Aarav's Note (50-100 words)
- Target: 2.5 hours (Wednesday evening + Saturday morning)

**Ubuntu:**
- No new development (project complete)
- Use for Coursera labs starting Module 4
- Monitor boot stability and driver performance

**Schedule Adjustments Based on Week 1 Learnings:**
- **Monday Nov 3:** Rest day (no study) - recover from intense Week 1
- **Tue-Thu:** 7:00-8:30 PM blocks (1.5 hrs each) instead of 4-5 PM 1-hour blocks
- **Saturday:** 9-11 AM deep work for SecureScholar writing
- **Sunday:** 2-3 PM reflection + Week 3 planning

**Week 1 was 18 hours. Week 2 targeting 7.5 hours. This is the sustainable pace test.**

---

### Time Breakdown

| Activity | Planned (hrs) | Actual (hrs) | Delta |
|----------|---------------|--------------|-------|
| Coursera Modules 1-2 | 5 | 6 | +1 |
| Ubuntu dual-boot project | 0* | 7 | +7 |
| SecureScholar Lesson 1 | 2.5 | 3 | +0.5 |
| Reflection/documentation | 1 | 2 | +1 |
| **Total** | **8.5** | **18** | **+9.5** |

*Ubuntu wasn't originally scheduled for Week 1 but was integrated because the native Linux environment is essential for upcoming Coursera labs (Module 4: Linux CLI and SQL).

**Key insight:** Week 1 pace (18 hrs) is not sustainable during school term. Week 2 must return to 7.5 hrs max to test long-term viability.

---

### Honest Assessment

**What's working really well:**
- Weekend morning deep work blocks (Saturday 9-11 AM, Sunday 9-12 PM) = highest productivity
- Taking screenshots immediately during work (not retroactively) = better evidence
- Writing reflections weekly (not monthly) = captures real learning while fresh
- Cross-linking projects strengthens both (Ubuntu docs reference Coursera concepts; Coursera notes reference Ubuntu experience)
- v4.9 documentation standards keep all repos professional and consistent

**What needs adjustment for Week 2:**
- Weeknight 1-hour blocks too short for quality work → extend to 1.5 hrs OR skip some nights entirely
- Week 1 intensity (18 hrs) cannot repeat every week → strict 7.5 hr limit Week 2
- Need to actively protect Saturday mornings from social plans - that's best productivity window
- Consider batch-watching Coursera videos (2-3 at once) instead of one per night

**What I'm uncertain about:**
- Can I maintain 2.5 hrs/week on SecureScholar + 5 hrs Coursera during midterms? (Will test Week 2-4)
- Is the Ubuntu environment stable enough for daily use or will kernel updates break drivers?
- Will User Validation Gate 1 (Week 10) actually get 10 testers or do I need to start recruiting earlier?

**Energy/motivation level:** 8/10
- High because launch momentum + seeing real tangible progress (working dual-boot, published repos, learning concepts)
- Slight fatigue from 18-hour week
- Concern about sustainability when school gets busier (midterms, project deadlines)

**Confidence in Week 2 plan:** 7/10
- Schedule adjustments (longer blocks, rest Monday, protect Saturday) should help
- Returning to 7.5 hrs feels more realistic
- Will reassess sustainability after Week 2 to see if pace is truly manageable

---

### Screenshot Evidence

**Google Cybersecurity Progress:**
- `2025-10-29_Module1_Complete.png` - Module 1 quiz passed
- `2025-10-31_Module2_Started.png` - Module 2 begun
- `2025-10-31_Module2_Completed.png` - Module 2 finished
- `2025-11-02_Module3_Progress.png` - Module 3 in progress

**Ubuntu Dual-Boot Project:**
- 27 screenshots across installation process (see Ubuntu-DualBoot-MacT2 repo)
- Complete repository: [github.com/AaravArora3835/Ubuntu-DualBoot-MacT2](https://github.com/AaravArora3835/Ubuntu-DualBoot-MacT2)

**SecureScholar Platform:**
- Module 2 Plan + Lesson 1 complete in SecureScholar repo
- [github.com/AaravArora3835/SecureScholar-Platform](https://github.com/AaravArora3835/SecureScholar-Platform)

---

**Week 1 Status:** ✅ COMPLETE  
**Course Progress:** 20% (2.5/8 modules)  
**Projects Shipped:** 1 major (Ubuntu guide)  
**Content Written:** ~3,000 words (reflections + SecureScholar)  
**Ready for Week 2:** Yes, with adjusted sustainable schedule  

---

**Biggest takeaway from Week 1:** Execution beats planning. I spent October planning this roadmap. Week 1 proved I can actually execute it. The hardest part of any long-term project is starting - and I've started strong.

**Week 2 mission:** Prove sustainability. Can I maintain quality work at 7.5 hrs/week during school? That's the real test.
