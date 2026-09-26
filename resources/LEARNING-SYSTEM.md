# The learning system I will actually follow

_Last reviewed: 2026-09-26_

This is the part of the roadmap where I stop collecting links and decide what I am actually going to study.

I am writing this as public documentation because somebody else may find the same problem: there are thousands of “best courses”, but no clear answer to **which one comes first, what it covers, what it does not cover, and when I am allowed to move on**.

The percentages below are **planning estimates, not scientific measurements**. They describe how much of the target in this repo a resource should cover when I finish the lessons, do the exercises, build the project, and pass the gate. Watching videos alone counts for almost nothing.

> My rule: **one main course + a small mastery layer + official documentation + one serious project + one gate.**

## The honest 8x/9x answer

No online course covers 90% of becoming a real engineer. A course can cover a large part of the **knowledge map**; it cannot give me years of production incidents, teamwork, university assessment, interviews, or judgment.

For the technical path in this repo:

- **CS50x + Missing Semester** should cover roughly **80–85% of the foundation stage**: programming thinking, C/Python basics, algorithms, data structures, SQL, web basics, command line, Git and developer tools.
- **Full Stack Open + the project gates** should cover roughly **80–90% of the practical web/backend stage**: React, Node, APIs, testing, TypeScript, relational databases, containers and CI/CD.
- **AWS free learning + Terraform/Docker/GitHub Actions/Kubernetes/OWASP/observability docs** should cover roughly **75–85% of the junior cloud/DevOps knowledge target** when I practise locally and document failures.
- The **whole engineering journey** still leaves a large part for university, internships, production work, system design, security depth and communication. That is the missing 10–20% (and sometimes much more) I cannot honestly pretend a course can replace.

The “rest” is not another giant playlist. It is:

1. building without a tutorial,
2. breaking and repairing the system,
3. explaining trade-offs,
4. receiving human review,
5. working with other people,
6. repeating the work until it becomes reliable.

---

# 1. Main technical path: computer science → software engineering

## My free main path

### Main course 1 — [CS50x: Introduction to Computer Science](https://cs50.harvard.edu/x/)

**Level:** beginner to early intermediate foundation.

**What it teaches:** computational thinking, C, memory, algorithms, data structures, Python, SQL, HTML/CSS/JavaScript, Flask and a final project. Harvard explicitly makes the OpenCourseWare version available to take for free; a verified certificate or academic credit is a different, potentially paid route.

**Expected coverage for this repo:** about **50–60% of the computer-foundation stage**, not the whole career.

**Why I choose it:** it is coherent, demanding, and it teaches me how to think instead of only teaching framework syntax.

**Why it does not finish the job:** it is not a Linux administration course, cloud course, Japanese-workplace course, or production SRE apprenticeship. I still need to do the problem sets and final project.

### Main course 2 — [MIT The Missing Semester](https://missing.csail.mit.edu/)

**Level:** beginner who has started coding; early university tooling.

**What it teaches:** shell, command line, Git, debugging, editors, automation and the tools that formal classes often skip.

**Expected coverage:** about **20–25% of the foundation stage**, mainly tools and workflow.

**Why I choose it:** it turns “I can write code” into “I can work in a real repository and diagnose my own environment”.

**Why it does not finish the job:** it is not a substitute for operating-systems, networking, algorithms or a backend project.

### The first gate

I do not move into cloud or Kubernetes until I can:

- write a small Python CLI without copying a tutorial,
- use Linux shell, files, permissions, processes and logs,
- use Git branches and recover from a normal mistake,
- explain arrays, hash tables, recursion, SQL joins and HTTP,
- build and document one small project,
- debug it after intentionally breaking it.

## The practical mastery course — [Full Stack Open](https://fullstackopen.com/en/)

**Level:** intermediate; not my first programming course.

**What it teaches:** modern web development with React, Node/Express, REST APIs, testing, user administration, GraphQL, TypeScript, React Native, CI/CD, containers, relational databases and Next.js.

**Expected coverage:** about **80–90% of the practical web/backend target** in this roadmap, if I complete the exercises and build my own version rather than clone the examples.

**Project gate:** a documented service with a frontend, API, authentication, PostgreSQL, tests, Docker Compose, CI, logs and a deployment diagram.

**Why choose it:** it is a university-backed, openly available sequence with unusually good breadth and practical work.

**Why not choose it as my first course:** it is JavaScript-heavy, moves quickly, and does not replace CS fundamentals, Linux, networking, cloud architecture or deep Python backend work.

## Official references I will use only when the project needs them

