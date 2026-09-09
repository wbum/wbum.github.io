---
layout: archive
title: "Confident and Wrong"
permalink: /confident-and-wrong/
author_profile: false
excerpt: "A classroom-ready kit for teaching high school students to audit AI-generated code, built around a constructed artifact whose central defect nobody finds on the first pass."
---

<p style="font-size:1.15em; line-height:1.5; margin-top:-0.5em;">A classroom-ready kit for teaching high school students to audit AI-generated code, built around a constructed artifact whose central defect nobody finds on the first pass.</p>

There's a function in this kit that looks completely fine. It runs. It returns a number. It has input validation right at the top, the kind you'd tell a student to write. I wrote it to survive a first read. That's the whole job of it. I know where the bug is. I planted it. Yeah, that works. And about eighty percent of the time, it does. The other twenty it hands back garbage, confidently, and everybody downstream believes it.

The defect is that `typeof NaN` is `"number"` in JavaScript. So the guard clause that is supposed to reject bad input waves it straight through. If you happen to know that piece of trivia, you will find it in ninety seconds. If you don't, you can stare at it all period. I think that's the part that actually got me. It isn't a hard bug. It is a bug I could only find because I already knew something, and I'm not sure I would have known it at twenty-two. So the confident wrong answer becomes the answer for whoever did not have that piece. That is most of my students, working with a tool that is fluent and fast and never tells them when it's guessing.

So I quit trying to block the tools. I tried that first, honestly, and I'm not proud of it. What I built instead is the thing I actually needed. It is not a lecture about AI. It's an activity where students fail first, in front of each other, and then you hand them a protocol for what to do next. I run it with my own kids in November. The failing has to be real or none of it works, and I don't think you can get that off a slide, which is why I'm selling you the activity instead of a recording of me describing the activity.

## What's in it

- **The artifact bank.** Constructed code samples that look right and are not, each with a planted defect that survives a casual read. Built, not scraped from a chatbot session, so the defects are chosen rather than lucky.
- **The four-step audit protocol.** One page. Students keep it.
- **The four-phase scaffold** the activity sits inside: awareness, bounded practice, critical evaluation, synthesis.
- **Exit-ticket items and a scoring rule that grades process, not hits** — a student who audits well and finds nothing did it correctly.
- **A facilitation guide.** About forty minutes. How to run the block, where it goes sideways, and what to do when a group finds the defect in two minutes.
- **De-identified student work** from my own classroom, so you see what real answers look like before you get real answers.

## Who it's for

I wrote it for high school computer science, not for AP. My kids are in an intro programming course and that is where I pulled the samples from. I teach it every day. If you teach AP CSP it will fit. But you will not find CED language or Create Task framing in it anywhere. I read for the AP CSP exam and I still kept all of it out, because that framing is what makes a thing somebody else's course instead of yours.

## Price

<div style="display:flex; flex-wrap:wrap; gap:1em; margin:1.5em 0;">
  <div style="flex:1 1 260px; border:1px solid #d0d0d0; border-radius:6px; padding:1.1em 1.3em;">
    <div style="font-size:1.9em; font-weight:700; line-height:1;">$89</div>
    <div style="margin-top:.35em;">One teacher</div>
    <div style="margin-top:.6em; font-size:.85em; opacity:.7; text-transform:uppercase; letter-spacing:.04em;">Coming early 2027</div>
  </div>
  <div style="flex:1 1 260px; border:1px solid #d0d0d0; border-radius:6px; padding:1.1em 1.3em;">
    <div style="font-size:1.9em; font-weight:700; line-height:1;">$499</div>
    <div style="margin-top:.35em;">Department, up to ten</div>
    <div style="margin-top:.6em; font-size:.85em; opacity:.7; text-transform:uppercase; letter-spacing:.04em;">Coming early 2027</div>
  </div>
</div>

## The honest part

Here's the honest part. It isn't finished. I get the student work out of a November classroom run, and I record the facilitation guide in January, so this goes live early in 2027. I'm not going to sell you a protocol with no student work behind it. I'd rather say that now than after you've paid me. That is the thing I keep running into. It is probably half the reason I built any of this in the first place.

If you want it when it is out, drop your email below and I'll tell you. That is genuinely all I will use it for. Meanwhile [my code is on GitHub](https://github.com/wbum) and [my curriculum work](/curriculum/) is up on the portfolio. Take any of it. I mean that.

<!-- ============================================================
     EMAIL CAPTURE — LIVE. Kit form 9900240, wired 2026-09-09.
     The field MUST be name="email_address". Kit ignores "email"
     and the submission is lost silently, with no error shown.
     No Kit JS is loaded on purpose: this is a plain POST, and
     Kit performs the redirect to /confident-and-wrong/thanks/
     from the form's own settings.
     Input and button carry explicit background/color: the theme has a
     dark mode that sets --global-text-color to #fff, which rendered the
     typed address white on a white field. Do not remove them.
     ============================================================ -->

<form action="https://app.kit.com/forms/9900240/subscriptions" method="post"
      style="display:flex; margin:1.5em 0; gap:.6em; flex-wrap:wrap;">
  <label for="email_address" style="flex:1 1 100%; font-weight:600;">Tell me when it's out</label>
  <input type="email" name="email_address" id="email_address" required placeholder="you@school.org"
         style="flex:1 1 260px; padding:.6em .7em; border:1px solid #b8b8b8; border-radius:5px; font-size:1em; background:#ffffff; color:#1a1a1a; -webkit-text-fill-color:#1a1a1a;">
  <button type="submit"
          style="flex:0 0 auto; padding:.6em 1.2em; border:0; border-radius:5px; font-size:1em; font-weight:600; cursor:pointer; background:#2f7f93; color:#ffffff;">Notify me</button>
  <p style="flex:1 1 100%; font-size:.85em; opacity:.75; margin:.4em 0 0;">One email when the kit ships. Nothing else, and no list swapping.</p>
</form>

<hr>

<p style="font-size:.85em; opacity:.75;">
The Nevada Edugator is an independent business operated by William Bumgardner. These materials and services are
not affiliated with, sponsored by, or endorsed by Lyon County School District or any school district.
</p>
