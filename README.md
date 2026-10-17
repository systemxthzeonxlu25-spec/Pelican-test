# 🐦 Pelican-test

> 每出一代新模型，就让它画一只骑自行车的鹈鹕。

用同一道题测试不同 AI 模型的前端 / SVG / 动画能力：**「画一只骑自行车的鹈鹕」**。
这题看着简单，其实挺刁钻——鹈鹕的身体结构、自行车的几何关系、腿怎么踩踏板，模型一不小心就会画出一只长在车架里的鸟。

每个模型的作品放在**独立分支**里，`main` 只放说明和索引，方便横向对比。

## 📂 分支索引

| 分支 | 模型 | 日期 | 形式 | 备注 |
| --- | --- | --- | --- | --- |
| [`DeepSeek-v4.1-1017`](../../tree/DeepSeek-v4.1-1017) | DeepSeek v4.1 | 2026-10-17 | 单文件 HTML（SVG + CSS/JS 动画） | 海岸线杂志封面风，踏板带腿部 IK |

## 🧭 分支约定

- **命名**：`模型名-版本-MMDD`，例如 `DeepSeek-v4.1-1017`
- **入口**：每个分支根目录放 `index.html`，浏览器直接打开就能看
- **截图**：附一张 `preview.png`，不想开浏览器也能一眼对比
- **说明**：分支自己的 `README.md` 写清楚模型、提示词和亮点 / 翻车点
- **原样提交**：尽量保留模型的原始输出，不手动修图，不然对比就没意义了

## ➕ 新增一个模型

```bash
git checkout main
git checkout -b <模型名>-<版本>-<MMDD>
# 放入 index.html 和 preview.png，写好分支 README
git add .
git commit -m "Add <模型名> <版本> pelican demo"
git push -u origin <分支名>
```

然后回到 `main`，在上面的分支索引表里补一行。

## 📄 License

[MIT](LICENSE)
