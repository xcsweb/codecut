# codecut

Headless、JSON-first 的剪辑 CLI：素材登记、多轨时间线、字幕、转场、混音、预览与渲染，底层调用 FFmpeg。

## 构建与测试

```bash
npm ci
npm run build
npm test
```

## 使用

```bash
node dist/cli.js --help
node dist/cli.js project init my-project --name "demo"
node dist/cli.js asset add clip.mp4 --id clip --project my-project
node dist/cli.js edit apply operations.json --project my-project --dry-run
node dist/cli.js render --project my-project
```

`codecut` 的行为与工程格式见 [docs/design.md](docs/design.md)。
