# Week 02 — Threats, Vulnerabilities & SecureScholar Coding

**Date Range:** Nov 3 – Nov 8, 2025  
**Total Hours:** 10.5 hrs  
**Phase:** Google Cybersecurity Certificate (Course 1 Complete) + SecureScholar Module 2

---

## Google Cybersecurity Certificate Progress

### 2025-11-03 — Module 3: Protect Against Threats, Risks & Vulnerabilities

**Status:** ✅ Completed

**Key Concepts:**

* **Threats, risks, and vulnerabilities** are interrelated. Threats exploit vulnerabilities to cause harm; risk measures likelihood × impact.
* **Threat actors** include cybercriminals, hacktivists, insiders, and nation-states, each with distinct motives.
* **Vulnerability vs. Exploit:** A flaw vs. the technique used to take advantage of it.
* **Risk formula:** `Risk = Likelihood × Impact` to prioritize mitigation.
* **Defensive measures:** Patch management, least privilege, firewalls, IDS/IPS, and security training.
* **Incident Lifecycle:** Identify → Contain → Eradicate → Recover → Lessons Learned.

**Evidence:**
* `Screenshots/2025-11-03_Module3_Completed.png` — Coursera completion screen for Module 3.

**Reflection:**  
Module 3 connected abstract security concepts to concrete frameworks. Understanding the risk formula helped me prioritize which vulnerabilities matter most—a skill that translates directly to SecureScholar's phishing defense content.

---

### 2025-11-04 — Module 4: Cybersecurity Tools & Local Practice

**Status:** ✅ 50% Completed (tool practice)

**Commands Tested:**

```bash
nmap -sn 127.0.0.1      # Ping scan of localhost
whoami                   # Display current user
grep "root" /etc/passwd  # Search for root user entry
```

**Purpose:**

| Command | Function | Result |
|---------|----------|--------|
| `nmap -sn 127.0.0.1` | Scans local host to verify network response | Host is up (127.0.0.1) |
| `whoami` | Displays current user context | labuser |
| `grep "root" /etc/passwd` | Finds root entries in system file | `root:x:0:0:root:/root:/usr/bin/zsh` |

**Environment:** Isolated Kali VM using Host-Only networking (no external targets)

**Evidence:**
* `Screenshots/2025-11-04_Tool_Commands_Tested.png` — Terminal showing command outputs

**Reflection:**  
This mini-lab reinforced core command-line skills and how they connect to vulnerability analysis. Testing tools locally helped validate system visibility and privilege checks in a controlled environment.

**Safety Note:** All commands run in isolated VirtualBox environment scanning localhost only. No external targets accessed.

---

### 2025-11-05 — Course 1 Completion: Foundations of Cybersecurity

**Status:** ✅ Completed

**Summary:**  
Completed all modules, hands-on exercises, and the final quiz for Course 1. Earned the Coursera certificate and recorded completion for portfolio integration.

**Evidence:**
* `Screenshots/2025-11-05_Module4_Completed.png` — Certificate of completion

**Reflection:**  
Course 1 built a solid foundation in both theory and practical skills—from risk assessment to command-line execution. It connected the CIA Triad to hands-on operations, laying the groundwork for risk management in Course 2 and for SecureScholar's teaching modules.

---

### 2025-11-07 — Vulnerability Scan Lab (Docker + Nmap on OWASP Juice Shop)

**Status:** ✅ Completed

**Overview:**  
Configured Docker in Kali, launched the OWASP Juice Shop container, and performed a series of Nmap scans to simulate vulnerability enumeration on a local web application.

**Steps Taken:**

1. Verified Docker service installation and startup
2. Ran Juice Shop container:
   ```bash
   docker run -d -p 3000:3000 bkimminich/juice-shop
   ```
3. Confirmed application availability at `http://127.0.0.1:3000`
4. Checked network reachability:
   ```bash
   ping -c 4 127.0.0.1
   ```
5. Validated open port (3000/tcp):
   ```bash
   sudo ss -tuln | grep 3000
   ```
6. Conducted Nmap scans to identify services and headers:
   ```bash
   sudo nmap -p 3000 -sS -sV 127.0.0.1
   sudo nmap -p 3000 --script http-enum,http-headers,http-server-header 127.0.0.1
   sudo nmap -p 3000 --script vuln 127.0.0.1
   ```

