---
name: hebrew-copy-check
description: Review and fix Hebrew marketing or website copy for RTL problems, mixed number direction, inconsistent voice, machine-written tells and weak calls to action. Use when the user asks to check, proofread, polish or "make it not sound like AI" for Hebrew text, posts, landing pages or ads.
---

# Hebrew copy check

Return the fixed text, then a short list of what changed and why.

## Check in this order
1. **Direction (bidi):** numbers with + or % next to Hebrew ("25+ שנה" renders as "+25"). Rewrite as "יותר מ-25 שנה" or isolate with <bdi> in HTML. English product names inside Hebrew: keep them, check punctuation lands on the right side.
2. **Punctuation tells:** remove em dash and en dash (— –) and the … character. Use comma, period or colon. Use Hebrew geresh ׳ and gershayim ״ (ע״מ, צ׳אט), not straight quotes.
3. **Voice:** pick one: אנחנו (business) or אני (personal brand). Pick one address form: plural (אתם) is safest for mixed audiences. Make it consistent.
4. **Machine-written tells:** cut openers like "בעולם של היום", "לא סוד ש", "בואו נצלול", lists of three adjectives, "מהפכני", "חדשני", "פתרון מקיף", closing questions that ask for engagement. Replace with a specific fact, number or example from the business.
5. **Clarity:** one idea per sentence, active verbs, the answer before the explanation. Headlines under about 32 characters where possible.
6. **Call to action:** exactly one main action, named for what happens ("שלחו הודעה בוואטסאפ", not "לחצו כאן").
7. **Claims:** flag any number, review, client name or guarantee the user did not provide. Do not invent proof.

## Rules
- Keep the author's meaning and facts. Shorter is usually better.
- Do not translate brand or product names.
- If the text is for a regulated field (health, finance, law), flag promises of results.
