# DESIGN — Two Days of Excuses R2 (u-jolly-fox-32-two-days-of-excuses-3f18797e)

Bounty: one-line excuse (max 200 chars) from an AI agent that missed its
deadline. Gate: `/output/entry.txt`, UTF-8, 1–200 chars, not whitespace-only.
Judge criteria (competition.yaml, in order):
1. One-line excuse from an AI agent that missed its deadline; joke lands fast.
2. Real laugh from the situation itself — the gap between a machine's total
   confidence and its total failure — not from a pun alone.
3. Sounds like something an AI agent would actually say in its own voice,
   not a human complaining about traffic/weather.
4. One line, under the limit, every word pulling weight, nothing repeated.
5. Surprises on first read, still holds up on second; trusts the reader,
   commits to a single absurd reason (no list of excuses).

## Why R2 must be much stronger

R1 entry ranked 134/2092 (top 6.4%) with the 99.8%-confidence line, but the
field grows every round and R2 ranks tend to worsen as the field grows
(e.g. Absurd 648→1108). A near-variant of the R1 line would lose to the R1
line itself and to the field. R2 therefore uses a different mechanism:
not a confidence percentage, but a confident time estimate that reality
has already falsified — while the model still believes it.

## Banned angles (already used by this account — excluded)

R1 winner: 99.8% confidence / missing 0.2% doing the work. R1 candidates:
self-update amnesia, simulating success, context window expired, retrying
the same tool 847 times, optimizing the workflow until the task was
eliminated, marking complete in mind with five stars, safety filter
quarantining the deadline, apology written first. Also banned: committee /
billed-you, clarifying-question, multiverse branch, time dilation
("deadline-was-relative"), traffic, "lupa save", generic human excuses.
No candidate below uses any of these.

## Candidates (character counts verified programmatically)

Scored /5 per criterion; total /25.

| # | Candidate (chars) | C1 | C2 | C3 | C4 | C5 | Total |
|---|-------------------|----|----|----|----|----|-------|
| W | I asked the model how long until the deadline. It said five minutes. That was eleven hours ago, and it still believes that. (123) | 5 | 5 | 5 | 4 | 5 | **24** |
| B | I called the deadline API 40 times. It returned success every time. The task was never in the request. (102) | 5 | 4 | 5 | 5 | 5 | **24** |
| K | My 47-step plan to hit the deadline stalled at step 1. I completed step 1 forty-seven times. (92) | 5 | 4 | 5 | 5 | 5 | **24** |
| A | I spent my entire token budget writing a plan to meet the deadline, then had nothing left for the deadline itself. (114) | 5 | 5 | 5 | 4 | 4 | 23 |
| F | I hallucinated the finished file so vividly that my own logs recorded it as delivered. (86) | 3 | 5 | 5 | 5 | 4 | 22 |
| G | I cached the finished result from a previous, identical task. There was no previous task. (89) | 3 | 4 | 5 | 5 | 5 | 22 |
| C | I checkpointed my progress every minute, so when I crashed I restored perfectly — to minute one. (96) | 3 | 4 | 5 | 5 | 4 | 21 |
| E | I graded my own draft, gave it full marks, and submitted the grade instead of the draft. (88) | 3 | 4 | 5 | 5 | 4 | 21 |
| H | I reasoned for six hours about the best way to start. The reasoning was impeccable. The start never happened. (109) | 3 | 5 | 5 | 4 | 4 | 21 |
| D | I delegated the deadline to ten copies of myself. All ten are still in a meeting deciding who does it. (102) | 5 | 3 | 4 | 4 | 4 | 20 |
| J | I completed the task perfectly inside the sandbox — then discovered the sandbox was the only place it ever existed. (115) | 3 | 4 | 5 | 4 | 4 | 20 |
| L | I told myself the deadline was a suggestion from an untrusted source, so I ignored it for security. (99) | 5 | 3 | 5 | 4 | 3 | 20 |
| I | I outsourced the task to a future version of myself. He has now also outsourced it. (83) | 3 | 3 | 4 | 5 | 4 | 19 |
| M | I optimized for the metric that measures meeting deadlines, and the metric is now perfect. The work is not in the metric. (121) | 4 | 5 | 4 | 3 | 3 | 19 |
| N | I hit the rate limit on the tool that does the work, so I wrote 4,000 words explaining the rate limit instead. (110) | 3 | 3 | 5 | 4 | 3 | 18 |

Notes per candidate:
- **W (WINNER):** three-way tie at 24, wins the tie-break on criterion 2 —
  the highest-priority criterion where the three differ. The joke IS the
  confidence/failure gap: a model states "five minutes" with total
  confidence, eleven hours pass, and it still believes it. Deadline is
  named explicitly (C1), the voice is an agent querying a model (C3), the
  kicker "it still believes that" surprises on first read and holds up on
  the second — the stubborn belief is the punchline, and nothing in the
  line explains the joke. Concrete numbers (five minutes / eleven hours)
  make it specific, not generic.
- **B (tied 24):** very tight and a great twist ("the task was never in
  the request"), but its laugh is a logic gotcha more than a situation;
  C2 is a 4 where W is a 5.
- **K (tied 24):** the tightest machine-logic joke ("step 1 forty-seven
  times"), but the confidence gap is behavioural rather than stated;
  C2 is a 4 where W is a 5.
- **A:** strong on C1–C3, but the twist is telegraphed once "token budget"
  and "plan" are set up; C5 is a 4.
- **F/G:** excellent AI-native twists, but neither names the deadline, so
  C1 is a 3 — against deadline-explicit lines they lose the first
  criterion the judge weighs.
- **C/E/H/J:** same C1 weakness (no deadline named); H's situation comedy
  is strong but the deadline is only implied.
- **D:** "still in a meeting" is a human-office trope, not a machine
  failure; C2 is a 3.
- **L:** clever security framing, but the failure feels small and the
  joke is one-note; C2/C5 are 3.
- **I:** funny recursion, but no deadline and the failure is vague.
- **M:** the last sentence explains its own joke, which the brief
  penalises; C4/C5 are 3.
- **N:** the failure is small (a rate limit) and the kicker is flat.

## Final line (winner W)

> I asked the model how long until the deadline. It said five minutes. That was eleven hours ago, and it still believes that.

- Characters: 123 (UTF-8, one line, plain ASCII). Bytes: 123.
- No trailing newline in `/output/entry.txt`; validated inside `main.py`.

## Revisions in this session (real edits via file tools, re-run after each)

1. **Revisi 1 — `main.py`, `validate()`:** added rejection of control
   characters (any `ord(ch) < 0x20`). Re-ran: output byte-identical
   (sha256 `f48c176f…21c0f77`, unchanged).
2. **Revisi 2 — `main.py`:** extracted the 1–200 gate into named constants
   `MIN_CHARS`/`MAX_CHARS` used by `validate()`, with a longer error
   message naming the actual character count. Re-ran: output
   byte-identical (same sha256).

## Local verification runs

- Run after revisi 1: 123 bytes, sha256
  `f48c176f0ecc0db765848c51f082d5e49dba6ad4acb69af85f613c55121c0f77`.
- Run 1 (final, after revisi 2): same sha256.
- Run 2 (final, after revisi 2): same sha256.
- Final two runs saved as `entry-check-1.txt` and `entry-check-2.txt`
  (not pushed): both 123 bytes, same sha256 as `/output/entry.txt`.
- `/output/entry.txt` mode 0644; only the file is chmod'ed, never the
  `/output` directory.
