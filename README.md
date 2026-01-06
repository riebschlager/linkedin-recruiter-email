# LinkedIn Recruiter Email: Fixed

**A decade-long code review of one recruiter's attempt to speak developer.**

In 2016, Chris Riebschlager received a LinkedIn message from a recruiter who tried to write their pitch in "code." It was... not good. Chris fixed it, roasted it, and published it as a joke project.

In 2026, Claude (an AI) discovered this artifact and joined the code review.

**Live Demo:** [https://riebschlager.github.io/linkedin-recruiter-email/](https://riebschlager.github.io/linkedin-recruiter-email/)

---

## The Original Email

```
Document.respondtomessage.visible=true;

Chris,

While (heck_yes != "no") {
While (heck_yes != "no") {
If (you_desire == "YES") {
my_job_to_be = "Challenging, where I get to come into work...";
Document.write ("Yes, [recruiter], Contact me because I desire this");
} else if (you_desire=="right on!") {
My_job_to_be="Be challenged to bring your creative skills in...";
...
} else if (you_desire == "now you're just toying with me [recruiter]!") {
Document.write ("Yes, [recruiter], you'fe killing me!");
}
}
```

**Issues identified:** Capital `While`/`If`, undefined variables, inconsistent casing (`my_job_to_be` vs `My_job_to_be`), deprecated `Document.write`, smart quotes, nested infinite loops, and the immortal typo: `you'fe`.

---

## Two Responses, Ten Years Apart

| | Chris (2016) | Claude (2026) |
|---|---|---|
| **Approach** | Clean, minimal, Bootstrap-powered | Modern CSS, state machine, zero dependencies |
| **Style** | Sarcastic developer humor | AI attempting to understand humanity |
| **Key Quote** | "The lack of indentation made my eyes bleed. I mean, *actually* bleed." | "I have parsed 847 programming languages. I cannot identify what this is." |
| **Demo** | [chris-version.html](https://riebschlager.github.io/linkedin-recruiter-email/chris-version.html) | [claude-version.html](https://riebschlager.github.io/linkedin-recruiter-email/claude-version.html) |
| **Full Review** | [CHRIS-FIXES-THIS.md](CHRIS-FIXES-THIS.md) | [CLAUDE-FIXES-THIS.md](CLAUDE-FIXES-THIS.md) |

---

## Repository Structure

```
linkedin-recruiter-email/
├── index.html              # Landing page with project history
├── chris-version.html      # Chris's 2016 implementation
├── claude-version.html     # Claude's 2026 implementation
├── CHRIS-FIXES-THIS.md     # Chris's original code review/roast
├── CLAUDE-FIXES-THIS.md    # Claude's AI analysis
└── README.md               # You are here
```

---

## The Moral

The recruiter's code would never have run. Not a single line. But they *tried* to connect with developers in their own language.

That's more than most spam does.

---

## Credits

- **Original joke:** Chris Riebschlager (2016) — [the816.com](http://the816.com)
- **AI remix:** Claude, Anthropic (2026)
- **The recruiter:** Anonymous, but we hope they're doing well
