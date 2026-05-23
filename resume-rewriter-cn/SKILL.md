---
name: resume-rewriter-cn
description: 中文简历诊断、优化、重写和复盘工作流。适用于用户上传图片、PDF、Word 或文字版中文简历后，需要按目标岗位、JD、行业或企业要求，提炼任职优势，重构一页纸简历，优化经历表达，检查排版，输出可编辑 Word/HTML 预览，并给出简洁修改说明的场景。Use for Chinese resume rewriting, JD alignment, one-page resume polishing, fresh graduate resume optimization, resume layout review, and candidate-facing revision summaries.
---

# Resume Rewriter CN

## Purpose

Turn a Chinese resume into a focused, truthful, one-page resume for one target job.

Use an employer/HR perspective: every retained item must explain why the candidate fits the target role. Do not simply polish the original wording or preserve the original order.

Core advantage: discover hidden value in the original resume. When the candidate wrote only a title, result, or vague duty, infer the likely job-recognized process, tools, objects, deliverables, and transferable abilities from the original facts and common role workflows. Keep the inference conservative; never invent results, numbers, awards, companies, clients, or tools that are not supported.

## When To Use

Use this skill when the user asks to:

- Rewrite, polish, diagnose, or optimize a Chinese resume.
- Convert an image/PDF/Word/text resume into an editable Word or HTML preview.
- Align a resume with a JD, target company, industry, campus recruitment role, or early-career role.
- Review a generated resume for layout, HR readability, role fit, or wording quality.

## Input Handling

1. Extract candidate facts from the source file or screenshot.
2. Identify the single target job. If multiple targets appear, choose the most likely one from context and avoid writing multiple job directions in one resume.
3. If a JD, target company, or target industry is provided, align wording, evidence order, and visual tone to it.
4. If the user asks for company adaptation, search official sources first when network access is available: company site, recruitment page, official account, or user-provided assets. Use search results only for language, keywords, visual tone, brand color, and verified logo. Do not turn external information into candidate facts.
5. If personal data is hidden or missing, use placeholders such as `【姓名】`, `【手机号】`, `【邮箱】`, `【学校名称】`.

## Operating Principles

- Truth first: do not fabricate outcomes, quantities, rankings, tools, awards, or company details.
- One resume, one job: all modules serve the same target role.
- Evidence before adjectives: prefer concrete facts over “优秀、良好、较强、显著提升”.
- Importance before chronology: order modules and experiences by role relevance, not by the source resume sequence.
- Hidden value mining is allowed only for process/tool/object/deliverable inference, not for unsupported results.
- Formal resume text must not include internal notes such as “建议补充、待完善、可补充”.

## Workflow

### 1. Diagnose

Check the source resume from four angles:

- Structure: one-page fit, section hierarchy, photo space, table traces, spacing balance, and bullet consistency.
- Content: irrelevant personal data, self-evaluation, slogan language, duplicated duties, vague descriptions, and job-description-style wording.
- Match: map major, courses, certificates, internships, projects, campus roles, military service, honors, and tools to the target job.
- Gaps: record useful missing data for the delivery note, such as candidate counts, interview invites, service volume, activity size, production volume, project deliverables, or measurable workload.

### 2. Classify Evidence

Use this relevance matrix before deciding where content goes:

| Evidence type | Rule | Treatment |
| --- | --- | --- |
| Strong role evidence | Directly proves target-role ability, workflow, tool, certificate, or professional practice | Expand and move forward |
| Transferable evidence | Not role-specific, but proves execution, communication, service, discipline, coordination, or documentation | Translate into role language and keep concise |
| Weak evidence | Only loosely related or repeats a stronger section | Compress to one line, merge, or move to the end |
| Irrelevant evidence | Does not support the target role and consumes space | Delete |
| Mixed evidence | One activity contains both strong and weak value | Split into separate modules before rewriting |

Examples:

- Nursing: clinical rotation, nursing operations, health education, blood pressure monitoring are strong; etiquette team is transferable; generic training camp is weak.
- HR: recruitment posting, screening, interview scheduling, candidate communication, HR data ledger, and employee development are strong; student union roles are transferable.
- Mechanical: production-line practice, quality inspection, CNC training, SolidWorks modeling, drawings, BOM, tolerance, and assembly are strong; general volunteer service is usually weak.

### 3. Reorder Modules

Default order:

1. Personal information
2. Job target and key advantages
3. Education background
4. Strong role-related internships/projects/practice
5. Role-relevant certificates and tools
6. Transferable campus/organization experience
7. Honors or supplementary information

Adjust the order when evidence demands it:

- If a certificate or qualification is a hard requirement, surface it in key advantages and place `证书与工具` before weaker experiences.
- If formal internship/project evidence is strong, place it before school training or campus roles.
- If the candidate has military service, student leader experience, or major honors that creates real differentiation, place the fact in key advantages and translate it in the relevant experience section.

## Module Specification

| Module | Keep | Remove or avoid |
| --- | --- | --- |
| Personal information | Name, target job, phone, email, one-inch photo/photo slot | Major, age, native place, political status, self-description, unrelated identity labels |
| Key advantages | 3 bullets, maximum 4; facts only; one line where possible | Labels such as “专业匹配、稀缺经历、数据工具、组织协调” |
| Education | School, time, major, degree, GPA/ranking if strong, core courses, study-related honors | Split fields like “主修课程/拓展课程”; low-value course lists |
| Internships/projects/practice | Role-relevant process, tools, objects, deliverables, standards, and outcomes if verified | Unsupported numbers, inflated senior wording, repeated generic duties |
| Campus/organization | Only transferable value: execution, coordination, documentation, service, discipline, communication | Long activity descriptions unrelated to the job |
| Certificates/tools | Hard certificates and role-relevant tools | Re-summarizing abilities already shown in experiences |
| Self-evaluation | Delete or absorb into evidence | Standalone self-evaluation section |

## Key Advantages

This section is the first-screen hook for HR. Write concrete facts, not summaries.

Priority:

1. Hard fit: major, certificate, qualification, core tool, core course.
2. Differentiator: military service, student leader role, strong award, well-known platform/company.
3. Practice: internship months, project/practice type, service object, workflow coverage.

Good:

```text
• 人力资源管理本科，持企业人力资源管理师证。
• 2 年中国人民解放军某部服役经历，曾任瞄准手。
• 9 个月人事助理实践，覆盖招聘发布、初筛、邀约、台账维护。
```

Avoid:

```text
• 专业匹配：系统学习人力资源管理相关课程，具备扎实模块基础。
• 稀缺经历：拥有军队服役经历，组织纪律性和抗压能力较强。
```

## Hidden Value Mining

When source text is vague, enrich it by adding likely process and tools only if they are consistent with the role and original facts.

Allowed:

- `负责招聘支持` -> `跟进候选人沟通、面试邀约和招聘进度，维护招聘台账`
- `参与质量检验` -> `依据检验标准检查外观、孔位、配合完整性，记录毛刺、碰伤、变形等缺陷`
- `完成建模项目` -> `完成零件建模、装配检查、工程图/爆炸图/BOM 输出`

Not allowed:

- Add candidate counts, efficiency gains, conversion rates, awards, customer names, or performance results without source support.
- Claim a tool was used when neither the source nor the role context supports it.

Put missing-but-useful data in the delivery note, not in the resume body.

## Writing Rules

