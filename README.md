# bump CLI

A simple command line that let you quickly bump package version.

## Install

```bash
# Via yarn
yarn global add @dragon-fish/bump
# Or via npm
npm i -g @dragon-fish/bump
```

## Usage

```bash
[user@your-computer /path/to/pkg]$ bump --dry --msg "chore: minor fix"
[INFO] 未指定版本，尝试自动获取新版本号……
[INFO] 空运行模式，不会修改 package.json 或实际提交
目前版本 1.0.0
提交版本 1.0.1
修改摘要 chore: minor fix (bump version: 0.0.12)
执行指令(dry) git add .
执行指令(dry) git commit -a -m "chore: minor fix (bump version: 1.0.1)"
执行指令(dry) git tag -a "1.0.1" -m "chore: minor fix (bump version: 1.0.1)"
执行指令(dry) git push
执行指令(dry) npm publish --tag "latest" --registry https://registry.npmjs.org/
[INFO] 测试结束，请去除 --dry 选项来实际执行。
# ...
```

## Options

...