- [Python tutorial](https://docs.python.org/3/tutorial/) — language and standard library reference.
- [MDN Learn Web Development](https://developer.mozilla.org/en-US/docs/Learn_web_development) — browser, HTML, CSS, JavaScript and HTTP-facing web fundamentals.
- [PostgreSQL tutorial](https://www.postgresql.org/docs/current/tutorial.html) — SQL, schema, constraints, transactions and indexes.
- [FastAPI documentation](https://fastapi.tiangolo.com/) — optional Python API implementation after the foundation gate.
- [Docker Get Started](https://docs.docker.com/get-started/) — images, containers, volumes, networks and Compose.

These are not five new courses. They are the manuals I open while building.

## Paid second path: [Boot.dev Backend Path](https://www.boot.dev/paths/backend)

**What I would be paying for:** a more guided, interactive path with frequent coding exercises and backend subjects such as Python, SQL, APIs, databases and Go.

**Why choose it:** if I repeatedly stop studying alone, the short feedback loop, visible progress and structured path may be worth paying for. It is a good alternative to assembling many small courses.

**Why not choose it:** it is not a university degree, not a replacement for CS50x or a European Bachelor's, and its marketing claims are not proof that I will get a job. I would still need my own projects, Linux depth, networking, cloud and human feedback.

**My decision:** free path first. I only pay when lack of structure is the bottleneck, not because I am bored with the current course.

---

# 2. Cloud, DevOps, security and reliability

This is deliberately a **second layer**. I do not start here before Linux, Git, Python, networking, SQL, HTTP and Docker are usable.

## Free main path

1. [AWS Skill Builder free learning](https://aws.amazon.com/training/digital/) — AWS says it offers 1,000+ free learning resources; the paid subscription unlocks additional labs and digital classrooms. I use the free Cloud Practitioner/cloud fundamentals material first.
2. [Terraform tutorials](https://developer.hashicorp.com/terraform/tutorials) — providers, resources, variables, state, modules and plan/apply/destroy. Start with Docker or local practice before paying for cloud.
3. [GitHub Actions documentation](https://docs.github.com/en/actions) — tests, builds, artifacts, secrets and deployment workflows.
4. [Introduction to Kubernetes (LFS158)](https://training.linuxfoundation.org/training/introduction-to-kubernetes/) — free introductory Kubernetes course; I run the exercises locally with kind or Minikube.

**Expected coverage:** approximately **75–85% of the junior cloud/DevOps knowledge target** in this repo. That estimate assumes I actually deploy locally, inspect logs, destroy infrastructure, restore it, and write a postmortem.

## Small mastery layer

- [OWASP Top 10](https://owasp.org/www-project-top-ten/) and [Web Security Testing Guide](https://owasp.org/projects/web-security-testing-guide/) — application-security thinking and authorised testing only.
- [Prometheus](https://prometheus.io/docs/introduction/overview/) + [OpenTelemetry](https://opentelemetry.io/docs/) — metrics, traces, instrumentation and SLO thinking.
- [Kubernetes documentation](https://kubernetes.io/docs/home/) — the reference after the introductory course.
- [System Design Primer](https://github.com/donnemartin/system-design-primer) — trade-offs and interview practice, not a replacement for distributed-systems study.

## Cloud/DevOps project gate

I build one service and make it boringly operational:

- containerise it,
- run it with Compose,
- add tests and CI,
- provision a small environment with Terraform,
- add logs and metrics,
- add a health check and rollback path,
- threat-model it with OWASP,
- break DNS, credentials, a container and a deployment,
- repair each failure and write the incident notes.

## Paid second path: [KodeKloud](https://kodekloud.com/)

**Why choose it:** the platform is strong when I need browser-based labs and repeated hands-on practice for Linux, Docker, Kubernetes, AWS and CI/CD. It also currently advertises free 100 Days of DevOps and 100 Days of Cloud challenges, so I can test the teaching style before paying.

**Why not choose it:** a lab can make me good at following a lab. It cannot create production judgment by itself, and the subscription/feature boundaries can change. I should not pay for it before I have a service to operate.

**Alternative paid purchase:** if my employer or degree is specifically AWS-focused, I can buy only the relevant official exam preparation or lab access rather than a broad subscription.

---

# 3. English: every skill, but one system instead of a dump

English supports university, IELTS, documentation, interviews, teamwork and Japan. I keep my existing IELTS coaching as the structured exam track and use the free system below around it.

## Free core — [British Council LearnEnglish](https://learnenglish.britishcouncil.org/free-resources)

This is the main hub. It has levelled practice for listening, reading, writing, speaking, grammar and vocabulary, plus business English and email material.

| Skill | What I use | Weekly output |
|---|---|---|
| Listening | [Levelled listening](https://learnenglish.britishcouncil.org/free-resources/listening) and BBC Learning English | Listen once for meaning, again with notes, then summarise aloud. |
| Reading | [Levelled reading](https://learnenglish.britishcouncil.org/free-resources/reading) and technical documentation | One short article; write five useful phrases in context. |
| Writing | [Writing practice](https://learnenglish.britishcouncil.org/free-resources/writing) and [English for emails](https://learnenglish.britishcouncil.org/free-resources/business/english-emails) | One 200–500 word explanation, revised once. |
| Speaking | [Speaking practice](https://learnenglish.britishcouncil.org/free-resources/speaking) | Record a 5–10 minute explanation of my current technical project. |
| Pronunciation | [BBC pronunciation](https://www.bbc.co.uk/learningenglish/english/features/pronunciation) and British Council audio | Shadow a short clip; focus on stress and clarity, not copying an accent. |
| Grammar | [British Council grammar](https://learnenglish.britishcouncil.org/free-resources/grammar) | Fix mistakes found in my own writing. |
| Word meaning/verbs | [British Council vocabulary](https://learnenglish.britishcouncil.org/free-resources/vocabulary), Cambridge Dictionary and example sentences | Learn words through phrases and verbs, not isolated translations. |

**Expected coverage:** roughly **80–90% of my everyday English practice needs** and a strong IELTS supplement. It does **not** guarantee an IELTS band, and free websites cannot give me continuous personalised speaking and writing correction.

**Extra course, only when needed:** [Cambridge English free learner activities](https://www.cambridgeenglish.org/learning-english/activities-for-learners/) for additional reading, listening, grammar and vocabulary practice.

## The English gate

I am improving when I can read a technical page, explain it without translating every sentence, write a clear issue/README/email, speak for ten minutes about a project, and revise my own errors. A test score is useful evidence, not the whole skill.

## Paid second path: [British Council IELTS Coach](https://learnenglish.britishcouncil.org/ielts-preparation/ielts-coach)

**Why choose it:** it is the official test organisation's paid coaching option, with expert teachers, needs analysis, mock tests, group/private class credits and practice across the four IELTS skills.

**Why not choose it:** it is IELTS preparation, not a full lifelong English curriculum; it may be wasteful if my only weakness is vocabulary or if my current coaching already supplies feedback. Prices and packages vary by country and time.

**My decision:** use free practice daily; pay only when I need a real teacher to diagnose speaking/writing and the exam date justifies it.

---

# 4. Japanese: Bengali bridge → practical Japanese → workplace Japanese

Japanese is a long-term support track. It must not damage the foundation stage, but it cannot remain a vague “I will learn later” promise either.

## Free main path A — [NHK Easy Japanese in Bengali](https://www3.nhk.or.jp/nhkworld/lesson/bengali/)

**Level:** complete beginner.

NHK's Bengali page provides conversation and grammar lessons, downloadable learning materials, and a 48-week beginner programme designed to teach basic phrases and conversation. This is the best Bengali-language on-ramp I found for the first stage.

**Expected coverage:** around **25–35% of the beginner stage**. It gives me a start, not N3/N2.

## Free main path B — [Irodori](https://www.irodori.jpf.go.jp/en/) + [Irodori Online](https://www.irodori-online.jpf.go.jp/)

**Level:** beginner through practical daily-life Japanese, with a path beyond the first stage.

**What it teaches:** practical language needed for life in Japan, with audio, video, illustrations and situation-based practice.

**Expected coverage:** roughly **50–65% of practical beginner/intermediate daily-life Japanese**, depending on how far I go and whether I practise speaking.

**Why choose it:** it is made by the Japan Foundation and is more useful for my Japan goal than learning random anime phrases.

**Why it does not finish the job:** it is not full workplace fluency, does not guarantee JLPT success, and does not replace live speaking/writing correction.

## Small Japanese mastery layer

- [Tae Kim's Guide](https://guidetojapanese.org/learn/) — free grammar explanation when I need a second explanation.
- [Tadoku free books](https://tadoku.org/japanese/en/free-books-en/) — graded reading; read aloud and retell.
- [Comprehensible Japanese](https://www.youtube.com/@cijapanese) — understandable listening with visual support.
- [Anki](https://apps.ankiweb.net/) — spaced repetition; I add sentences from what I read, not a thousand random words.
- After I can read native material: [Yomitan](https://yomitan.wiki/) for dictionary lookups while reading.

**Expected combined coverage:** about **70–80% of the N5–N3 learning target** with consistent practice, but only around **40–60% of actual communication** because speaking, writing and workplace interaction require people.

## Japanese gate by level

- **Kana/basic:** read and type hiragana and katakana; understand basic sentence order.
- **N5/N4 range:** handle introductions, daily routines, shopping, transport and simple messages.
- **N3 range:** follow graded/native-ish everyday content, explain familiar topics and write short practical messages.
- **N2/work preparation:** read job-related material, write polite emails, follow meetings with support, and practise keigo and technical vocabulary.

JLPT is useful evidence, but JLPT does not test speaking and writing as a complete workplace ability. I track both the certificate and the real tasks.

## Paid second path: [Coto Academy Online](https://cotoacademy.com/online-japanese-lessons/)

**Why choose it:** live native-teacher classes, structured courses from beginner to advanced, conversation practice, JLPT preparation and business Japanese. This is where money buys the thing free resources cannot reliably provide: scheduled human interaction and correction.

**Why not choose it:** it is expensive compared with self-study, class time is not the same as daily immersion, and I still need reading, vocabulary and listening practice outside class. Coto lists prices that can change, so I check the current fee before enrolling.

**Cheaper paid supplement:** [Bunpro](https://bunpro.jp/) if my main problem is grammar review and spaced repetition, not speaking. It is a tool, not a complete language school.

---

# 5. Bangla support and Bangla-first alternatives

I want Bangla explanations when a concept is blocking me. I do **not** want Bangla to become an excuse to avoid the English documentation that I will need in Europe and Japan.

## Free-first rule

I could not verify one single, stable, fully free Bangla course that covers this whole stack: CS fundamentals → backend → cloud → DevOps → security → production. So I will not pretend that a random Bangla playlist covers 90%.

I use:

- [10 Minute School free catalogue](https://10minuteschool.com/categories/free/) for short Bangla lessons and study support when a topic needs a first explanation.
- Bangla explanations as a **bridge**, then immediately redo the exercise from the English primary course.
- [NHK Bengali Japanese](https://www3.nhk.or.jp/nhkworld/lesson/bengali/) for the Japanese beginner start.

## Paid Bangla-first pick — [Phitron CSE Fundamentals](https://phitron.io/)

**What it appears designed to cover:** a Bangla-led, structured foundation around C, C++, data structures, algorithms, competitive programming and software-development preparation, with support and placement-oriented claims on its current site.

**Why choose it:** if Bangla explanation, accountability and a long structured cohort are the exact bottleneck, it may be more useful than buying five disconnected courses.

**Why not choose it:** its centre of gravity is CSE fundamentals and competitive programming, not the complete Linux → backend → cloud → SRE ladder. Placement stories are not a guarantee. I would not take it **instead of** a degree or the engineering project gates.

**Alternative Bangla web path:** [Programming Hero](https://www.programming-hero.com/) currently advertises an AI-driven full-stack path covering JavaScript/TypeScript, React, Next.js, Node.js, Express, MongoDB, authentication, deployment and AI-assisted workflows. I would choose it only if my target changes toward full-stack web development; it is not the best match for the cloud/platform direction of this repo.

---

# 6. Other side skills that quietly decide whether the plan works

These do not get their own giant curriculum.

| Side skill | One free anchor | Practical proof |
|---|---|---|
| Technical writing | [Google Technical Writing](https://developers.google.com/tech-writing) | Rewrite a confusing README and explain the change. |
| Documentation and open source | [Open Source Guides](https://opensource.guide/) | Make one small documentation or bug-fix contribution. |
| Maths for computing | [Khan Academy math](https://www.khanacademy.org/math) | Repair algebra, probability or discrete-math gaps when the degree requires it. |
| Typing and keyboard fluency | [keybr](https://www.keybr.com/) | Type accurately enough that the keyboard is not the bottleneck. |
| Presentation | [TED-Ed public speaking lessons](https://ed.ted.com/) + my own recordings | Explain one architecture diagram in five minutes. |
| Host-country language | The government's public course or a local university/community course | Handle housing, health, banking and university conversations. |

The rule is simple: I add a side skill only when it removes a real obstacle in the current phase.

---

# My weekly operating system

- **Main technical block:** 60–90 minutes, five days a week.
- **English maintenance:** 20–30 minutes most days, mostly through the technical work I am already doing.
- **Japanese:** 20–30 minutes a day while overloaded; more only when the current phase justifies it.
- **One project block:** at least once a week, with no tutorial open for part of the time.
- **One review:** every Sunday, record what I can do without help and what failed.

I do not start a second main course because the first one feels slow. I change course only when there is a clear failure: wrong level, missing prerequisite, poor format, or a goal that genuinely changed.

## Sources and checking rule

I checked the official course/provider pages on **2026-09-26**. Prices, subscriptions, course editions, immigration rules, cloud free tiers and exam policies change. Before paying, applying, deploying billable cloud resources, or relying on a certificate, I open the official page again.
