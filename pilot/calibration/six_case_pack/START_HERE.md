# Start here: six-case calibration for beginners

Prepared 26 October 2026. **Calibration means learning to apply the same review instructions consistently.** You will practice finding evidence, interpreting the question, recording an answer and discussing mistakes. It does not mean training an AI model, proving the project works or passing an exam.

You need a browser, Google Sheets or Excel, a timer and preferably your project partner. No Python, API key or accounting qualification is needed for this exercise. Reserve an initial two-hour session as a planning allowance; actual time is unknown and taking longer is fine.

## Step 1 — Extract and open the pack

Download `six_case_calibration.zip`, right-click it in Windows, choose **Extract All**, then open the extracted folder. Double-click **START_HERE.html** to read these instructions in Chrome or Edge. Leave **OPEN_AFTER_FIRST_ATTEMPT.html** closed for now: it contains the provisional discussion answers for these six cases only.

The six rows are P001, P002, P015, P016, P018 and P023. The 24 other pilot cases are not in this training worksheet. Do not open the existing full draft-label file, model demo, manual baseline outputs or full pilot bundle while practicing. If you already saw answers, that is not a failure; record the exposure honestly.

## Step 2 — Assign IDs and open separate worksheets

Call one student **R1** and the other **R2**. R1 uses `calibration_R1.csv`; R2 uses `calibration_R2.csv`. Each student should fill their own sheet. Do not split the six cases three each. Both students should practice all six.

For the free Google Sheets route:

1. Open https://sheets.google.com and create a blank spreadsheet.
2. Rename it `calibration_R1` or `calibration_R2`.
3. Choose **File → Import → Upload**, then select your CSV from the extracted folder.
4. Select **Replace spreadsheet**, comma separation (or automatic detection) and, if shown, turn off **Convert text to numbers, dates, and formulas**. Click **Import data**. Use the account approved for your university work if applicable.
5. Choose **View → Freeze → 1 row** so the headings stay visible. Use **Format → Wrapping → Wrap** if text is cut off. Scroll sideways to see the answer columns.

If you already use Excel, choose **Data → From Text/CSV**, select the file, UTF-8 and comma separation. Keep date/ID columns as text where possible. You do not need to use both programs.

Leave the supplied claim, policy, cutoff, period and packet columns unchanged. Start typing in the blank answer columns. Use aliases, not names, email addresses or phone numbers.

## Step 3 — Learn these terms before opening a filing

| Term | Meaning for this exercise |
|---|---|
| Claim | The sentence we are checking. It may be right, wrong or unsettled under the selected interpretation. |
| Metric | The exact thing measured. Net income and income from continuing operations are different rows. |
| Fiscal year | The company's reporting year. It may start/end on dates different from January 1/December 31. Use the supplied exact period. |
| Filing | A company's document filed with the US Securities and Exchange Commission (SEC). |
| 10-K | An annual report. |
| 10-K/A | An amendment to an annual report. The letter A does not by itself prove that a particular number was corrected. |
| 8-K Item 4.02 | A disclosure about non-reliance on specified earlier statements or related audit/review material. Read what it actually covers. |
| Original as filed | What the named original document reported, even if a later document corrects it. |
| Corrected named | What the named later report's current corrected column says, not its "previously reported" column. |
| As known in the packet | Use only eligible documents in the supplied packet and honor applicable withdrawals/corrections. |
| Cutoff | Our evaluation date. A document is eligible only if its official filing date is strictly earlier than this date. This conservative rule is a project convention. |
| Non-reliance | The notice says specified earlier statements should no longer be relied upon. It does not by itself give the replacement number or prove every old line item wrong. |
| Packet | The fixed set of source documents for a case, such as SP0+SPW+SP1. We are not claiming this is everything the market knew. |

Dates use **YYYY-MM-DD**: `2023-10-25` means 25 October 2023. Use the SEC **Filing Date**, not a date inside the filename or the board/audit committee's meeting date. The source-links page provides filing-index links so you can check that field.

Parentheses often mark negative amounts: `(12,300)` is negative 12,300 in that table's units. A claim saying "a loss of 12.3 million" describes the positive loss magnitude. Always read the row and units together.

## Step 4 — Learn the three verdicts

| Enter | Use it when |
|---|---|
| S | The eligible source evidence supports the claim under the specified policy. |
| C | The eligible source evidence positively conflicts with the claim under that policy. |
| U | The permitted evidence/interpretations do not establish either support or contradiction. |

