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

### [The key: Use AI as a training partner, not a replacement for thinking.]{.block .mt-1em}

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

- **Large Language Model**: An AI model trained on massive amounts of text data from books, websites, and other sources.
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

## ⚠️ Important: Data Privacy and Security

When using AI tools, be aware:

### [What NOT to share:]{.block .mt-1em}

- Personal information (addresses, phone numbers, ID numbers)
- Sensitive data from internships or work
- Code from group projects (without permission from teammates)
- Proprietary or confidential information

### [Remember:]{.block .mt-1em}

- AI systems log your conversations
- Your data may be used to train future models
- Assume anything you share could become public
- When in doubt, ask your instructor or supervisor first

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
Act like a really critical and stern (but just)
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

## Who It's For (Audience)

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

Ask the system to break down complex tasks (most ‘thinking’ models do this for you):

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
- Specify constraints: `Don't use frameworks or libraries we haven't covered`
- Ask: `Can you solve this using only <specific concepts>?`
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
- Use phrases like: `Be critical` or `Don't just agree with me`

---
layout: section
class: text-left
---

# 5. Studying with AI

[5.1 Explaining concepts]{.block .text-left}
[5.2 Explaining code]{.block .text-left}
[5.3 Fixing Code]{.block .text-left}
[5.4 Programming Assignments]{.block .text-left}
[5.5 Extra exercises]{.block .text-left}
[5.6 Checking for understanding]{.block .text-left}
[5.7 Hardcore Learning Mode: Socratic Learning]{.block .text-left}
[5.8 More ideas]{.block .text-left}

---
layout: section
---

## 5.1 AI for Explaining Concepts

---

## Two Ways to Ask AI to Explain Concepts

### [❌ "Just tell me what it is"]{.block .mt-1em}

### [✅ "Help me understand by building on what I know"]{.block .mt-1em}

---

## [❌ Example: The Wrong Way]{.block .mb-1em}

```markdown
What is typecasting?
```

#### [Problems:]{.block .mt-1em}

- You get a generic definition that might be too advanced
- AI doesn't know what you already understand
- Explanation might use concepts you haven't learned yet
- You can't connect new knowledge to existing knowledge
- No way to check if you actually understood❗️

---

## [✅ Example: The Learning Way]{.block .mb-1em}

```markdown {*}{maxHeight:'360px'}
I'm learning about data types in Java. I understand primitive types like int and double,
and I know that variables have specific types.

I have seen the term "typecasting" but I'm not sure what it means or when to use it.

Could you help me understand typecasting by:

1. First asking me what I already know about data types and type compatibility
2. Then explaining typecasting using simple examples that build on these concepts
3. Showing me practical examples in code where typecasting is needed
4. Asking me questions to check if I understand the difference between implicit and explicit casting
5. Suggesting a small exercise I can try myself to practice the concept
```

---

## If the concept is still not clear

Tell the AI to:

- `Explain this like I am 12 years old.`
- `Give me a real life example`
- `Give me a simple code example`
- `Break it down step by step`
- `Connect it to things I already know`

---
layout: section
---

## 5.2 AI for Explaining Code

---

## Two Ways to Ask AI to Explain Code

### [❌ "What does this code do?"]{.block .mt-1em}

### [✅ "Help me understand this code step by step"]{.block .mt-1em}

---

## [❌ Example: The Wrong Way]{.block .mb-1em}

```markdown
What does this code do?

public static boolean isValidEmail(String email) {
return email.matches("^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$");
}
```

#### [Problems:]{.block .mt-1em}

- You get a quick summary but don't understand HOW it works
- AI might use technical terms you don't know (regex syntax)
- You can't apply this knowledge to similar problems
- You won't be able to modify or debug it later
- You miss the learning opportunity❗️

---

## [✅ Example: The Learning Way]{.block .mb-1em}

```markdown {*}{maxHeight:'360px'}
I'm learning Java and I found this email validation code online.
I understand basic String methods like length() and charAt(), but I am still
learning about regular expressions.

public static boolean isValidEmail(String email) {
return email.matches("^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$");
}

Could you help me understand this code by:

1. First explaining what the matches() method does in simple terms
2. Breaking down the pattern piece by piece (what does ^ mean? what does + mean?)
3. Showing me what email addresses would pass and fail this validation
4. Asking me questions to check if I understand each part
5. Suggesting how I could test my understanding by modifying the pattern
```

---

## If it is still not clear

`Explain this code line by line, statement by statement.`

---
layout: section
---

## 5.3 AI for Fixing Code

---

## Two Ways to Ask AI to Help Fix Code

### [❌ "Fix this code"]{.block .mt-1em}

### [✅ "Help me debug this problem"]{.block .mt-1em}

---

## [❌ Example: The Wrong Way]{.block .mb-1em}

```markdown
Fix this code:

public static double calculateAverage(int[] numbers) {
int sum = 0;
for (int i = 0; i <= numbers.length; i++) {
sum += numbers[i];
}
return (double) sum / numbers.length;
}
```

#### [Problems:]{.block .mt-1em}

- AI just gives you the fixed code without explanation
- You don't learn to identify the bug yourself
- You won't recognize this type of error next time
- You miss developing debugging skills
- You don't understand WHY it was wrong❗️

---

## [✅ Example: The Learning Way]{.block .mb-1em}

