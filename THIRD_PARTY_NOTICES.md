# 第三方组件声明

畅投使用了以下开源组件，感谢这些项目的作者。各组件按自己的许可证授权，与畅投本身的[使用条款](LICENSE.md)无关。

| 组件 | 版本 | 用途 | 许可证 | 包含在 |
| --- | --- | --- | --- | --- |
| [AndroidX Media3](https://github.com/androidx/media)（ExoPlayer、HLS、DASH、UI、Effect） | 1.4.1 | 视频、音乐播放；滤镜 | Apache License 2.0 | 普通版、增强版 |
| [AndroidX](https://developer.android.com/jetpack/androidx) 支持库（Media3 的依赖） | — | 系统兼容 | Apache License 2.0 | 普通版、增强版 |
| [Guava](https://github.com/google/guava)（Media3 的依赖） | — | 基础工具库 | Apache License 2.0 | 普通版、增强版 |
| [Kotlin 标准库](https://github.com/JetBrains/kotlin) | — | 编程语言运行库 | Apache License 2.0 | 普通版、增强版 |
| [NanoHTTPD](https://github.com/NanoHttpd/nanohttpd) | 2.3.1 | 局域网 HTTP 服务（接收投屏指令） | BSD 3-Clause | 普通版、增强版 |
| [ZXing](https://github.com/zxing/zxing)（`com.google.zxing:core`） | 3.3.3 | 在本机生成“关于”页的二维码 | Apache License 2.0 | 普通版、增强版 |
| [libVLC for Android](https://code.videolan.org/videolan/vlc-android)（`org.videolan.android:libvlc-all`） | 3.6.5 | 备用播放内核（软件解码） | GNU LGPL 2.1 或更高版本 | 仅增强版 |

## libVLC（仅增强版）

增强版以独立的动态链接库（APK 内 `lib/*/libvlc.so` 等文件）形式包含 libVLC，畅投没有修改 libVLC。libVLC 及其内置的解码库（如 FFmpeg）按 GNU 宽通用公共许可证 2.1 或更高版本（LGPL-2.1-or-later）授权。

- 许可证全文：https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
- 源代码：VideoLAN 官方发布的 libvlc-all 3.6.5，源码见 https://code.videolan.org/videolan/vlc-android 及 https://code.videolan.org/videolan/vlc 对应版本。
- 如需我们提供所用 libVLC 版本的完整源代码副本，请在本仓库提交 Issue，自增强版发布之日起三年内有效。

你有权按 LGPL 修改 libVLC 并替换增强版中的对应动态库。

## Apache License 2.0

AndroidX Media3、AndroidX、Guava、Kotlin 标准库、ZXing 按 Apache License 2.0 授权：

```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## NanoHTTPD

```
Copyright (c) 2012 - 2016, nanohttpd

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the nanohttpd nor the names of its contributors
   may be used to endorse or promote products derived from this software without
   specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
OF THE POSSIBILITY OF SUCH DAMAGE.
```