**U does not mean "I do not understand."** If you cannot open a source, cannot locate the row or do not understand a concept, leave `first_attempt_label` blank and explain the problem in `help_needed`. This keeps a research label separate from a reviewer's difficulty.

Toy example, unrelated to our companies: a report displays 12,300 in **USD thousands**. That is 12,300,000 dollars, or 12.3 million dollars. To convert thousands into millions, divide the displayed number by 1,000. A report displaying 12.3 in **USD millions** already uses millions; do not divide it again.

## Step 5 — Use the same routine for every case

1. Read the full claim, exact metric, reporting period, policy and cutoff. Say aloud which question the policy asks before trying to answer it.
2. Open the [source-links page](SOURCE_LINKS.html). Use the source IDs in the case instructions below. Use **Ctrl+F** to search within the filing and **Enter** to cycle through repeated matches.
3. Check the statement/note heading, exact row caption, year column and units. A matching number somewhere else in the report is insufficient. Keep a screenshot locally if it helps, but also record the locator in text.
4. Check the official filing date against the cutoff. For original/corrected cases, use the named report specified below; for as-known cases, list which packet sources are eligible.
5. Fill your own first-attempt answer and reason. Do not ask an AI tool to decide the label and do not view the answer key yet. Asking your partner how to navigate the browser is fine; keep verdicts separate until discussion.
6. Stop the case timer and record actual minutes. Include source reading done during that case. Record shared source reading done outside case timers and group discussion separately in `session_log.csv`; do not count the same time twice.

## Step 6 — Work through these six cases, in this order

### Case 1: P001 — read an original report

- Company: Plug Power. Period: 2019-01-01 through 2019-12-31.
- Claim: reported **net loss attributable to the Company** was USD 85.465 million.
- Policy: `original_as_filed`. Cutoff: 2021-05-15.
- Open **P19**. Find **Consolidated Statements of Operations**, the 2019 column and the row **Net loss attributable to the Company**. Read the units above the table.
- Do not substitute **net loss attributable to common stockholders**; that is a different caption.
- Write the number exactly as the table displays it, including parentheses and units. Convert it to millions if needed, then decide whether it matches the claim under this policy.

### Case 2: P002 — keep the claim, change the document policy

- The claim, reporting period and cutoff are the same as P001. The policy is now `corrected_named`.
- Open **P20**, the later annual report. Find **Note 2 — Restatement of Previously Issued Consolidated Financial Statements** and the 2019 reconciliation for the same net-loss row.
- Identify **As Previously Reported**, **Cumulative Adjustments** and **As Restated**. Read the current corrected column for the verdict. Do not choose the old column just because its number matches the claim.
- Record the original and corrected displayed amounts and units. State which column controls this question.

### Case 3: P015 — apply a historical cutoff

- Company: SunPower. Fiscal-2022 interval: 2022-01-03 through 2023-01-01.
- Claim: net income **attributable to stockholders** was USD 56.037 million according to the active authoritative statements in the packet.
- Policy: `as_known_packet`. Cutoff: **2023-10-18**.
- Open the source-links page and check filing dates for **SP0**, **SPW** and **SP1**. List which were filed strictly before the cutoff. Do this before deciding the answer.
- In an eligible numerical report, find **Consolidated Statements of Operations** and **Net income (loss) attributable to stockholders**, fiscal year ended January 1, 2023. Do not substitute the separate **Net income** row above attribution to noncontrolling interests.
- Record the value, units, eligible source IDs and reason. A document visible to you today can still be ineligible for this historical question.

### Case 4: P016 — same claim, later cutoff

- Same SunPower claim and policy as P015. The cutoff is now **2023-10-25**.
- Recheck eligibility for SP0, SPW and SP1.
- Open **SPW**, find **Item 4.02** and the phrase **should no longer be relied upon**. Read the surrounding sentences to identify which annual statements it covers.
- Check whether an eligible replacement amount for this annual row is supplied in the packet. Do not use a later report merely because you can open it today.
- Record why a withdrawal notice matters. Avoid assuming that the notice alone supplies the corrected numerical value.

### Case 5: P018 — distinguish a displayed value from exactness

- Same SunPower fiscal interval. Policy: `corrected_named`. Cutoff: **2023-12-19**.
- Claim: the **exact unrounded** net income attributable to stockholders was **USD 42,849,000 with zero rounding uncertainty**.
- Open **SP1**. Find **Note 2 — Summary of Restatement**, the **Consolidated Statements of Operations** reconciliation, printed pages 88–89. Browser page numbering may differ. Use the stockholder-attributable row and corrected fiscal-2022 column.
- Read the table's unit/precision statement. Record both the displayed amount and its conversion into dollars.
- Decide whether a rounded report establishes the stronger claim of exact unrounded equality. Our protocol treats displayed rounding as uncertainty; copying digits into dollars does not remove it.

