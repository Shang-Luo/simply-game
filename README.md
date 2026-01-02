# simply-game
这是一个旨在锻炼git操作和简单结构化编程的简单小游戏，作为下一步计划的练手之作。
本作为一个简单的飞机大战小游戏，重点在于面向对象的编程能力和代码规范提交能力。

---
# 目录
### 1.技术栈及开发语言

---
## 1.技术栈及开发语言

本项目采用`python(pygame)`为前端，`c++`后端，`pybind11`集成的方法
##### 阶段一
```
game_project/
├── src/
│   ├── cpp_backend/              # C++后端
│   │   ├── core/                 # 核心系统
│   │   │   ├── game_engine.h
│   │   │   └── game_engine.cpp
│   │   ├── physics/              # 物理引擎
│   │   │   ├── physics.h
│   │   │   └── physics.cpp
│   │   └── bindings/             # Python绑定（关键）
│   │       └── game_bindings.cpp  # 唯一绑定文件
│   │
│   └── python_frontend/          # Python前端
│       ├── core/                 # 核心（3个文件）
│       │   ├── main.py          # 主入口
│       │   ├── game.py          # 游戏主类
│       │   └── config.py        # 配置管理
│       ├── rendering/           # 渲染（2个文件）
│       │   ├── renderer.py      # 渲染器
│       │   └── sprite.py        # 精灵类
│       └── input/               # 输入（1个文件）
│           └── input.py         # 输入处理
│
├── assets/                       # 资源
│   ├── images/                  # 图片
│   ├── fonts/                   # 字体（仅需1个）
│   └── audio/                   # 音频（可选）
│
├── config/                      # 配置（3个文件）
│   ├── settings.json           # 游戏设置
│   ├── keybindings.json        # 按键绑定
│   └── game_data.json          # 游戏数据
│
├── saves/                      # 存档（简单实现）
│   └── save_001.json          # 单一存档文件
│
├── CMakeLists.txt              # C++构建配置
├── requirements.txt            # Python依赖
├── run.py                     # 一键运行脚本
├── README.md                  # 项目说明
└── .gitignore                 # Git忽略
```
