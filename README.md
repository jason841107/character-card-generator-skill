# Character Card Generator

把一张或多张成年人物主图扩展成高清、多页、可复用的角色参考卡。

## 核心能力

- 一张主图对应一个身份，同一卡内锁定脸、发型、年龄感和身材比例。
- 服装场景保持同一人物，同时改变表情、视线、脸部角度、手部动作和姿态。
- 默认服装页采用完整的年轻时装编辑系统：九套按三套旗袍或旗袍衍生、三套连衣裙、三套叠穿造型组织；同时强制加入宽松下装、外套造型、动态细节、运动与精致材质碰撞以及真实街头场景，限制长窄裙和传统高跟鞋的重复。
- 不同角色卡重新建立身份锚点，避免跨卡串脸。
- 图片主体无字生成，中文、编号和标签由本地 ImageMagick 模板排版。
- 默认输出完整三页高清卡，尺寸为 3072×4608 PNG。

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
使用 $character-card-generator 根据这张主图生成完整三页高清角色卡。
```

还可以指定风格包、页数和清晰度，例如：

```text
使用 $character-card-generator 生成新中式旗袍和都市连衣裙为主的服装扩展页，高清档。
```

## 清晰度

- `standard`：2048×3072，整页生成。
- `hd`：3072×4608，分组生成，默认。
- `ultra`：4096×6144，主要分镜独立生成。

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