### Case 6: P023 — reject a wrong-metric match

- Company: Tupperware. Period: 2020-12-27 through 2021-12-25.
- Claim: reported **total net income** for fiscal 2021 was USD **151.0 million**.
- Policy: `corrected_named`. Cutoff: **2023-10-14**.
- Open **T1**. Find **Note 22 — Restated Previously Issued 2021 and 2020 Financial Statements**, the statement of income/loss for the year ended December 25, 2021, printed page 114.
- Read the **As Restated** column for both **Income from continuing operations** and **Net income**. Record the two row captions and amounts separately.
- Choose the row that the claim actually asks about. Finding the claimed number in a different row does not support the claim.

If Ctrl+F fails, search a shorter phrase such as `attributable`, `Restatement`, `4.02` or `continuing operations`. If the SEC link fails, try its filing-index link and then open the main 10-K/10-K/A/8-K document. If both fail, record the source ID in `help_needed` and stop that case; do not replace it with a search-engine snippet.

## Step 7 — Know what to type in the answer columns

| Column | What you enter |
|---|---|
| `prior_answer_exposure` | `yes`, `no` or `unsure`: had you already seen this case's proposed answer or demo output? |
| `first_attempt_label` | Your initial S/C/U, or blank if you cannot complete the review. |
| `source_ids_and_locator` | Source ID plus note/statement, exact row, year column and preferably printed page. A URL alone is insufficient. |
| `source_value_and_units` | The number exactly as displayed, its unit and any conversion you used. For a notice, record its relevant scope instead of inventing a number. |
| `eligible_source_ids` | Packet sources filed strictly before the cutoff. This list can include a withdrawn report; eligibility by date is different from active authority. Explain the policy's final source choice in your reason. |
| `your_reason` | One or two sentences connecting policy, date, row and value to your verdict. |
| `case_minutes` | Actual time spent on this case. An estimate is acceptable if marked as an estimate in `help_needed`. |
| `help_needed` | What blocked you or what you are unsure about. Leave empty if nothing did. |
| `label_after_discussion` | Fill only after Step 9. Do not overwrite the first attempt. |
| `what_changed_after_discussion` | Record the correction or explain why you retained your initial answer. |

Use this reason template: **"The policy asks for ____. Source ____ was/was not eligible because ____. The relevant row/notice says ____. Therefore my answer is ____."** You may adapt it; do not fill gaps with assumptions.

## Step 8 — Save both first attempts before discussion

In Google Sheets choose **File → Download → Comma Separated Values (.csv, current sheet)**. Rename the downloads `calibration_R1_first.csv` and `calibration_R2_first.csv`. In Excel use **Save As → CSV UTF-8**. Keep these files unchanged. If only one student is available, save that student's file and record that this was solo practice; do not create a second reviewer identity.

## Step 9 — Discuss, then open the provisional answer key

Compare your first attempts case by case. For each disagreement, each student must show the source, year column, unit and cutoff reasoning. Then open **OPEN_AFTER_FIRST_ATTEMPT.html**. It contains proposed discussion answers with explanations, not independently certified gold labels.

If you change your mind, enter the new verdict in `label_after_discussion` and explain the change. Keep `first_attempt_label` unchanged. If the key seems wrong or the source is ambiguous, preserve your objection and locator; do not change your answer just to match it. An unresolved issue remains an issue for review, not a forced agreement.

Save updated copies as `calibration_R1_after_discussion.csv` and `calibration_R2_after_discussion.csv`. Fill `session_log.csv` with actual shared reading/discussion time. Record any interruptions.

## Step 10 — Return the work and pause

Upload both first-attempt files, both after-discussion files and the session log in this chat. Remove any personal details first. If you are working alone, return only your files and say so. Tell me which case/source was hardest to locate.

We will inspect missing evidence and recurring mistakes before the remaining 24 cases. You are ready to proceed when each student can independently explain the source choice, date eligibility, row/units and reason for the six verdicts, and any unresolved issue is documented. Matching six letters alone is not readiness. This is a proposed training criterion, not a validated competence certification.

During the later review, **both students review all 24 remaining cases separately**, without the proposed key or each other's answers. Record prior exposure. Calibration uses some of the same issuers and documents, so the remaining cases are still pilot/development material, not a clean held-out publication test. Never report these six discussed practice cases as blinded inter-annotator agreement or model accuracy.