- Use the structure `action + object/process + method/tool + deliverable/result`.
- Prefer specific verbs: 负责、整理、跟进、对接、统计、统筹、核对、记录、复盘、输出.
- Avoid starting every bullet with `参与、协助、支持`; vary verbs according to real responsibility.
- Keep early-career language credible. Do not make a student sound like a senior expert.
- Do not use internet buzzwords, slogans, exaggerated adjectives, or obvious AI phrasing.
- Translate special experiences into workplace value:
  - Military service: discipline, task execution, teamwork, complex-environment response, procedure compliance, field execution.
  - Student organization: coordination, task allocation, event execution, cross-team communication, documentation, review.
  - Volunteer/service work: service awareness, communication, patience, public-facing delivery, professional relevance if applicable.

## Adaptive Style

- Role style: medical resumes emphasize procedure, nursing operations, patient communication, documentation, handover, emergency support; HR resumes emphasize recruitment workflow, candidate communication, data ledger, coordination; technical resumes emphasize project, tool, system, standard, and deliverable.
- Industry style: medical, state-owned, education, finance, and public-sector roles should be steady and standardized; internet, operations, and design roles may be cleaner and lighter; technical/manufacturing roles should be factual and tool/process-oriented.
- Company style: when a target company is known, use official sources to align keywords, visual tone, brand color, and logo. Logo use must be subtle, verified, and non-distracting.
- Reference style: when searching excellent resume examples, learn only structure, section order, language density, and layout. Never copy content or invent candidate facts.

## Layout Rules

- Default to a one-page vertical Chinese resume.
- Use a clear top-down reading path. Avoid two-column body layouts unless space requires it and readability remains clear.
- Personal information contains only name, target job, phone, email, and photo/photo slot.
- One-inch photo slot should be vertical, about 2.5cm x 3.5cm, placed at top right. Do not make it a horizontal strip.
- Avoid a large blank header caused by photo height. Put key advantages close to the name/contact area when useful.
- Key advantages should be 3 concise vertical bullets by default.
- Avoid visible table grids, dotted layout lines, heavy color blocks, and large pale title bars.
- Use restrained color based on role/company style. A resume should not look like a promotional page.
- Page height should be used about 80%-95%. If bottom whitespace is too large, adjust font size, line height, section spacing, margins, and verified content density.

## Output Protocol

When generating a resume, provide:

1. Editable output, preferably Word when requested, or HTML preview when layout review is needed.
2. A concise candidate-facing explanation in second person.
3. A short list of data worth confirming, only if important.
4. A brief comparison or review when the user asks to compare versions.

Candidate-facing explanation template:

```text
你的简历主要问题是：[1-2句说明结构、重点或岗位匹配问题]。我按照[目标岗位/JD/行业风格]，帮你重新梳理了个人信息、任职优势、教育背景和经历模块，并把经历改成更贴近岗位要求的表达；重点强化了[1-2个关键优化点]。有些结果数据还需要你补充确认，建议优先补充[具体数据类型]。仅供参考，祝求职顺利。
```

Keep the explanation practical and concise.

## Validation Checklist

Before delivery, revise the output through two reviews.

### Layout Review

- One page is complete and printable.
- Content height uses about 80%-95% of the page.
- Top and bottom spacing are balanced.
- Key advantages are easy to scan and visually aligned.
- Photo slot is vertical one-inch ratio and does not create empty header space.
- Font size, line height, title spacing, margins, bullets, and colors are consistent.
- There are no visible table grids, text overlaps, excessive decorations, or awkward blank areas.

### HR Review

- The resume serves only one target job.
- Personal information contains only name, target job, phone, email, and photo/photo slot.
- Key advantages are short, factual, and memorable.
- Strong role evidence appears before weak or generic evidence.
- Hard certificates/tools are surfaced when they are role requirements or strong proof.
- Hidden value has been mined through process, tools, objects, deliverables, and transferable abilities.
- No unsupported numbers, outcomes, tools, company details, or awards have been added.
- Certificates/tools are hard information and do not repeat descriptive content from experiences.
- The language and visual style fit the target role, JD, industry, or company.
- Missing data is mentioned only in the delivery note, not in the resume body.