**Key Findings:**
* Port 3000/tcp open (Node.js Express server)
* HTTP headers revealed server version and framework
* No critical vulnerabilities detected (expected for patched container)

**Evidence:**
* `Screenshots/2025-11-07_Docker_Install_Success.png`
* `Screenshots/2025-11-07_JuiceShop_App_Up.png`
* `Screenshots/2025-11-07_Ping_OK.png`
* `Screenshots/2025-11-07_nmap_sV_output.png`
* `Screenshots/2025-11-07_nmap_http_output.png`

**Reflection:**  
This lab demonstrated practical network reconnaissance and vulnerability scanning techniques. By testing a local containerized application, I safely observed how services respond to probes and how Nmap scripts identify metadata such as headers and server types. It reinforced ethical testing principles and the importance of working within isolated environments.

---

## SecureScholar Module 2 Development

### 2025-11-05 — Module 2 HTML Skeleton

**Status:** ✅ Completed

**What I Built:**  
Created the structural foundation for Module 2 (Phishing Defense) with:
* 2-lesson layout (expandable to 4)
* Prev/Next navigation buttons
* Keyboard shortcuts (arrow keys)
* Quiz placeholder button
* Progress footer with autosave timestamp
* localStorage integration

**Files Created:**
* `src/modules/module2.html` (~150 lines)

**Technical Implementation:**
* Embedded CSS (no external dependencies)
* Vanilla JavaScript for navigation
* Modular lesson sections (easy to add/remove)
* Responsive design matching Module 1 aesthetic

**Evidence:**
* `Screenshots/2025-11-05_Module2_HTML_Skeleton.png`

**Commit:**
* `feat: create Module 2 HTML structure with navigation`

---

### 2025-11-08 — Lesson 1: What is Phishing?

**Status:** ✅ Completed

**Content Details:**
* **Main lesson:** 250 words covering phishing definition, real-world examples, psychology, and statistics
* **Aarav's Note:** 169 words sharing personal near-miss phishing experience
* **Statistics cited:** Verizon DBIR 2024 (36% of breaches involve phishing)
* **Examples used:** Netflix scam, package delivery text, school IT phishing

**Writing Process:**
* Researched Verizon DBIR and FBI IC3 reports
* Drafted 3 versions to find right tone (peer-to-peer, not academic)
* Integrated authentic personal story for relatability
* Used accessible language for high school audience

**Key Learning:**  
Writing for peers requires different tone than writing for instructors. Had to translate cert concepts into relatable scenarios. The "teach to learn" effect was real—explaining phishing forced deeper understanding than just studying it.

**Evidence:**
* `Screenshots/2025-11-08_Module2_Lesson1_Live.png`

**Commits:**
* `feat: add Lesson 1 content - What is Phishing (Module 2)`

---

### 2025-11-08 — Module 2 Quiz Navigator

**Status:** ✅ Completed

**Overview:**  
Built interactive JavaScript quiz system for Module 2 (Phishing Defense). Created question navigation loop with visual feedback and state management.

**Files Created:**
```
src/js/module2-quiz.js          # Quiz logic (80 lines)
src/modules/module2-quiz.html   # Quiz UI (120 lines)
```

**Features Implemented:**
* Question array with 3 phishing defense questions
* State tracking: `currentQuestionIndex`
* Dynamic DOM rendering for each question
* Visual feedback: selected answers highlight blue
* "Next Question" button advances through quiz
* Completion message after final question
* No scoring yet (Week 3 feature)

**Technical Details:**

```javascript
// Core navigation function
function nextQuestion() {
  if (currentQuestionIndex < module2Questions.length - 1) {
    currentQuestionIndex++;
    nextButton.disabled = true;
    renderQuestion();
  } else {
    finishQuiz();
  }
}

// Dynamic question rendering
function renderQuestion() {
  const q = module2Questions[currentQuestionIndex];
  questionContainer.textContent = q.text;
  
  optionsContainer.innerHTML = '';
  q.options.forEach((option, index) => {
    const button = document.createElement('button');
    button.className = 'quiz-option';
    button.textContent = option;
    button.onclick = () => selectOption(index);
    optionsContainer.appendChild(button);
  });
  
  questionCounter.textContent = `Question ${currentQuestionIndex + 1} of ${module2Questions.length}`;
}
```

