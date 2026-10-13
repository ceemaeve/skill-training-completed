# Team tracks

The sprints are the same for everyone. What changes is which parts a person does and whether they sit exams.

Every track starts with C1, Claude basics (2 weeks, see SPRINTS.md). The weeks below include it.

## Track F: Foundations (A+, Network+)

For people new to IT, or moving into IT from another kind of work.

- Do F1, F2 and F3 (see SPRINTS.md).
- Sit A+ Core 1 after F2, A+ Core 2 after F3, then Network+.
- About 16 weeks at 8 hours per week.
- Then pick B, C or D, or carry on with S0 as Track E does.

## Track G: Networking (CCNA)

For network administration, network operations center (NOC) and network support roles.

- Do F2, S0, S1 and N1 (see SPRINTS.md). S0 builds the lab that S1 needs.
- Sit CCNA after N1. Network+ after F2 is optional.
- About 17 weeks at 8 hours per week.
- New to IT? Do Track F first, then go straight to S0.

## Track H: AWS (Solutions Architect – Associate)

For cloud jobs on AWS.

- Do S0, S1, S9 and A1 (see SPRINTS.md). S0 builds the lab that S1 needs.
- In S9, skip lab 3 (it needs the file server from S5) and lab 5 (Azure cost alerts; A1 lab 1 does the AWS version). In lab 2, use AWS as the second cloud.
- Sit AWS Solutions Architect – Associate after A1.
- About 16 weeks at 8 hours per week.
- New to IT? Do Track F first, then go straight to S0.

## Track I: Claude

For anyone who wants to use Claude well in IT work, on its own or next to another track.

- Do C1, S0, C2 and C3 (see SPRINTS.md). S0 teaches the command line and Git that C2 needs.
- No exam. Claude Academy courses give completion certificates; the "prove it" deliverables are your record.
- C2 needs a paid Claude plan or an Anthropic Console account. C1 and C3 work on the free plan.
- About 8 weeks at 8 hours per week.
- On another track already? Add C2 and C3 after S0 (4 weeks).

## Track A: Skills only (no exams)

For people who want the capability without the certificate.

- Do every sprint's labs and its "prove it" deliverable.
- Skip the exam gates and their review weeks. That saves about 10 weeks.
- New to IT? Do the F1 to F3 labs first, still without the exams.
- Skip S9 (cloud architecture) and S11 (security operations) if they don't apply to the role, and jump to S13 with a smaller capstone.
- About 46 weeks at 8 hours per week (40 if you skip S9 and S11).
- Assessment is by peer review of the deliverables using the rubric in ASSESSMENT.md.

## Track B: Microsoft (AZ-802, AZ-104)

- Do S0 through S8, including the Linux lanes at reduced depth (one lab per sprint is enough).
- Sit AZ-802 after S7 and AZ-104 after S8.
- About 31 weeks at 8 hours per week.

## Track C: Linux (Linux+, LPIC-1, LPIC-2, LPIC-3)

- Do S0, S1, S2, S5, S6, S7 and S8 with the Linux lane as the main lab and the Windows lab as reference.
- Then S10, S12 and the capstone (S13).
- Sit Linux+ and LPIC-1 after S10, LPIC-2 after S12, LPIC-3 after the capstone.
- About 40 weeks at 8 hours per week.

## Track D: Security-focused

- Do S0 through S2, S6, S7, S9, S11 and the capstone with a security emphasis. S9 adds cloud security context.
- Sit Cloud+ after S9 and Security+ after S11.
- About 28 weeks at 8 hours per week (24 if you skip S9 and Cloud+).

## Track E: Everyone

- Every sprint except N1 (Cisco), A1 (AWS), C2 and C3 (Claude): C1, F1 to F3, then S0 to S13, with all their exam gates, A+ and Network+ included. About 70 weeks at 8 hours per week. CCNA, AWS and the later Claude sprints are not in Track E; add N1 and its gate (6 weeks) for CCNA, A1 and its gate (6 weeks) for AWS, or C2 and C3 (4 weeks) for more Claude.
- Already past the basics? Do C1, then start at S0 and skip the Foundations block (56 weeks).

## Choosing

| If your role is mostly... | Start with track |
| --- | --- |
| New to IT, or help desk and desktop support | F, then B, C or D |
| Network administration or a NOC | G (Track F first if new to IT) |
| Windows and Microsoft 365 administration | B |
| Linux server administration | C |
| Cloud engineering on Azure | B, then S9 and Cloud+ |
| Cloud engineering on AWS | H |
| Security or compliance | D |
| A mix, or growing into a senior generalist | E |
| Not interested in exams | A, with the other track's sprints as a guide |
| Using Claude well in IT work | I, on its own or next to another track |

## Working as a team

- Pair up on the fault lab (S7) and the tabletop (S11): one breaks, one fixes.
- Review each other's "prove it" deliverables before anyone moves on.
- Keep deliverables in your team repo under `deliverables/<name>/<sprint>/`.
- Hold a 20-minute demo at the end of each sprint, one person presenting.
