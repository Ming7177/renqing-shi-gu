# 人情世故

![陈汉生](skill/assets/chen-hansheng.png)

一个把《我真没想重生啊》中陈汉升的人情世故处事方式，蒸馏成可复用 Codex skill 的开源项目。

这个项目不提供小说原文，不提供长段摘录，也不试图替代阅读原书。这里开源的是阅读后的处事模型、场景规则、说话方式和测试题。

## 核心模型

陈汉升不是简单的“会说话”。他的核心是现实判断：

1. 先看场域权力
2. 再定自己的身份
3. 再稳住局面
4. 再给对方台阶
5. 最后把事办成

## 目录

```text
skill/
  SKILL.md
  agents/openai.yaml
  references/analysis.md
  references/rules.md
  references/speaking.md
examples/
  campus-registration.md
  dinner-toast.md
  slow-approval-flow.md
evals/
  scenario-tests.md
docs/
  distillation-method.md
```

## 安装

把 `skill/` 目录复制到你的 Codex skills 目录下，并改名为：

```text
人情世故
```

例如 Windows：

```powershell
Copy-Item -Recurse .\skill D:\.codex\skills\人情世故
```

然后重启 Codex，让技能重新扫描。

## 使用

触发名：

```text
$人情世故
```

示例：

```text
用 $人情世故 分析这个场景：我创业初期要去地推，商家不信任我，我该怎么开口？
```

## 触发条件

适合：

- 分析现实人情世故场景
- 处理饭局、求人、拒绝、亲戚局、同学局、商务谈判
- 判断公开场合的聚光灯该接还是该灭
- 把尴尬转成台阶、面子或可执行动作
- 用场景题反复校准 skill

不适合：

- 复述小说剧情
- 输出小说正文或长段摘录
- 把角色当成纯善良、纯坏人或万能油滑话术模板

## 版权说明

本仓库只包含原创分析、规则和示例场景，不包含小说原文或长段摘录。请勿提交小说全文、章节摘录或可替代阅读原书的内容。
