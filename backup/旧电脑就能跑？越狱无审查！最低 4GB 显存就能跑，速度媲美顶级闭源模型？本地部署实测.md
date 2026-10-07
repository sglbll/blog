<img width="515" height="175" alt="Image" src="https://github.com/user-attachments/assets/3aca708e-2fb4-47c8-9c46-0ea06921054a" />


# 部署教程
## 一、Qwen3.5-9B 开源模型 

> 目前量化的 Qwen3.5 9B 模型总共有 22 个（21 个量化档位 + 1 个 BF16 全精度权重，另外还附送 3 个 mmproj 多模态视觉投影文件，整个仓库合计 25 个 GGUF 文件），格式为 GGUF，体积从 3.0 GB 一直到 16.7 GB，可以适配多种不同尺寸的显存大小，最低支持 4G 显存（UD-IQ2_XXS，仅 3.0 GB，量化得相当激进，画质/智力损失也最大）；8G 显存推荐 Q4_K_M 或 UD-Q4_K_XL 这档甜点位，12G 显存可以上 Q6_K / UD-Q6_K_XL，16G 显存则能吃下 Q8_0 甚至 UD-Q8_K_XL。当然如果你的显存是低于 4G 的，那么你可以直接跳到第四步，下载越狱（abliterated）的模型——目前已有 lukey03、mradermacher、Abiray、huihui-ai 等多套 Qwen3.5-9B 越狱版，同样提供 GGUF 量化，最低也能压到 4G 显存以下

### 1、Huggingface 下载： 【[点击前往](https://huggingface.co/unsloth/Qwen3.5-9B-GGUF)】
### 2、网盘下载： 【[点击前往](https://1849512709.share.123pan.cn/123pan/ElMkvd-0GbJd)】
### 3、镜像下载：【[点击前往](https://hf-mirror.com/unsloth/Qwen3.5-9B-GGUF)】


| 量化 | 文件大小 | 权重(GiB) | 8K 上下文 | 32K 上下文 | 建议显卡 |
| -- | -- | -- | -- | -- | -- |
| UD-IQ2_XXS | 3.19 GB | 3.0 | 3.9 | 4.6 | 6G（3050 6G / 2060 6G） |
| UD-IQ2_M | 3.65 GB | 3.4 | 4.3 | 5.1 | 6G |
| UD-IQ3_XXS | 4.02 GB | 3.7 | 4.6 | 5.4 | 6G 极限 / 8G 舒适 |
| UD-Q2_K_XL | 4.12 GB | 3.8 | 4.7 | 5.5 | 8G |
| Q3_K_S | 4.32 GB | 4.0 | 4.9 | 5.7 | 8G |
| Q3_K_M | 4.67 GB | 4.4 | 5.3 | 6.0 | 8G |
| UD-Q3_K_XL | 5.05 GB | 4.7 | 5.6 | 6.4 | 8G　低显存首选 |
| IQ4_XS | 5.17 GB | 4.8 | 5.7 | 6.5 | 8G |
| IQ4_NL | 5.37 GB | 5.0 | 5.9 | 6.7 | 8G |
| Q4_K_S / Q4_0 | 5.38 GB | 5.0 | 5.9 | 6.7 | 8G |
| Q4_K_M | 5.68 GB | 5.3 | 6.2 | 6.9 | 8G（4060 8G / 3070） |
| Q4_1 | 5.84 GB | 5.4 | 6.3 | 7.1 | 8G 偏紧 / 12G |
| UD-Q4_K_XL | 5.97 GB | 5.6 | 6.5 | 7.2 | 8G　全场最佳性价比 |
| Q5_K_S | 6.36 GB | 5.9 | 6.8 | 7.6 | 8G 极限 / 12G |
| Q5_K_M | 6.58 GB | 6.1 | 7.0 | 7.8 | 12G（3060 12G / 5070） |
| UD-Q5_K_XL | 6.74 GB | 6.3 | 7.2 | 7.9 | 12G |
| Q6_K | 7.46 GB | 7.0 | 7.9 | 8.6 | 12G |
| UD-Q6_K_XL | 8.76 GB | 8.2 | 9.1 | 9.8 | 12G |
| Q8_0 | 9.53 GB | 8.9 | 9.8 | 10.5 | 12G 偏紧 / 16G |
| UD-Q8_K_XL | 12.97 GB | 12.1 | 13.0 | 13.7 | 16G（4060Ti 16G / 5060Ti 16G） |
| BF16（文件夹） | 17.92 GB | 16.7 | 17.6 | 18.3 | 24G（3090 / 4090）或双卡 12G |


## 二、下载llama.cpp
 

### 1、Github 下载：【[点击前往](https://github.com/ggml-org/llama.cpp)】
### 2、网盘下载：【[点击前往](https://pan.quark.cn/s/4f3fad9080b0)】

<img width="1409" height="1049" alt="Image" src="https://github.com/user-attachments/assets/75f63123-3280-43bb-85c0-f8b3f74a21f8" />

## 三、越狱模型

> Qwen3.5-9B 现在已经推出了多个真正无审查的越狱模型，如果你想更自由，不受约束和限制，在本地使用越狱模型，那么下方的模型切勿错过！真正实现模型自由，几乎可以满足你任何的特殊需求。并且最低支持4G显存！

### 1、Huggingface 下载 【[点击前往](https://huggingface.co/DavidAU/Qwen3.5-9B-The-Defiant-Fable-Uncensored-Heretic-NEO-IMATRIX-MAX-MTP-GGUF/tree/main)】

### 2、镜像下载：【[点击前往](https://hf-mirror.com/DavidAU/Qwen3.5-9B-The-Defiant-Fable-Uncensored-Heretic-NEO-IMATRIX-MAX-MTP-GGUF/tree/main)】

## 四、对接 DSH

### 1、官方下载：【[点击前往](https://deepseek.com/harness/)】

### 2、高速下载：【[点击前往](https://1849512709.share.123pan.cn/123pan/ElMkvd-KGbJd)】

<img width="1923" height="1234" alt="Image" src="https://github.com/user-attachments/assets/836eb719-9b0a-4e56-8238-ec472545775a" />