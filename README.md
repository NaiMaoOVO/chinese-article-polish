# 中文文章润色 Skill

一个可反复调用的中文文章编辑技能：在尽量贴近原稿的前提下，改善表达自然度、句式与段落节奏，并清理没有信息价值的防御性措辞。

适用于随笔、公众号文章、学术文本、营销文案、新闻稿、工作报告和技术说明。专业表达、证据边界、必要限定和作者真实立场都会保留。

## 安装到 Codex

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/NaiMaoOVO/chinese-article-polish.git ~/.agents/skills/chinese-article-polish
```

也可以下载仓库 ZIP，将整个文件夹复制到 `~/.agents/skills/chinese-article-polish/`。加载技能后可直接这样调用：

```text
$chinese-article-polish 请轻度润色，保留原意和篇幅，不补造经历或数据。[粘贴文章]
```

修改后，Codex 通常需要重新加载技能目录才能识别新技能。

## 编辑约定

- 默认轻改；体裁、受众、发布场景和语气可以补充，但不是开始润色的前提。
- 不随机替换词语、不故意打乱逻辑，也不编造个人经验、案例、数字或来源。
- 删除无依据的自我削弱，同时保留必要的方法限制、范围条件和不确定性。
- 长文完整处理；用户要求扩写或结构重组时再扩大改动范围。

## 来源与许可

防御性写作部分参考并改写自 [Kiterlin/anti-defensive-writing](https://github.com/Kiterlin/anti-defensive-writing)。其 MIT 许可文本保存在 `LICENSES/`。本仓库采用 MIT License。