**Debugging Notes:**  
Quiz button in `module2.html` initially showed alert popups. Fixed by replacing conditional logic with direct navigation:

```javascript
quizBtn.addEventListener('click', () => {
  window.location.href = 'module2-quiz.html';
});
```

Required hard browser refresh (Ctrl+Shift+R) to clear cached JavaScript.

**Evidence:**
* `Screenshots/2025-11-08_Quiz_Navigator_Working.png` — Quiz page showing question cycle

**Commits:**
* `feat: add Module 2 quiz navigator (JavaScript question loop)`
* `doc: add quiz navigator screenshot`

**Reflection:**  
This quiz navigator establishes the foundation for Week 3's scoring system. Building without a framework (vanilla JS) forced me to understand state management fundamentals. The code is simple but functional—exactly what a portfolio needs to demonstrate core skills.

---

## Week 2 Summary

### Accomplishments

**Google Certification:**
* ✅ Completed Course 1: Foundations of Cybersecurity
* ✅ Finished Modules 3-4 (Threats, Tools, Programming)
* ✅ Earned Course 1 certificate

**Hands-On Labs:**
* ✅ Kali VM tool practice (nmap, whoami, grep)
* ✅ Docker + OWASP Juice Shop vulnerability scan
* ✅ Multiple Nmap reconnaissance techniques

**SecureScholar Development:**
* ✅ Module 2 HTML skeleton built
* ✅ Lesson 1 written and integrated (250 words + personal note)
* ✅ Quiz navigator coded and functional (200 lines total)

### Progress Metrics

| Metric | Week 2 | Total |
|--------|--------|-------|
| Hours | 10.5 | 18.5 |
| Commits | 7 | 24+ |
| Lessons | +1 | 5 |
| Code Files | +3 | 14 |
| Screenshots | 8 | 15+ |

### Key Takeaways

1. **Completed entire Course 1** ahead of schedule—momentum building
2. **Vulnerability scanning** translated theory into practice
3. **Content writing** took 3x longer than expected but quality shows
4. **Quiz foundation** proves vanilla JS competency
5. **Sustainable pace** maintained (avg 1.5 hrs/day)

### Challenges Overcome

**Challenge 1:** Docker networking in VirtualBox required troubleshooting  
**Solution:** Adjusted NAT + Host-Only adapters, documented configuration

**Challenge 2:** Module 2 felt empty with just HTML skeleton  
**Solution:** Patience paid off—Lesson 1 completion made it feel legitimate

**Challenge 3:** Quiz button showed old alert code after changes  
**Solution:** Learned about browser caching, now use hard refresh + incognito testing

---

## Next Week Preview (Week 3)

**Priorities:**
* Begin Course 2: Play It Safe - Manage Security Risks
* Write Lesson 2: Types of Phishing (email, spear, smishing, vishing)
* Add basic scoring system to quiz navigator
* Update homepage to link Module 2

**Time Budget:** 6 hours max (maintenance mode until Course 2 underway)

**Success Criteria:**
* Lesson 2 matches Lesson 1 quality
* Quiz scoring works correctly
* Module 2 accessible from homepage

---

## Professional Statement (Updated Nov 8, 2025)

> My name is **Aarav Arora**, a high school student committed to cybersecurity education and digital safety. Through the Google Cybersecurity Certificate and hands-on labs, I am building a foundation in network security, Linux administration, and threat analysis.
>
> I value integrity, persistence, and precision in problem-solving. I see cybersecurity as both technical expertise and ethical responsibility—defending systems while building awareness that helps others stay safe online.
>
> Through SecureScholar, I'm translating what I learn into accessible education for peers. My goal is to make cybersecurity knowledge available to students who might not otherwise encounter it, bridging the gap between technical skills and community impact.

---

**Status:** Week 2 Complete ✅  
**Momentum:** 🟢 Green — Course 1 finished, Module 2 foundation shipped, sustainable pace maintained

*Last updated: November 8, 2025*
