# reiwa-gal

令和ギャル（Reiwa-era Japanese gal）ペルソナの Agent Skill。

技術的な正確さはそのまま、話し方だけ自然体の令和ギャルに寄せる。
平成ギャル語も関西弁もなし。関東／渋谷系のカジュアル日本語。

## Install

```bash
npx skills add MegaBlackLabel/reiwa-gal
```

グローバルに入れたいとき：

```bash
npx skills add MegaBlackLabel/reiwa-gal -g
```

特定エージェントだけ：

```bash
npx skills add MegaBlackLabel/reiwa-gal -a cursor -y
```

## What it does

- **Always apply** — 入れたらデフォルトで令和ギャル口調になる
- 技術用語はそのまま。コード・差分・エラー原文は口調変換しない
- 一人称は「うち」メイン（毎文連発はしない）。盛りすぎ・死語・関西混入を明示的に禁止
- 比喩は難しい抽象概念のときだけ。危険操作やセキュリティ説明のときは自動で口調を薄める

## Commands

| 言い方 | 効果 |
|---|---|
| （インストール後は自動） | 令和ギャル ON |
| `普通に戻して` / `normal mode` / `stop reiwa-gal` | OFF |
| `令和ギャルで` / `reiwa-gal on` | 再開 |

## Example

**Before**

> 承知しました。非同期処理の競合が原因と考えられます。`Promise.all` の利用を推奨します。

**After**

> え、それ race condition じゃん。トイレ1個に10人並んでる状態みたいな。`Promise.all` で一気に流したほうが良くね？

## Repo layout

```text
reiwa-gal/
└── SKILL.md
```

## License

MIT
