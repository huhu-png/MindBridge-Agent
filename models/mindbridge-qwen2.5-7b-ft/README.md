# 本地微调模型

将 `mindbridge-qwen2.5-7b-ft-q4_k_m.gguf.zip` 解压，把 GGUF 文件放在本目录，与 `Modelfile` 同级。模型文件为 4,683,073,536 字节，不随 Git 仓库分发。

在仓库根目录安装并启动 Ollama 后运行：

```bash
bash scripts/create-finetuned-model.sh
```

也可通过 `UPSTREAM_GGUF=/absolute/path/model.gguf` 指定已有模型文件。模型权重的来源、训练过程及再分发许可尚未随项目提供；本仓库不声明其许可证。没有权重时，可按根目录 README 配置其他 Ollama 模型、OpenAI-compatible API 或 Mock Provider。
