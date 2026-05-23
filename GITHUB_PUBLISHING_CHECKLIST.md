# GitHub Publishing Checklist

发布 `resume-rewriter-cn` 前，建议按下面清单检查。

## 必备文件

- [ ] `README.md`
- [ ] `.gitignore`
- [ ] `GITHUB_PUBLISHING_CHECKLIST.md`
- [ ] `resume-rewriter-cn/SKILL.md`
- [ ] `resume-rewriter-cn/agents/openai.yaml`
- [ ] `examples/anonymized-cases.md`
- [ ] `LICENSE`

## 推荐仓库结构

```text
resume-rewriter-cn/
  SKILL.md
  agents/
    openai.yaml

examples/
  anonymized-cases.md

README.md
GITHUB_PUBLISHING_CHECKLIST.md
.gitignore
LICENSE
```

## 不要上传

- 真实简历文件：`.docx`、`.pdf`、`.jpg`、`.png`
- 生成预览文件：`resume_*_preview.html`
- 本地构建脚本：`build_resume_docx*.py`
- Mac 临时文件：`.DS_Store`
- WPS/Word 临时文件：`.~*`、`~$*`
- 带姓名、手机号、邮箱、照片、学校、公司敏感信息的文件

## 发布前检查

- [ ] README 能清楚说明这个 Skill 的核心价值。
- [ ] README 明确体现“HR 视角”和“隐藏技能挖掘”。
- [ ] 示例全部脱敏或虚构。
- [ ] Skill 文件没有真实候选人信息。
- [ ] `.gitignore` 已上传，避免后续误提交隐私文件。
- [ ] GitHub 仓库 Description 已填写。
- [ ] License 已选择，推荐 MIT。

## 推荐仓库简介

```text
A Codex Skill for Chinese resume rewriting, JD alignment, hidden value mining, one-page layout, and HR-style review.
```

## 推荐 Topics

```text
codex-skill
resume
chinese-resume
job-search
career
jd-alignment
hr
prompt-engineering
```

## 首次提交信息

```text
Add Resume Rewriter CN skill
```