```markdown {*}{maxHeight:'360px'}
I'm learning Java arrays and I'm getting an ArrayIndexOutOfBoundsException with this code.
I understand arrays and for loops, but I'm not sure what's causing the error.

public static double calculateAverage(int[] numbers) {
int sum = 0;
for (int i = 0; i <= numbers.length; i++) {
sum += numbers[i];
}
return (double) sum / numbers.length;
}

Could you help me debug this by:

1. First asking me what I think might be wrong (let me try to figure it out)
2. Giving me hints about which line is causing the problem
3. Asking me questions about how array indexing works
4. Explaining why this error happens and how to prevent it in the future
5. Suggesting how I can test the fix to make sure it works correctly
```

---
layout: section
---

## 5.4 Programming Assignments

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
layout: section
---

## 5.5 AI for Creating Extra Practice Exercises

---

## Getting More Practice with AI-Generated Exercises

AI can create custom practice exercises that match your course material and current skill level.

### [The key: Be specific about what you're learning and what style of exercises you need.]{.block .mt-1em}

---

## [✅ Example: Good Practice Exercise Request]{.block .mb-1em}

```markdown {*}{maxHeight:'360px'}
I'm learning about loops and arrays in Java. We just finished a chapter on:

- for loops and while loops
- one-dimensional arrays
- finding min/max values in arrays
- calculating sums and averages

Our course exercises typically:

- Start with a clear problem description
- Include example input and expected output
- Focus on one or two concepts at a time
- Don't require advanced topics we haven't covered yet

Could you create 3 practice exercises similar to what we've been doing?
Make them progressively harder:

- Exercise 1: Basic (just applying what we learned)
- Exercise 2: Medium (combining two concepts)
- Exercise 3: Challenge (requiring some creative thinking)

For each exercise, provide:

- The problem description
- Example input/output
- Hints if I get stuck (but don't show me the solution yet)
```

---
layout: section
---

## 5.6 AI for Checking Your Understanding

---

## Using AI to Test If You Really Understand

After learning a concept, use AI to verify your understanding through questions and explanations.

### [The key: Ask AI to quiz you or have you explain concepts back, rather than just re-explaining them.]{.block .mt-1em}

---

## [✅ Example: Good Understanding Check Request]{.block .mb-1em}

```markdown {*}{maxHeight:'360px'}
I just finished studying instance methods vs class methods in Java. I think I understand the basics:

- When to use static vs non-static methods
- How to call instance methods vs class methods
- That instance methods can access instance variables
- That static methods can't access instance variables directly

Before I move on to the next topic, I want to make sure I really understand this.

Could you help me check my understanding by:

1. Asking me 3-4 questions about instance and class methods (don't give me the answers yet)
2. After I answer each question, tell me if I'm right or wrong and why
3. If I get something wrong, ask me follow-up questions to help me figure it out
4. Give me a small coding scenario and ask me to explain what would happen
5. At the end, tell me what gaps in my understanding I should work on

Make the questions progressively harder to really test if I understand deeply.
```

---

## 5.7 Hardcore Learning Mode: Socratic Method

Want to really understand something?

Tell AI:

```markdown
You are like a Socratic teacher: please don't give me answers right away.
Instead, ask me questions that help me figure it out myself.
```

---

### Example: Regular Way

`How do I center something with CSS?`

vs.

### Socratic, Question-Based Learning

```markdown
I'm learning CSS layout. Use the Socratic teaching method and instead of telling me how,
you ask me questions that help me discover how to center elements by myself?
```

---

AI might ask:

```markdown
- What CSS properties do you know for positioning?
- How does display:flex work?
- What have you tried so far?
```

---

### Try It!

Pick something you're learning and:

1. Ask AI to be your question-asking teacher
2. Try to answer its questions
3. See what you discover!
4. How did you feel about this?

(5 minutes)

---

### Why Questions Work Better

- You understand deeper
- You remember longer
- You learn to solve problems
- Learning is more fun
- You feel more confident (afterwards)

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
- ...

---

## Practice: Rubber Ducking

Ask your favourite AI Chat System how it could help you with your programming assignments by rubber ducking.

Ask it for a good prompt to start a rubber ducking session.

---

## Example Output

```markdown {*}{maxHeight: '360px'}
**What “rubber ducking” means**

_Rubber duck debugging_ (or simply _rubber ducking_) is a problem-solving technique used by programmers:
you explain your code, line by line, out loud to an inanimate object—traditionally a rubber duck.
The act of explaining forces you to slow down, articulate assumptions, and notice mistakes or gaps
in logic that you’d normally overlook while thinking silently.

As ChatGPT, I can act as the “rubber duck”:

- I won’t solve the problem for you.
- I’ll ask clarifying questions that help you reason through the issue.
- I’ll encourage you to articulate their intention, assumptions, and understanding of each part of the code.

This helps build independence and problem-solving skills rather than providing answers outright.

### 🟡 A good prompt to start a rubber-ducking session

> **Rubber Duck Mode:**
> I want you to act as a rubber duck for debugging my code.
>
> - Do _not_ give me the solution directly.
> - Ask me questions that help me uncover the issue myself.
> - Encourage me to explain what each part of my code is supposed to do, what I expect to happen,
>   and what actually happens.
> - If I make unclear or incorrect assumptions, ask me to clarify or reconsider them without giving
>   the answer outright.
>
> I’ll start by describing my assignment, my goal, and the part of the code I’m stuck on.
```

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
