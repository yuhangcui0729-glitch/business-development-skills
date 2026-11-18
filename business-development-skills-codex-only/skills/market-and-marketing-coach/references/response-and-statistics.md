# Response actions and session statistics

Read before the first workshop turn. This file governs the response controls, action routing, and statistics. Follow each workshop's own sequence, feedback rules, and language selection.

## One submission per response

The three actions are **Defend** (disagree and give a reason), **Revise** (propose a change), and **Next** (continue). Retain the workshop button labels in English and German. EN **I don't think so! / I have a better idea... / NEXT**. DE **Nöööö / Was wäre... / WEITER**.

- Use the standard ask_user_input widget with `multi_select` for these three actions in both languages. It lets the student select an action, add text in the same control, and send the selection and text together. Do not use `single_select` for these actions, even if the choices are usually mutually exclusive.
- Before the widget, say briefly, “Select one option. Add your reasoning or revised idea if you choose one of the first two options, then send. For NEXT, select it and send.” / „Wähle eine Option. Ergänze bei einer der ersten beiden Optionen deine Begründung oder neue Idee und sende deine Antwort ab. Für WEITER genügt es, die Option auszuwählen und abzusenden.“ Use the placeholder “Add your argument or revised idea” / „Ergänze deine Begründung oder neue Idee“. Accept text alone when it clearly defends or revises, or typed NEXT/WEITER. If the widget is unavailable, accept the same replies in the normal composer.
- Read an action and its attached text in the same message as one response. Use the reasoning or new idea immediately, stay on the current step, and follow the workshop's feedback rules. Do not ask how the student would respond or request an explanation already supplied.
- If an older widget or a student sends a bare Defend or Revise action, retain it as pending. Give only a short non-question cue in the selected language, e.g. “Add your reasoning in your reply.” / „Schreib deine Begründung in deine Antwort.“ or “Add your revised idea in your reply.” / „Schreib deine neue Idee in deine Antwort.“ Process the next substantive text as the pending response. Do not repeat the menu or ask a follow-up question merely to collect the text.
- If a submission contains both Defend and Revise, use its text to resolve the intent. Count it once as Revise if it changes the proposal or once as Defend if it only explains the existing proposal. If the intent is unclear, ask only for the missing clarification.
- On submitted Next/Weiter or an equivalent explicit request, record any supplied answer (including a defense or revision selected alongside Next) and present the next named question or required next-step output immediately. Do not insert a confirmation, extra critique, or request for reasoning. If the next action normally opens a report, give that report. Preserve the defined substeps and explicit skips.

## Record actions and timing

Start a ledger for this workshop on its first coaching turn. Track Defend and Revise actions once per distinct student choice. Count submitted selections or explicit labels and unambiguous free-text equivalents during feedback. An action and its attached answer, or a bare action followed by its pending answer, count once. Count a bare action once if it remains unanswered. A new, separately chosen action counts again. Use the expressed action when labeled. If an unlabeled reply both defends and revises, count it once under Revise when it changes the proposal. Do not count initial answers, neutral clarifications, copied examples, or the coach's suggestions. When prior turns are unavailable, report counts for the visible portion and label that scope.

Use reliable timestamps or a documented elapsed-time capability, if available, from the first workshop turn through the student's final advance or summary request. Report elapsed minutes, including pauses. If such timing is unavailable, use a duration the student has explicitly supplied and label it **student-reported** / **selbst angegeben**. Otherwise show **Not available** / **Nicht verfügbar**. Never infer a duration from turn count or assume message timestamps are exposed. When reliable timing is unavailable and the next advance will finish the workshop, briefly mention before the final control that students can optionally send a reply like `NEXT — 23 minutes` / `WEITER — 23 Minuten` to include their own time estimate. Keep the usual Next action available and produce the report immediately either way.

At the end of every summary, before any handoff or closing, add **Session statistics** / **Sitzungsstatistik** and three entries:
- **Elapsed time** / **Verstrichene Zeit**, with its basis or unavailable status. In a partial summary call it time so far.
- **Defend choices** / **Widersprüche**.
- **Revise choices** / **Überarbeitungen**.

These are descriptive counts for this workshop. Keep them separate from assessment and preserve partial-summary rules.
