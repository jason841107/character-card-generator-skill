# Character Card Generator

把一张或多张成年人物主图扩展成两页高清、可复用的角色参考卡。

## 效果示例：林澄

同一人物贯穿角色简介、人物设定、细节与五套服装情景。点击图片可查看完整 PNG。

### 第 1 页 · 人物简介、设定与表情

<p align="center">
  <a href="examples/lin-cheng/page1-profile-v2.png"><img src="examples/lin-cheng/page1-profile-v2.png" alt="林澄角色卡第 1 页：人物简介、设定与表情" width="76%"></a>
</p>

### 第 2 页 · 细节与场景

<p align="center">
  <a href="examples/lin-cheng/page2-details-scenes-v2.png"><img src="examples/lin-cheng/page2-details-scenes-v2.png" alt="林澄角色卡第 2 页：细节与五套服装情景" width="76%"></a>
</p>

示例第一页为 3072×5517 PNG，第二页为 3072×4608 PNG。最终画布按拼接内容确定。

## 核心能力

- 一张主图对应一个身份，同一卡内锁定脸、发型、年龄感和身材比例。
- 服装场景保持同一人物，同时改变表情、视线、脸部角度、手部动作和姿态。
- 第二页五套造型默认包含两套旗袍或旗袍衍生、两套连衣裙和一套叠穿造型，并加入宽松下装、外套、动态细节、材质碰撞和真实街头场景。
- 不同角色卡重新建立身份锚点，避免跨卡串脸。
- 图片主体无字生成，中文标题和必要标签由本地 ImageMagick 模板排版；默认不添加数字角标。
- 第一页包含独立的两三句虚构人物简介和结构化设定；第二页只输出纯图片拼接，不添加页眉、页码、标题、标签或说明。
- 两页均按源图比例和实际拼接内容确定画布；清晰度档位不强制固定页面比例或高度，也不拉伸单图。
- 默认交付完整两页角色卡，不包含技术设定板或第三页服装扩展。

## 安装

将仓库复制到 Codex Skills 目录：

```bash
git clone https://github.com/jason841107/character-card-generator-skill.git \
  ~/.codex/skills/character-card-generator
```

公开仓库无需额外的 GitHub 访问权限。

## 使用

在 Codex 中附上人物主图，并输入：

```text
使用 $character-card-generator 根据这张主图生成完整两页高清角色卡，并附上可复制的人物简介。
```

还可以指定风格包和清晰度，例如：

```text
使用 $character-card-generator 生成新中式旗袍和都市连衣裙为主的两页角色卡，高清档。
```

## 清晰度

- `standard`：标准图像细节。
- `hd`：高清图像细节，默认。
- `ultra`：最高图像细节，分组生成主要面板。

清晰度档位影响素材细节，最终画布尺寸仍由拼接构图决定。

## 目录

```text
SKILL.md
agents/openai.yaml
references/
assets/layouts/
```

人物姓名、年龄、职业、性格和生活经历均作为虚构创作设定。性感或修身造型只用于明确的成年人，并保持完整穿着。

## 许可证

本项目采用 [MIT License](LICENSE)。
