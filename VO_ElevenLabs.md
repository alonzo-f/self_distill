# SELF DISTILL — 画外音脚本（ElevenLabs 专用）

---

## 一、声音角色规格 VOICE CHARACTER

> 本片画外音为唯一配音角色，贯穿全片。所有生成须使用同一 Voice ID，以保证声线一致。

| 属性 | 规格 |
|------|------|
| **性别** | 女 |
| **年龄感** | 50–55 岁 |
| **口音** | 美式英语（American English），Mid-Atlantic 广播腔 |
| **音色** | 温暖、略带沙哑，中低音区，不尖锐 |
| **语速** | 平稳偏慢，约 105–115 words/min |
| **情绪** | 无论说什么内容，始终保持愉快、自信、不露讽刺 |
| **参考形象** | 1962 年美国电话接线员，被要求朗读一份反乌托邦产品说明，且对此感到发自内心的高兴 |

---

## 二、ElevenLabs 参数设置 SETTINGS

### 推荐声音（Voice Library）

按优先级排列，任选其一：

| 优先 | Voice Name | 说明 |
|------|-----------|------|
| ★★★ | **Dorothy** | 温暖美式女声，有轻微播报质感，最接近目标 |
| ★★★ | **Grandma Archer** | 成熟温暖，自然沙哑，60s 感强 |
| ★★☆ | **Ruth** | 成熟旁白女声，权威中带温暖 |
| ★★☆ | **Matilda** | 温暖美式，略年轻，可接受 |
| ★☆☆ | **Serena** | 专业感强，偏现代，需调低 style |

> 若以上均不满意，使用 **Voice Design** 功能，输入描述：
> `"Warm, slightly husky American female voice, age 55, 1960s broadcast cadence, cheerful and measured, mid-low register, never rushed, never ironic"`

---

### 参数面板设置

| 参数 | 推荐值 | 说明 |
|------|--------|------|
| **Stability** | `0.72` | 稳定但不机械，保持一致性 |
| **Similarity Boost** | `0.78` | 锁定声线特征 |
| **Style Exaggeration** | `0.12` | 极低——要的是克制，不是戏剧性 |
| **Speaker Boost** | `ON` | 增强清晰度和存在感 |
| **Model** | `Eleven Multilingual v2` | 质量最优；如需快速迭代用 `Turbo v2.5` |

---

## 三、完整脚本（一次生成）FULL SCRIPT — ONE TAKE

> 将以下文本直接粘贴进 ElevenLabs，生成完整连读版 VO。
> 生成后导入剪辑软件，按第五节《时间码参照表》截取各段。

---

### 3A — 纯文本版（UI 直接粘贴）

```
Are you tired of useless emotion?

Don't let your bad feelings get in your way. Introducing Self Distill — our new system to help you produce the fullest.

Upload yourself in seconds — and we'll make you better, faster, stronger.

Free yourself — right now, right away.

Self Distill — let us do the feeling for you.
```

> **操作说明**：
> - 每一段之间的空行会让 ElevenLabs 自动产生约 0.5 秒停顿，符合各段之间的视觉间隔
> - 如停顿不够长，在段落之间手动添加 `...` 延长停顿感

---

### 3B — SSML 版（ElevenLabs API 使用）

> 适用于 ElevenLabs API（`/v1/text-to-speech`），通过 `text_type: "ssml"` 参数传入。
> 提供精确的停顿时长、语速变化和重读控制。

