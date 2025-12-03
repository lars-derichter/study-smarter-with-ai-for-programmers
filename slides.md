---
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /cover.png
# some information about your slides (markdown enabled)
title: Study Smarter with AI (as a Programming Student)
info: |
  Workshop on studying with AI as a Programming Student.
  Given on 2025-12-03 to the students of the Associate Degree
  of Software Development at Thomas More University of Applied
  Sciences.
  &copy; Lars De Richter

# apply UnoCSS classes to the current slide
class: text-center
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

# Study Smarter with AI

## (as a Programming Student)

---

## Who am I?

- Lars De Richter
- Lecturer at [Thomas More University of Applied Sciences](https://thomasmore.be)

---

## Topics

1. Learning vs Getting Answers
2. Current AI Tools
3. Writing Better Prompts
4. Troubleshooting
5. Studying with AI
6. Even More Use Cases

---
layout: section
---

# 1. Learning vs Getting Answers

<!--
Wie sport regelmatig?
Hoe weet je of je goed bezig bent? Of je sterker aan het worden bent?

=> beetje pijn
-->

---
layout: fact
---

# If it doesn’t hurt a little, you didn’t learn!

_-- Anonymous_

<!--
No pain, no gain!

Zonder moeite te doen, leer je niet bij.
-->

---
layout: image
image: /watching-cycling.png
---

[I’ll become a great developer…]{.absolute .top-1em .left-1em}

[…by watching ChatGPT do the work.]{.absolute .bottom-1em .right-1em}

---
layout: image
image: /muscle-toner.png
---

[When you ask AI to write every function]{.absolute .top-1em .left-1em}

[but still expect your brain to get stronger]{.absolute .bottom-1em .right-1em}

---
layout: image
image: /cycling-in-the-rain.png
---

[Typing code, breaking code, fixing code]{.absolute .top-1em .left-1em}

[THIS is how you become a developer!]{.absolute .bottom-1em .right-1em}

---

## Cognitive offloading:

### [when we rely on external tools (like AI) to do our thinking for us.]{.block .mt-1em}

- Short-term: Feels efficient, saves time
- Long-term: Prevents skill development, reduces problem-solving ability
- Result: You become dependent on the tool instead of developing expertise

### [The key: Use AI as a _training partner_, not a _replacement_ for thinking.]{.block .mt-1em}

---
layout: iframe
url: https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:7399510076979601408?compact=1
---

---
layout: iframe
url: https://www.linkedin.com/embed/feed/update/urn:li:share:7398424554987065344
---

---
layout: fact
---

# [If you are serious about learning, never ever just ask for the answer!]{.block .text-left}

---
layout: section
---

# 2. Current AI Tools

---

## Remarks

- By AI-tools I mean generative AI-Tools, mainly based on Large Language Models (LLM)
- All tools that we will use during this workshop use a chat interface
- Continually evolving
- Different qualities
- Different styles
- General principles and tricks work everywhere!

---

## LLM

- **Large Language Model**: An AI model trained on massive amounts of text data (basically all of the internet).
- Learns patterns in language: grammar, facts, reasoning, and even coding patterns.

---

## GPT

- **Generative Pre-trained Transformer**: An AI architecture that predicts the next word in a sequence based on patterns learned from training data.
- Takes your input (prompt) and generates responses by predicting what text should come next, word by word.
- Can handle various tasks (coding, writing, analysis) because it learned from diverse text sources during training.

---

## The Big Three

- [ChatGPT](https://chatgpt.com/)
- [Gemini](https://gemini.google.com/app)
- [Claude](https://claude.ai/)

---

## European Alternative

[Mistral](https://chat.mistral.ai/chat)

---

## Other Systems

- Llama, Deepseek, Grok, Qwen
- Multisystem Online Interfaces: [Abacus.ai](https://apps.abacus.ai/chatllm/)
- Local Interfaces: [AnythingLLM](https://anythingllm.com/), [Ollama](https://ollama.com/)
- ...

---

## ChatGPT Settings for Educational Use

- In Settings \>\> Personalization
  - Base style and tone -> Professional
  - Custom Instructions: see ‘Custom Instructions and Memory’
  - Occupation: Beginning Software Development student learning Java
- In Chats:
  - \+ \>\> More \>\> Study and learn (almost always)

Study and learn makes ChatGPT more like a tutor and less likely to ‘just give the answer’. (But it is far from perfect.)

---

## Claude Settings for Educational Use

- In Settings \>\> General \>\> What personal preferences should Claude consider in responses?:

```markdown
I am a beginning Software Development student learning Java
```

(See ‘Custom Instructions and Memory’ for more tips)

- In chats:
  - Settings Icon \>\> Use style -> Learning
  - Web search -> active

---
layout: section
---

# 3. Writing better prompts

---

## It’s all about the context!

- The system needs to know your background
- The system needs to know what you want
- The system needs to know your limitations
- You can tell the system all of these things!

---

## Parts of a Good Prompt

1. Context: Your Situation
2. Role: Who You Want AI to Be
3. Task: What You Want to Do
4. Format: How You Want the Answer (when needed)
5. Audience: Who It's For (when needed)
6. Scope: What's Included/Not Included (when needed)
7. Step-by-Step (when needed)

---

## Your Situation (Context)

Tell AI about yourself and what you know:

```markdown
I'm a first-year web student. I know how to:

- Write semantic HTML
- Style with CSS
- Use grid-template-area for layout
```

---

## Who You Want the System to Be (Role)

Tell the system what kind of expert you need:

```markdown
You are a patient teacher who's really good at
explaining things to beginners...
```

```markdown
Be like an experienced web developer who always
writes clean, simple code...
```

```markdown
Be like a really critical and stern (but just)
teacher with expert knowledge of web development...
```

---

## What You Want (Task)

Be specific about what you need:

❌ Bad: `Make a form`

✅ Good:

```markdown
Help me create a simple contact form that:

- Gets the user's name and email
- Checks if the email has the right format
- Shows a message when sent
```

---

## How You Want It (Format)

Tell the system how to present the solution:

```markdown
Please show me:

- HTML first
- Then CSS
- Add helpful comments
- Keep it simple - plain HTML and CSS, no frameworks
```

---

## Who it's for (Audience)

For texts or user facing products. Tell the system who the product is for:

```markdown
The letter is for potential employers at a startup specialising in mobile apps...
```

```markdown
The target users are teenagers with an interest in online gaming...
```

---

## What's Included (Scope)

Be clear about what you need (and don't need):

```markdown
For now, I just need:

- The form layout
- Basic styling
- Simple checks
- No fancy features yet
```

---

## Step by Step (When Needed)

Ask the system to break down complex tasks (most modern (deep) ‘thinking’ models do this for you:

```markdown
Can you help me build this form by:

1. First showing the basic HTML
2. Then adding simple CSS
3. Finally adding basic checks
4. Explain each part before moving on
```

---

## ❌ Bad Example

```markdown
Fix this code:

<div class="card">
  <h2>Title</h2>
  <p>Text</p>
</div>
```

Problems:

- Doesn't say what's wrong
- Doesn't say what you want
- Doesn't mention your skill level

---

## ✅ Better Example

```markdown
I'm learning CSS and this card won't center on the page.
I know about flexbox but I'm not sure how to use it here.
Can you explain what I need to add and why it works?

<div class="card">
  <h2>Title</h2>
  <p>Text</p>
</div>
```

---

## Practice Exercise

Make this basic prompt better:

```markdown
Help me make a website header with a logo and menu
```

Take 5 minutes to improve it!

---

## Example Solution

```markdown {*}{maxHeight:'360px'}
I'm a first-year web student learning HTML and CSS.

Could you be like a helpful teacher and show me how to make
a simple website header that has:

- A logo on the left
- A menu on the right
- Works on phones too

I know about:

- Basic HTML
- CSS flexbox
- Simple styling

Please show me:

- Clean HTML first
- Simple CSS using flexbox
- Helpful comments
- No complex features yet

I want it to:

- Look good on all screens
- Be easy to read
- Be simple to maintain
```

---

## Keep Improving Your Prompts (~ iterative development)

You don't need a perfect prompt on the first try!

### [Start simple, then refine:]{.block .mt-1em}

1. **Start with a basic request** - Get the conversation going
2. **Review the response** - Does it match what you need?
3. **Add missing details** - "I should have mentioned I can't use..."
4. **Ask for adjustments** - "Can you make this simpler?" or "Explain step 3 more"
5. **Clarify misunderstandings** - "Actually, I meant..." or "That's not quite right..."

### [Remember:]{.block .mt-1em}

- Conversations are iterative - each message builds on the previous
- It's okay to guide AI toward what you need
- Asking follow-up questions shows you're thinking critically

---

## Custom Instructions and Memory

Most current systems have

- custom instructions or preferences that are reused in every prompt
- projects with custom instructions and context that you can reuse between chats
- memory across chats

You can put your context, the roles you want the system to be etc. there.

(I’ll show you in ChatGPT and Claude)

---

## Bonus: Ask AI to Improve Your Prompts

```markdown
Act as an expert prompt engineer with specialized knowledge of LLM behavior.

Review and optimize the prompts I provide by:
Increasing clarity and conciseness
Preserving all essential instructions and information
Using direct, specific language that elicits optimal LLM responses
Improving structure and organization where needed

For each prompt:
Present the optimized version first
Explain key improvements and their expected impact on output quality
Identify any remaining weaknesses or limitations
```

---
layout: section
---

# 4. Troubleshooting

---

## Answers with Unknown Concepts

### AI suggests solutions using concepts, libraries, or techniques you haven't learned yet in your course.

### [Risks:]{.block .mt-1em}

- Using code you don't understand and can't explain
- Missing the learning objective of the assignment
- Unable to adapt or debug the solution when problems arise
- Getting flagged for using unauthorized tools or approaches

### [How to prevent it:]{.block .mt-1em}

- Tell AI what you've learned: `I only know 'for loops' and 'while loops'`
- Specify constraints:`Don't use frameworks or libraries we haven't covered`
- Ask: `Can you solve this using only \[specific concepts\]?`
- If AI uses unknown concepts, ask: `Can you do this with simpler techniques?`
- **Always understand every line before using it❗️**

---

## Hallucinations

### AI confidently presenting false information, non-existent facts, or made-up code as if they were real.

### [Risks:]{.block .mt-1em}

- Using code that doesn't actually work or uses non-existent functions
- Learning incorrect concepts or facts
- Wasting time debugging fabricated solutions
- Building on false foundations in your understanding

### [How to prevent it:]{.block .mt-1em}

- Always verify code suggestions by testing them
- Check facts against official documentation
- Ask: `Are you sure this function/library exists?`
- Be skeptical of overly specific details (version numbers, exact syntax)
- Cross-reference important information with reliable sources

---

## Context Rot

### AI "forgets" earlier parts of long conversations and gives inconsistent or contradictory advice.

### [Risks:]{.block .mt-1em}

- Solutions that contradict earlier advice
- Loss of important requirements or constraints
- Wasted time fixing conflicts between responses
- Confusion about which approach to follow

### [How to prevent it:]{.block .mt-1em}

- Start a new chat for new topics/problems
- Summarize key points periodically: `So far we've established...`
- Include important context in each message
- Ask AI to recap: `What are the main requirements we discussed?`

---

## Sycophantism

### AI agreeing with you even when you're wrong, to please you

### [Risks:]{.block .mt-1em}

- Reinforces incorrect understanding
- Prevents you from learning the right approach
- Makes you overconfident in wrong solutions

### [How to prevent it:]{.block .mt-1em}

- Explicitly ask AI to challenge your assumptions
- Request: `Tell me if my approach is wrong`
- Ask: `What are the problems with my solution?`
- Use phrases like: `Be critical" or "Don't just agree with me`

---
layout: section
class: text-left
---

# 5. Studying with AI

[5.1 Explaining concepts]{.block .text-left}
[5.2 Explaining code]{.block .text-left}
[5.3 Fixing Code]{.block .text-left}
[5.4 Assignments]{.block .text-left}
[5.5 Extra exercises]{.block .text-left}
[5.6 Checking for understanding]{.block .text-left}
[5.7 Hardcore Learning Mode: Socratic Learning]{.block .text-left}
[5.8 More ideas]{.block .text-left}

---
layout: section
---

## 5.4 AI for Programming Assignments

---

## Two Ways to Use AI for Programming Assignments

### [❌ "Give me the code"]{.block .mt-1em}

### [✅ "Help me understand how to do this"]{.block .mt-1em}

---

## [❌ Example: The Wrong Way]{.block .mb-1em}

```markdown
Write Java code that checks if a string is a valid Belgian IBAN account number.
```

#### [Problems:]{.block .mt-1em}

- You get code but don't learn
- You probably don’t understand the code
- You won’t understand how to fix bugs
- You can't adapt it for other projects
- You miss learning opportunities❗️

---

## [✅ Example: The Learning Way]{.block .mb-1em}

```markdown
I'm learning about regular expressions in Java. I need to validate Belgian IBAN account numbers.

Instead of giving me the complete solution, could you:

1. First explain what makes a valid Belgian IBAN format
2. Then ask me questions to help me think about the regex pattern
3. Let me try writing the pattern myself
4. Give me hints if I'm stuck, but don't write the code for me
5. Check my understanding by asking me to explain my solution
```

---

## 5.8 More Ideas for Using AI as Study Help

- Code reviews - Getting feedback on your own code
- Rubber ducking - Explaining your thinking process to find issues
- Analogies and metaphors - Understanding difficult concepts through comparisons
- Algorithm walkthroughs - Step-by-step execution tracing
- Common pitfalls - Learning what mistakes to avoid
- Best practices - Understanding idiomatic code patterns
- Error message interpretation - Understanding what errors mean
- Project planning - Breaking down larger problems into steps
- Compare approaches - Evaluating different solutions to the same problem
- Documentation lookup - Finding and understanding API/library usage

---

## Practice

Ask your favourite AI Chat System how it could help you with your programming assignments by rubber ducking.

Ask it for a good prompt to start a rubber ducking session.

---
layout: section
---

# Colophon

---

## Contact

Contact me at [lars.derichter@thomasmore.be](mailto:lars.derichter@thomasmore.be)

Find my [LinkedIn Profile](https://www.linkedin.com/in/larsderichter/)

---

## AI Used to Create This Presentation

- Comet browser to resurface saved LinkedIn posts on Cognitive offloading
- ChatGPT for help with configuring [Slidev](https://sli.dev/)
- ChatGPT for images
- Claude (Code) as a sparring partner for improving this slideshow (structure and contents) and reformulating some texts

---

## License

<a href="https://lars-derichter.github.io/learn-with-ai-prg">Study Smarter with AI (as a Programming Student)</a>

© 2025 by <a href="https://lars-derichter.github.io/">Lars De Richter</a>

is licensed under <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a>

<img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">
