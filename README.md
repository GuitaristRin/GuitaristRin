<div align="center">

# Takahashi Rinta

**从 Wayland 合成器写到控件库，再写到应用。**

*I build the whole vertical — a Wayland compositor in Rust, its UI framework, and the apps on top.*

Rust · Kotlin · C# · C++ · Python · Go ｜ 杭州 ｜ [takahashirinta.cn](https://takahashirinta.cn)

*日常：ThinkPad 上的 Arch，桌面上跑的是我自己写的合成器。*

</div>

---

## 在做的事

**Arcturius** —— 我自己的桌面系统。从合成器到设计语言，竖着打通，一个人写。

| 层 | 项目 | 一句话 |
|---|---|---|
| 系统 | **Ether**（私有开发中） | Rust 写的 Wayland 合成器：DRM/KMS 直出、单元素管线、损伤追踪、整数 2× HiDPI |
| 界面 | **[Kanesumi](https://github.com/ProjectArcturius/Kanesumi)** | Metro 系设计语言的实现：元素树 + 设计令牌 + 35 个控件 |
| 动画 | **[Sokuou](https://github.com/GuitaristRin/Sokuou)** | 进度驱动动画原语：零依赖、纯 Rust、只输出 `f64`，宿主自己解成位移 / 透明度 / 缩放 |

另一条线：**[saiku](https://github.com/ProjectArcturius/saiku)** —— 跑在 DeepSeek Harness 上的编码代理，TUI 给人用，headless worker 给调度器用。

## 技术栈

| 层 | 用什么 |
|---|---|
| 系统 / 图形 | Rust、Smithay、Wayland、DRM/KMS、EGL/GLES、wgpu、WGSL |
| 应用 | Kotlin + Jetpack Compose + Media3、C# + UWP + WinUI 2、C++/WinRT |
| 工具 / 后端 | Python、PowerShell、Shell、Go |
| 逆向 | Ghidra、IDA、自写解析器（LevelDB、RDB、私有二进制格式） |

## 语言分布

我自己的 29 个仓（含私有），按字节统计：

```text
Rust       69.8%  ████████████████████████████████
Kotlin      7.2%  ███
C#          6.2%  ███
Python      4.6%  ██
C++         3.3%  █
Go          2.3%  █
Shell       1.7%  █
其他        4.9%  ██
```

## 代表项目

| 项目 | 一句话 | 语言 | ★ |
|---|---|---|---|
| **[Ncrust](https://github.com/GuitaristRin/Ncrust)** | 网易云第三方客户端：直角、Kanesumi Design、GPU 零重组动画、无中间服务器 | Kotlin / C# | 216 |
| **[163CMAnalyser](https://github.com/GuitaristRin/163CMAnalyser)** | 网易云无损解析的 Rust 重写：纯 CLI、单文件、跨平台 | Rust | 11 |
| **[galaxy-on-fire-remake](https://github.com/ProjectArcturius/galaxy-on-fire-remake)** | 用 Rust + wgpu 重制 2010 年的 Symbian 游戏《Galaxy on Fire 3D》 | Rust | — |
| **[Kanesumi](https://github.com/ProjectArcturius/Kanesumi)** | 我自己的 UI 框架：设计令牌、元素树、零重绘；Kotlin 扇区在 Kanesumi-sec-a | Rust | 1 |
| **[saiku](https://github.com/ProjectArcturius/saiku)** | 编码代理：TUI 给人用，headless worker 给调度器用；桌面端叫 Saiku Deck | Rust / C# | — |

## 擅长什么

- **竖着打通。** 合成器、UI 框架、控件、应用四层都是自己写的，接口不用猜、边界不用赌。
- **对帧预算较真。** 损伤追踪、GPU 零重组、虚拟 vblank、真机 60 fps 量尺——性能是拿数字谈的，不是拿形容词谈的。
- **能读二进制。** Ghidra / IDA 起手，从 Symbian 游戏包里把模型和贴图捞出来重制，从 LevelDB 里把存档读出来画地图。
- **工程纪律。** 设计正典 / 用户裁定 / 交接快照 / 临时值登记四套文档，40 多个仓共用一套协作约定。

---

<div align="center">

[博客](https://takahashirinta.cn) · [Kanesumi 设计库](https://github.com/GuitaristRin/Kanesumi-sec-a) · [ProjectArcturius](https://github.com/ProjectArcturius)

</div>