```xml
<speak>

  <!-- LINE 1: 0:03–0:08 | SHOT 02 | 亲切提问，"useless" 轻重读 -->
  <prosody rate="95%">
    Are you tired of <emphasis level="moderate">useless</emphasis> emotion?
  </prosody>

  <break time="1.2s"/>

  <!-- LINE 2: 0:20–0:24 | SHOT 07 | 治疗师口吻，温和权威 -->
  <prosody rate="93%">
    Don't let your bad feelings get in your way.
  </prosody>

  <break time="0.3s"/>

  <!-- LINE 3: 0:24–0:30 | SHOTS 08–09 | 品牌介绍，破折号处停顿 -->
  <prosody rate="93%">
    Introducing <emphasis level="moderate">Self Distill</emphasis>
    <break time="0.45s"/>
    our new system to help you produce the <emphasis level="reduced">fullest</emphasis>.
  </prosody>

  <break time="0.8s"/>

  <!-- LINE 4–5: 0:30–0:37 | SHOTS 10–11 | 功能列举，三词等距强调 -->
  <!-- 注意：em-dash 处是 SHOT 10/11 的剪辑切点，生成后在此处裁切 -->
  <prosody rate="100%">
    Upload yourself in seconds
    <break time="0.5s"/>
    and we'll make you
    <emphasis level="moderate">better</emphasis>,
    <emphasis level="moderate">faster</emphasis>,
    <emphasis level="moderate">stronger</emphasis>.
  </prosody>

  <break time="1.0s"/>

  <!-- LINE 6–7: 0:40–0:47 | SHOTS 13–14 | 最温柔，几乎低语，停顿 -->
  <!-- 注意：em-dash 处是 SHOT 13/14 的剪辑切点，生成后在此处裁切 -->
  <prosody rate="88%" volume="-2dB">
    Free yourself
    <break time="0.5s"/>
    right now, right away.
  </prosody>

  <break time="1.0s"/>

  <!-- LINE 8–9: 0:55–1:00 | SHOTS 17–18 | 最深沉，品牌名如仪式 -->
  <!-- 注意：em-dash 处是 SHOT 17/18 的剪辑切点，生成后在此处裁切 -->
  <prosody rate="85%" volume="-1dB">
    Self Distill
    <break time="0.5s"/>
    let us do the <emphasis level="moderate">feeling</emphasis> for you.
  </prosody>

</speak>
```

---

## 四、分段脚本（精细控制）SEGMENTED TAKES

> 如需对每句进行独立调音，可按以下 5 个 Take 分别生成。
> 每个 Take 在 ElevenLabs 中单独生成、单独下载，在剪辑软件中拼接。
> 各 Take 须使用**完全相同的 Voice ID 和参数设置**，保证声线一致。

---

### TAKE 01
**对应时间码**：0:03 – 0:08（SHOT 02）
**情绪指令**：亲切，像在问老朋友周末过得怎么样。轻松，不沉重。

**Settings 微调**：
- Stability: `0.72`
- Style: `0.12`

**粘贴文本**：
```
Are you tired of useless emotion?
```

**SSML 版**：
```xml
<speak>
  <prosody rate="95%">
    Are you tired of <emphasis level="moderate">useless</emphasis> emotion?
  </prosody>
</speak>
```

**导演备注**：
- "Are you tired of" — 平直，稍快
- "useless" — 略微拉长元音，带温暖，不带嘲讽
- "emotion?" — 略微上扬（问句），但幅度小，不惊讶

---

### TAKE 02
**对应时间码**：0:20 – 0:30（SHOTS 07–09）
**情绪指令**：温和权威，像医生在宣布你的诊断，但语气是在讨论天气。品牌名"Self Distill"像亲切介绍老朋友。

**Settings 微调**：
- Stability: `0.74`
- Style: `0.10`

**粘贴文本**：
```
Don't let your bad feelings get in your way. Introducing Self Distill — our new system to help you produce the fullest.
```

**SSML 版**：
```xml
<speak>
  <prosody rate="93%">
    Don't let your bad feelings get in your way.
    <break time="0.3s"/>
    Introducing <emphasis level="moderate">Self Distill</emphasis>
    <break time="0.45s"/>
    our new system to help you produce the <emphasis level="reduced">fullest</emphasis>.
  </prosody>
</speak>
```

**导演备注**：
- "bad feelings" — 说得很自然，像在说"bad weather"，不带情绪评判
- "Introducing" — 略微提亮，宣告感，像主持人念品牌名
- "Self Distill" — 清晰发音，稍慢，每个音节等重
- em-dash "—" 处 → 停顿约 0.4s（视觉上对应 James 的眼镜反光）
- "produce the fullest" — 略微加重，收尾有分量

