# linkedin-recruiter-email

## A recruiter sent me a clever message written in code. I fixed it.

### Here is the email I was sent, unedited but anonymized.

```
Document.respondtomessage.visible=true;

Chris,

While (heck_yes != “no”) {
While (heck_yes != “no”) {
If (you_desire == “YES”) {
my_job_to_be = “Challenging, where I get to come into work and be able to use my creative side to develop new applications and break down an applications and make it better.”;
Document.write (“Yes, [recruiter's name], Contact me because I desire this”);
} else if (you_desire==”right on!”) {
My_job_to_be=”Be challenged to bring your creative skills in, to be part of the solutions to complex problems and be valued.”;
Document.write (“Yes, [recruiter's name], Contact me because I desire this”);
} else if (you_desire == “you_had_me_at_hello”) {
My_job_to_be=”Where I want to wake up every day wanting to go to work, love the people I work with, and feel compensated for my worth.”;
Document.write (“Yes, [recruiter's name], Contact me because I desire this”);
} else if (you_desire == “now you’re just toying with me [recruiter's name]!”) {
My_job_to_be=”Able to keep learning new technologies and putting them to good use while I do all the above.”;
Document.write (“Yes, [recruiter's name], you’fe killing me! Contact me because I desire this”);
} else {
Document.write (“No [recruiter's name], I want none of these things and want to be stagnant with my same old job, and to be phased out of new opportunities.”);
//Staying on top of your industry is necessary. Partner with and actual IT guy not a recruiter that just cares about money and shoving you through a square hole.
}
}

[recruiter's name]
[recruiter's contact info]
```

There are several glaring issues with this code. First off, it's a bit difficult to call out which language the recruiter was attempting to use. The capital `While` and `If`s threw me for a loop. But the `Document.write` [sic] made me think it was supposed to be JavaScript.

The lack of indentation made my eyes bleed. I mean, _actually_ bleed. It was weird.

In this repo, you'll find a perfectly passable web application that accomplishes what I feel this recruiter set out to do. It's clean, extensible and has zero dependencies. HOW HOT IS THAT?

# So let's fix this shit.

```
While (heck_yes != “no”) {
While (heck_yes != “no”) {
```

Ok. I'm not sure why we're doing two nested `while` loops based on the same condition, but I'm an open-minded guy. I'll roll with it. But I can't abide the snake case, lack of strict comparison and the educated quotes. (Which were no doubt an artifact of composing this code in Microsoft Outlook). I see your game, Recruiter.

```
If (you_desire == “YES”) {
```

Again with the snake case. What is this? Python? Are you Python-izing your JavaScript? Is this crazyland? Also, `desire` represents a true or false state, so it'd be better to use a boolean in this case. If you open it up to being a string, you're gonna have all kinds of desires lurking around and this code is going to become completely unmaintainable. I think you'd agree, that is not `desire`able.

```
my_job_to_be = “Challenging, where I get to come into work and be able to use my creative side to develop new applications and break down an applications and make it better.”;
Document.write (“Yes, [recruiter's name], Contact me because I desire this”);
} else if (you_desire==”right on!”) {
My_job_to_be=”Be challenged to bring your creative skills in, to be part of the solutions to complex problems and be valued.”;
Document.write (“Yes, [recruiter's name], Contact me because I desire this”);
} else if (you_desire == “you_had_me_at_hello”) {
My_job_to_be=”Where I want to wake up every day wanting to go to work, love the people I work with, and feel compensated for my worth.”;
```

Ok. Now you're just getting silly. You set a variable that was never declared and then decide a few lines later that `my_job_to_be` should be `My_job_to_be`. Let's set aside that you assign this variable and never use it. Let's set aside that the snake case and capitalization completely break whatever logic you were attempting to achieve. `you_had_me_at_hello`??? Come on, man. I mean... _come on_.

Also, `document.write` is a bad practice. Stop it.

```
Document.write (“Yes, [recruiter's name], you’fe killing me! Contact me because I desire this”);
```

Spelling error. Very unprofessional. See me after class.

```
//Staying on top of your industry is necessary. Partner with and actual IT guy not a recruiter that just cares about money and shoving you through a square hole.
```

Another spelling error. `and` should be `an`. I know it's just a comment, but this stuff matters. Also, you should consider that maybe I _want_ to be shoved through a square hole. All night. YEAH! This code review just got SEXY!

## Thanks for reading. Pull requests welcome.