---

### TAKE 03
**对应时间码**：0:30 – 0:37（SHOTS 10–11）
**情绪指令**：产品广告功能列举节奏，稍快，自信，节奏均匀。三个形容词像在打节拍。

**Settings 微调**：
- Stability: `0.70`
- Style: `0.15`（略微增加活力感）

**粘贴文本**：
```
Upload yourself in seconds — and we'll make you better, faster, stronger.
```

**SSML 版**：
```xml
<speak>
  <prosody rate="100%">
    Upload yourself in seconds
    <break time="0.5s"/>
    and we'll make you
    <emphasis level="moderate">better</emphasis>,
    <emphasis level="moderate">faster</emphasis>,
    <emphasis level="moderate">stronger</emphasis>.
  </prosody>
</speak>
```

**导演备注**：
- "Upload yourself" — 说得和"upload a file"一样自然，零迟疑
- "in seconds" — 略快，轻松
- em-dash "—" 处 → 停顿约 0.5s（**此处是 SHOT 10/11 的剪辑切点**）
- "better, faster, stronger" — 三词等时间间隔，每词之间约 0.2s 停顿，像在打三个轻拍

---

### TAKE 04
**对应时间码**：0:40 – 0:47（SHOTS 13–14）
**情绪指令**：全片最温柔的一句。像在低语一个礼物。"Free yourself"要有重量，但不要沉重——是温柔的释放。

**Settings 微调**：
- Stability: `0.76`（更稳定，防止过度波动）
- Style: `0.08`（极克制）
- 可在 ElevenLabs 界面将整段音量略微调低

**粘贴文本**：
```
Free yourself — right now, right away.
```

**SSML 版**：
```xml
<speak>
  <prosody rate="88%" volume="-2dB">
    Free yourself
    <break time="0.5s"/>
    right now, right away.
  </prosody>
</speak>
```

**导演备注**：
- "Free" — 全片最重的一个词，拉长元音，但不要呻吟，像在轻轻放下什么
- "yourself" — 正常，不拖
- em-dash "—" 处 → 停顿约 0.5s（**此处是 SHOT 13/14 的剪辑切点**）
- "right now" — 轻微节奏感，像 Bossa Nova 的节拍
- "right away" — 平稳收尾，尾音不拖

---

### TAKE 05
**对应时间码**：0:55 – 1:00（SHOTS 17–18）
**情绪指令**：全片最深沉、最亲密的一刻。"Self Distill"像念一个神圣的名字。"let us do the feeling for you"要带微笑，句末轻微上扬——不是问句，是承诺。

**Settings 微调**：
- Stability: `0.78`（最稳定）
- Style: `0.08`（极克制）
- 整段语速最慢

**粘贴文本**：
```
Self Distill — let us do the feeling for you.
```

**SSML 版**：
```xml
<speak>
  <prosody rate="85%" volume="-1dB">
    Self Distill
    <break time="0.5s"/>
    let us do the <emphasis level="moderate">feeling</emphasis> for you.
  </prosody>
</speak>
```

**导演备注**：
- "Self Distill" — 两个词各自清晰，停顿在中间（约 0.5s），像在念两个音节的咒语
- em-dash "—" 处 → 停顿约 0.5s（**此处是 SHOT 17/18 的剪辑切点**）
- "let us do" — 平稳，温柔
- "the feeling" — "feeling"是全句最重的词，元音略拉长
- "for you" — 句末轻微上扬，像微笑着说完。不是疑问，是礼物

---

## 五、剪辑时间码参照表 EDITING TIMING REFERENCE

> 生成完成后，将音频导入剪辑软件，按以下表格将各段放置在对应时间码位置。
> 生成的 VO 音频总时长约 **25–28 秒**（含段内停顿），剩余时间为视频中的静默段。

| Take | VO 文本 | 画面入点 | 画面出点 | 对应 Shot | 备注 |
|------|---------|---------|---------|----------|------|
| 01 | "Are you tired of useless emotion?" | `0:03.0` | `0:07.5` | SHOT 02 | VO 随画面起，约 4.5s |
| — | *(静默)* | `0:07.5` | `0:20.0` | SHOTS 03–06 | 12.5s 空白，**不放任何 VO** |
| 02a | "Don't let your bad feelings get in your way." | `0:20.0` | `0:23.5` | SHOT 07 | VO 与马林巴 Sting 同时起 |
| 02b | "Introducing Self Distill —" | `0:23.8` | `0:25.5` | SHOT 08 | 破折号停顿约 0.45s |
| 02c | "our new system to help you produce the fullest." | `0:25.9` | `0:29.5` | SHOTS 08–09 | 最后一词"fullest"落在 Sofia 点击图标瞬间 |
| — | *(静默)* | `0:29.5` | `0:30.0` | — | 短暂空白，让音乐过渡 |
| 03a | "Upload yourself in seconds—" | `0:30.0` | `0:32.5` | SHOT 10 | **在此处切断音频**，剩余部分用于 SHOT 11 |
| 03b | "—and we'll make you better, faster, stronger." | `0:34.0` | `0:37.0` | SHOT 11 | 从 Take 03 音频中剪出后半段接入 |
| — | *(静默)* | `0:37.0` | `0:40.0` | SHOT 12 | 3s 空白，让音乐过渡至 Bossa Nova |
| 04a | "Free yourself —" | `0:40.0` | `0:42.5` | SHOT 13 | **在此处切断音频**，与 Bossa Nova 同时起 |
| 04b | "right now, right away." | `0:44.0` | `0:46.5` | SHOT 14 | 从 Take 04 音频中剪出后半段接入 |
| — | *(静默)* | `0:46.5` | `0:55.0` | SHOTS 15–16 | 8.5s 空白，三人的目光 + 台词覆盖 |
| 05a | "Self Distill —" | `0:55.0` | `0:56.5` | SHOT 17 | **在此处切断音频**，随虚焦画面起 |
| 05b | "let us do the feeling for you." | `0:57.0` | `1:00.0` | SHOT 18 | 从 Take 05 音频中剪出后半段接入，随 Logo 出现 |

---

### Take 03/04/05 的剪辑切点说明

Take 03、04、05 每个都是一整句，但句子跨越两个 Shot。
生成后按以下方法处理：

```
Take 03 原始音频：
[Upload yourself in seconds] [0.5s停顿] [and we'll make you better, faster, stronger.]
                            ↑
                       在此切断
                  前半 → 放在 0:30.0 (SHOT 10)
                  后半 → 放在 0:34.0 (SHOT 11)

Take 04 原始音频：
[Free yourself] [0.5s停顿] [right now, right away.]
                ↑
           在此切断
      前半 → 放在 0:40.0 (SHOT 13)
      后半 → 放在 0:44.0 (SHOT 14)

Take 05 原始音频：
[Self Distill] [0.5s停顿] [let us do the feeling for you.]
               ↑
          在此切断
     前半 → 放在 0:55.0 (SHOT 17)
     后半 → 放在 0:57.0 (SHOT 18)
```

---

## 附：人物台词（非 VO，另行录制）

> 以下台词**不属于**画外音 VO，须由真人演员分别录制，不通过 ElevenLabs 生成。

| 角色 | 时间码 | 台词 | 情绪 |
|------|--------|------|------|
| Maya | 0:03–0:09 | *"Yes— yes, I understand— hold please— no, YOU hold please—"* | 碎片化、交叠，仍保持职业微笑语气 |
| Maya | 0:09–0:12 | *"—one moment please— I said HOLD—"* | 快要崩溃，但仍在撑 |
| Sofia | 0:15–0:18 | *"This is really important, okay? Can everyone look up? Anyone?"* | 从热情到无奈，语调缓慢下滑 |
| 三人齐声 | 0:51–0:55 | ***"We recommend Self Distill!"*** | 见主脚本录音说明 |
