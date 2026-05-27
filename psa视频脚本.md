# SELF DISTILL — PSA 完整制作手册

> **配音风格**：温暖客服阿姨，60年代美国广播感——愉快、略带沙哑的女声，音调略高，节奏稳定如播报天气预报；言辞令人不安，语气却无比温馨。

---

## 一、人物设定 CHARACTER BIBLE

> AI生成时须严格保持人物物理特征一致性，尤其是脸型、眼神光位置、服装细节。

### 角色 A — Maya（客服代表）

| 属性 | 描述 |
|------|------|
| 性别／年龄 | 女，32 岁 |
| 种族 | 非裔美国人 |
| 脸型 | 圆脸，颧骨高挺 |
| 头发 | 4C 型自然卷，梳成蓬松丸子头（afro puff bun），金色发圈固定 |
| 眼睛 | 深棕色，略呈杏仁形，双眼均有 LED 眼神光高光点（瞳孔左上象限） |
| 肤色 | 深棕（Fitzpatrick V 型） |
| 嘴唇 | 丰满唇形，自然唇色 |
| 身高／体型 | 约 165 cm，中等身材 |
| **工作服装** | 矢车菊蓝色纽扣衬衫，黑色头戴式耳机（带 boom 话筒），细金项链 |
| 标志性物件 | 双手各持一部电话 |

---

### 角色 B — James（白领职员）

| 属性 | 描述 |
|------|------|
| 性别／年龄 | 男，48 岁 |
| 种族 | 白人（东欧裔美国人） |
| 脸型 | 方形下颌，眉骨明显 |
| 头发 | 短发，灰白相间（约 60% 灰，40% 深棕），梳理整齐 |
| 眼睛 | 蓝灰色，轻微鱼尾纹，双眼均有 LED 眼神光高光点（瞳孔左上象限） |
| 肤色 | 白皙（Fitzpatrick II 型），两颊略泛红，轻微短胡茬 |
| 身高／体型 | 约 180 cm，略显壮实 |
| **工作服装** | 深海军蓝西装，白色衬衫，暗红色领带（略松），细框金属眼镜 |
| 标志性物件 | 被文件淹没的办公桌 |

---

## 二、技术规格 TECHNICAL SPECIFICATIONS

### 拍摄设备

| 设备类型 | 规格 |
|----------|------|
| 主摄像机 | ARRI Alexa 35（室内实景：客服室／办公室） |
| 副摄像机 | Sony FX3（手持特写／快剪／自拍 INSERT） |
| 室内镜头组 | Leica Summilux-C Prime Set（25 mm 广角 / 50 mm 标准 / 75 mm 人像） |
| 数字段虚拟摄像机 | CG 虚拟摄像机（Unreal Engine / After Effects 合成），等效 50 mm 球面视角 |
| 稳定系统 | DJI Ronin 4D（运动推拉） / O'Connor 2575（固定三脚架） / 80 cm 滑轨（横移） |

---

### 全片统一打光方案

> **一致性要求**：两个实景室内场景（客服室／办公室）光源角度、色温完全一致，确保剪辑无跳跃感。数字处理段与数字替身段以纯黑或深色背景为主，绿色数字自发光替代传统灯光设置。

| 光源类型 | 参数 | 说明 |
|----------|------|------|
| **主光 Key Light** | ARRI SkyPanel S60-C，5600 K，左上方 45° 入射 | 主照明，模拟窗光 |
| **辅助光 Fill Light** | Kino Flo Diva 400，右侧扩散柔光箱，强度为主光 1/3 | 补暗部细节 |
| **眼神光 Eye Light** | Litepanels Micro LED，固定于摄像机正下方 | 双眼高光点，瞳孔左上象限 |
| **轮廓光 Rim Light** | ARRI L7-C，6500 K，后方 45° 侧照 | 勾勒人物轮廓 |
| **背景光 BG Light** | 散射柔光面板，降低背景曝光 −1.5 EV | 虚化背景，突出人物 |
| **数字段自发光** | 绿色 #00FF41 内部辉光，无外部光源 | 仅用于 SHOTS 09–12 |

---

### 后期色调方案

| 幕次 | 色温 | 风格 |
|------|------|------|
| Act 1 混乱段（SHOTS 01–05） | 4800 K，偏冷 | 高对比，青绿色阴影，轻微色差，8 mm 胶片划痕叠层 |
| Act 2 系统介入（SHOTS 06–08） | 5200 K，回暖 | 对比渐软，暖调渗入，白色 UI 反光净化画面 |
| Act 3 数字处理（SHOTS 09–10） | 去色化，黑底绿光主导 | 仅保留绿色 #00FF41 数字发光，Tron 美学，无颗粒 |
| Act 4 数字替身（SHOTS 11–12） | 纯黑背景，深蓝环境辉光 | 高对比，人体轮廓由绿色数字构成，轮廓外发光 glow |
| Act 5 解脱（SHOT 13） | 5600 K，温暖自然 | 对比柔和，skin tone 全面还原，微金色调 |
| Act 6 CTA（SHOT 14） | 纯白底 #FFFFFF，极简 | 品牌色调，零颗粒，零纹理 |
| 全片叠加 | — | 轻微暗角（vignette）＋极轻色差（chromatic aberration，仅 Act 1） |

---

## 三、音乐方案 MUSIC DESIGN

| 幕次 | 时间码 | 风格描述 | 乐器 | 参考曲目 | BPM | 情绪 |
|------|--------|----------|------|----------|-----|------|
| Act 1 混乱 | 0:00–0:18 | 混乱大乐队爵士＋焦虑弦乐 | 弱音小号、快速拨弦、不和谐钢琴 | Raymond Scott《Powerhouse》 | 168 | 失控、压迫、荒诞 |
| 过渡 Sting | 0:18 | 单一清亮钟声＋2 拍停顿 | 马林巴＋铃铛 | 老式电话接通音效 | — | 解脱瞬间 |
| Act 2 系统介入 | 0:18–0:36 | 欢快 60 年代企业广告曲 | 马林巴、跳跃低音、明亮铜管 | 《The Jetsons》主题曲 | 132 | 效率、乐观、微妙讽刺 |
| Act 3 数字处理 | 0:36–0:46 | 电子合成器＋企业广告曲混合 | Kraftwerk 式合成器贝斯＋60 年代铜管 | Kraftwerk《Computer Love》× The Jetsons | 132 | 数据化、精准、微妙不安 |
| Act 4 数字替身 | 0:46–0:53 | 玻璃质感极简电子 | 玻璃音阶、马林巴回响、极简鼓机 | Philip Glass 式极简主义钢琴 | 100 | 空灵、超自然、略显孤独 |
| Act 5 解脱 | 0:53–0:57 | 温暖管弦乐广告收尾 | 弦乐＋铜管＋钢琴全奏和弦 | 经典 60 年代 TV 广告收尾 | 110 | 圆满、温暖、微讽 |
| Act 6 CTA | 0:57–1:00 | 品牌广告结束音效（jingle） | 清亮双音钢琴 | 经典 60 年代 TV 商业广告收尾音 | — | 圆满、记忆钩子 |

---

## 四、分镜与 AI 提示词 STORYBOARD + AI PROMPTS

> 本节将分镜说明与 AI 生成提示词合并。每个 shot 的提示词均包含完整的 **图像（IMAGE）**、**画外音（VOICEOVER）**、**音乐（MUSIC）** 三部分，可直接用于 Runway Gen-4 / Kling 2.0 / Sora / Pika 2.0 等工具。

---

### 🔑 人物一致性速查（每条 prompt 须复制对应角色描述）

**[MAYA]**
> Maya, a 32-year-old Black American woman. Round face with high cheekbones. Type 4C natural hair in a voluminous afro puff bun secured with a gold scrunchie. Deep brown almond-shaped eyes — a sharp LED catch-light dot visible in the upper-left quadrant of BOTH pupils at all times. Full lips, natural lip color. Deep brown skin (Fitzpatrick Type V). Medium build, ~165 cm. Thin gold chain necklace.

**[JAMES]**
> James, a 48-year-old white American man of Eastern European descent. Square jaw with prominent brow ridge. Short salt-and-pepper hair (60% silver-gray, 40% dark brown), neatly combed. Blue-gray eyes with light crow's feet — a sharp LED catch-light dot in the upper-left quadrant of BOTH pupils at all times. Light stubble. Fair complexion, slight ruddiness on cheeks (Fitzpatrick Type II). Tall, slightly heavyset, ~180 cm. Thin gold wire-rimmed rectangular glasses.

---

### 🔑 画外音声音规格（VO VOICE SPEC，全片统一）

> 每条 prompt 中的 VOICEOVER 段均默认使用以下声音角色规格。AI 语音生成工具（ElevenLabs、Eleven v2 等）建议选用 50–55 岁成熟美国女声模型，稳定性 high，语气夸张度 low，情感温度 max。

**声音角色**：女性，约 50–55 岁，声线温暖、略带沙哑，带有 1960 年代美国广播腔——语速平稳（约每分钟 110 词），无论台词内容如何均保持愉快自信、不露丝毫讽刺。效果目标：一位 1962 年的电话接线员被要求朗读一份反乌托邦产品说明，且对此感到发自内心的兴奋。

---

### 🔴 ACT 1：情绪噪音的痛苦 [0:00 – 0:18]

---

#### SHOT 01｜0:00 – 0:03｜片头字卡

| 项目 | 内容 |
|------|------|
| **景别** | 字卡（黑底白字） |
| **摄像机运动** | 静止 |
| **场景描述** | 纯黑背景，复古衬线字体缓缓出现："HAVE YOU EVER FELT…"，字体参考 1960 年代美国 PSA 字卡（slab serif），带轻微胶片颗粒。 |
| **人物动作** | 无人物 |
| **人物台词** | 无 |

```
=== IMAGE ===
Motion graphic title card. Pure black background (#000000). Vintage slab-serif typeface
(Clarendon or Rockwell style) in white, fading in letter by letter over 2 seconds:
"HAVE YOU EVER FELT..." Subtle 8mm film grain texture overlaid. Light vignette at
corners darkening toward edges. No camera movement. Duration: 3 seconds.
Static composition, centered text, nothing else in frame.

SHOT TYPE: Title card / motion graphic. No camera. No lens. No live action.
LIGHTING: None — black background with white text only.
PROPS: None.
STAGING: Typography-only composition. Text centered at 40% of frame height.
SCENE: Pure black void.

=== VOICEOVER ===
SILENCE. No voiceover in this shot.
Ambient only: a barely audible film projector hum texture, rising from nothing to
-35 dB over 3 seconds — the acoustic atmosphere of an old public service film reel.

=== MUSIC ===
Complete silence. A single low piano tone (C2) at -32 dB holds for 3 seconds —
nearly inaudible, felt more than heard. This is the quiet before the chaos.
Do NOT begin the jazz theme yet.
```

---

#### SHOT 02｜0:03 – 0:09｜全景 WS → 缓慢推进 DOLLY IN

| 项目 | 内容 |
|------|------|
| **景别** | 全景（Wide Shot），轴线缓慢推进 |
| **摄像机运动** | O'Connor 三脚架开场，0:06 起 DJI Ronin 缓慢 dolly in，移动约 15 cm |
| **场景描述** | 明亮客服中心接待台。浅灰色隔间，白色荧光灯，背景模糊的同事剪影。桌面堆满文件夹，电脑屏幕持续弹出绿色通知弹窗。左侧窗户透入冷白日光。 |
| **人物动作** | Maya 站在台后，左手持电话贴耳，右手横向伸出持第二部电话，双唇同时移动。眼神在屏幕与两部电话间不断切换，额头有轻微汗珠，表情：即将崩溃但仍强撑职业微笑。 |
| **人物台词** | *"Yes— yes, I understand— hold please— no, YOU hold please—"* |

```
=== IMAGE ===
Shot on ARRI Alexa 35, Leica Summilux-C 25mm prime lens.
Movement: slow dolly-in from wide shot to medium-wide over 6 seconds.

SCENE: Bright corporate customer service reception desk. Light gray cubicle panels,
white fluorescent overhead lighting. Background: blurred coworker silhouettes.
Desk covered in stacked manila folders. Computer monitor showing overlapping green
notification popup windows (practical green screen glow). Cold daylight entering
from a window on the LEFT side of frame.

CHARACTER: [MAYA]. Work outfit: cornflower blue button-up shirt, black over-ear
headset with boom microphone, thin gold chain necklace. Standing behind the reception
counter — left hand holding telephone receiver pressed to left ear, right hand
extending a second phone outward. Both lips moving simultaneously. Eyes rapidly
darting between monitor and both phones. Subtle sweat beads on forehead catching
key light as specular highlights.

STAGING: Maya center-frame, body axis facing camera. The two phones create a
horizontal wingspan gesture — her arms form a cross of competing obligations.
Coworker silhouettes in soft background L and R provide depth context.

LIGHTING: Key — ARRI SkyPanel S60-C equivalent, 5600K, upper-left 45°, simulating
window light. Fill — diffused Kino Flo softbox from RIGHT at 1/3 key intensity.
Eye light — small LED panel directly below camera lens, creating a sharp specular
catch-light in the upper-left quadrant of BOTH pupils (must be visible and sharp).
Rim — cool 6500K kicker from behind at 45° right.

PROPS: Two telephone receivers (one corded desk phone, one cordless handset),
stacked manila folders, computer monitor with green popup overlays, black headset.

COLOR: Cold grade (4800K), elevated contrast, subtle cyan-green tint in shadows.
Light film grain. Slight corner vignette.

ACTION: Expression cycles between forced customer-service smile and barely suppressed
panic. Phone cord tangles around right index finger. Head alternates left-right to
address each phone.

STYLE: Photorealistic cinematic. 1960s American PSA aesthetic with modern production
quality. No stylized filters.

=== VOICEOVER ===
VO BEGINS at 0:03 (shot start), simultaneous with music:
TEXT: "Are you tired of useless emotion?"
DELIVERY: Warm, cheerful, as if asking a friend about their weekend — not a
challenge, a genuine inquiry. "Useless" receives a gentle emphasis (slightly longer
vowel). Pace: unhurried, approximately 4 seconds for the full line.
The line COMPLETES within this shot by approximately 0:07.
VO CHARACTER SPEC: See Section 四 VO Voice Spec above.

=== MUSIC ===
Big-band jazz ENTERS simultaneously with VO at 0:03.
Muted trumpet plays a rapid ascending chromatic scale. Dissonant piano chord
clusters layer in immediately. 168 BPM. The music is busy and cluttered —
mirroring Maya's screen full of competing notifications.
Reference: Raymond Scott "Powerhouse" — opening 4 bars.
Volume: -12 dB under VO, full mix when VO is absent.
```

---

#### SHOT 03｜0:09 – 0:12｜中近景 MCU

| 项目 | 内容 |
|------|------|
| **景别** | 中近景（Medium Close-Up），胸部以上至头顶 |
| **摄像机运动** | O'Connor 三脚架静止，光学防抖模拟轻微手持晃动感 |
| **场景描述** | Maya 正面特写。背景虚化的弹窗电脑屏幕，绿色弹窗光反射在 Maya 脸左侧与左肩。 |
| **人物动作** | 双眼在两部电话间快速转动，嘴唇轻声嗫嚅。眼神光在双眼清晰可见。额头汗珠在主光下形成高光。电话线绕住右手食指。 |
| **人物台词** | *"—one moment please— I said HOLD—"* |

```
=== IMAGE ===
Shot on Sony FX3, Leica Summilux-C 75mm prime lens.
Static shot on fluid head tripod. Slight optical stabilizer breathing simulates
gentle handheld quality.

SCENE: Same customer service desk. Background: severely blurred computer monitor
with green popup notifications casting intermittent green practical light on Maya's
LEFT cheek and left shoulder.

CHARACTER: [MAYA]. Same work outfit. Frame: chest to top of head (medium close-up).
BOTH eyes fully visible — LED catch-light sharp in upper-left quadrant of BOTH pupils.
Single sweat bead on forehead catching key light as a bright specular highlight.
Telephone cord wrapped once around right index finger.

STAGING: Maya faces camera directly, filling 60% of frame width. Green monitor glow
creates a secondary split-light effect — warm key from upper-left, cool green fill
from right. This competing light direction externalizes her internal conflict.

LIGHTING: Same continuity as SHOT 02 — Key upper-left 45°, Fill right 1/3 intensity,
Eye light from below-camera. The blurred green monitor creates a secondary practical
fill tinging the RIGHT side of her face — subtly competing with the warm key light.

PROPS: Corded telephone receiver pressed to left ear, second cordless phone in right
hand, black headset boom microphone, telephone cord coiled around right index finger.

COLOR: Same cold 4800K grade. No beauty retouching.

ACTION: Eyes dart rapidly left-right between two phone conversations. Lips form
fragments of words (DIALOGUE: "—one moment please— I said HOLD—"). Brow slightly
furrowed. Shot ends with a quick exhale through the nose — barely contained.

=== VOICEOVER ===
SILENCE. The VO question ("Are you tired of useless emotion?") has already been
delivered and completed in SHOT 02. This shot runs without VO — Maya's chaos IS
the answer to the question. The silence spanning SHOTS 03–05 is intentional.
Do not add any VO here.

=== MUSIC ===
Continuing big-band jazz — strings enter with rapid pizzicato beneath the brass.
Musical texture intensifies slightly from SHOT 02. Dissonance builds.
168 BPM. Volume: full mix (no VO competing).
```

---

#### SHOT 04｜0:12 – 0:15｜中景 MS｜滑轨横移

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot），腰部以上 |
| **摄像机运动** | 80 cm 滑轨向右横移 30 cm，模拟路人经过视角 |
| **场景描述** | 开放式办公室。James 的格子间，桌面被文件和文件夹完全覆盖，只露出一角电脑屏幕。荧光灯直射，后期添加轻微闪烁感。 |
| **人物动作** | James 双手抱起一叠文件，文件从顶部开始滑落。他用下巴试图压住，文件仍继续掉落。他弯腰捡起，另一叠又倒塌。他直起身，眼神空洞，嘴角抽搐。 |
| **人物台词** | 无（哑剧式动作，表情自说） |

```
=== IMAGE ===
Shot on ARRI Alexa 35, Leica Summilux-C 50mm prime lens.
Movement: 80cm slider, 30cm rightward lateral tracking over 3 seconds —
simulating a passing-coworker perspective.

SCENE: Open-plan office. James's cubicle. Desk surface ENTIRELY covered by
stacked manila folders and document towers — only ONE corner of the computer
monitor visible. Fluorescent overhead lighting (slight flicker quality in post-grade).
Neutral beige walls, standard gray office carpet.

CHARACTER: [JAMES]. Work outfit: dark navy suit jacket, white dress shirt, slightly
loosened dark red tie, thin gold wire-rimmed glasses. Frame: waist to head.
Arms wrapped around an impossibly tall, unstable document stack.

STAGING: James positioned center-left of frame as slider moves right, briefly
revealing the full extent of the desk chaos behind him. Camera travels PAST him
from left-to-right — he remains at center as the frame shifts, creating a
momentary parallax reveal of how buried his workspace truly is.

LIGHTING: Same continuity as SHOT 02 — Key upper-left 45°, 5600K. Fill right
softbox 1/3 intensity. Eye light: catch-light visible in BOTH blue-gray eyes
(upper-left quadrant) when he faces camera. Cool rim kicker from behind right.

PROPS: Impossibly tall stack of manila folders, loose white documents, coffee mug
reading "World's Okayest Employee" visible on desk corner, thin gold wire-rimmed
glasses, dark red tie slightly loosened.

COLOR: Same cold 4800K grade. Film grain.

ACTION: James lifts the document stack — papers begin sliding from the top
immediately. He thrusts his chin down to press them. It fails: papers cascade
to the floor. He slowly bends to collect them. As he straightens, a SECOND
independent stack on the desk tips sideways in slow motion. He freezes. Empty
eyes stare at it. A slow, involuntary jaw-twitch — ambiguous between the beginnings
of a laugh and the beginnings of tears. NO DIALOGUE.

=== VOICEOVER ===
SILENCE. Continued VO pause (same silence as SHOT 03). Let James's wordless
physical comedy carry the scene. Do not add any VO.

=== MUSIC ===
Big-band jazz reaches a small peak here — brass section plays a unison dissonant
cluster chord representing peak stress. Full ensemble: trumpet, trombone, strings,
piano all competing. 168 BPM. Slightly cacophonous — the sound of too many things
happening at once.
```

---

#### SHOT 05｜0:15 – 0:18｜极近景快切 ECU MONTAGE × 2

| 项目 | 内容 |
|------|------|
| **景别** | 极近景（Extreme Close-Up）× 2 快切，每个约 1.5 秒 |
| **摄像机运动** | 两个固定特写，后期剪辑快速切换 |
| **场景描述** | 切 1：Maya 双眼——眼白轻微充血，弹窗绿光在瞳孔中反射。切 2：James 双手——颤抖地试图稳住滑落文件。 |
| **人物动作** | 见两切描述 |
| **人物台词** | 无（ECU 无台词） |

```
=== IMAGE ===
TWO SEQUENTIAL EXTREME CLOSE-UP SHOTS (edit in post, each ~1.5 seconds):

— CUT A — MAYA'S EYES (0:15.0 – 0:16.5):
Shot on Sony FX3, Leica Summilux-C 75mm prime lens at minimum focus distance.
Static shot, fluid head tripod.
FRAME: Both eyes only — top of cheekbones to eyebrows. Horizontal composition.
[MAYA]: Deep brown irises. Slight reddening at inner corners of sclera.
Green monitor light reflects as a subtle practical green tint in RIGHT eye.
Sharp LED catch-light visible in upper-left quadrant of BOTH pupils simultaneously.
Shallow depth of field — eyelashes razor-sharp, forehead edge slightly soft.

STAGING: Eyes fill 80% of frame width. The gold scrunchie of her bun is barely
visible at top-right frame edge — the only color accent beyond the brown-green palette.

LIGHTING: Eye light active — clean sharp LED catch-light at upper-left quadrant of
BOTH pupils. Secondary green practical fill from blurred computer monitor at right.
Key light continues from upper-left (cutting a sharp cheekbone highlight).

PROPS: Black over-ear headset boom arm visible at very bottom frame edge.
SCENE: Customer service desk, background completely abstracted / blown out.
COLOR: Cold 4800K. High contrast. Subtle cyan-green fringe on right side.

— CUT B — JAMES'S HANDS (0:16.5 – 0:18.0):
Shot on Sony FX3, Leica Summilux-C 75mm, extreme close-up of hands and papers only.
Static shot. Frame: only hands and document stack — no face, no body in frame.
[JAMES]: Fair-skinned hands, light back-of-hand hair. Gold wedding band on LEFT
ring finger. Both hands trembling while pressing down on a shifting paper stack.
Papers slide DESPITE the pressure — a losing battle, frame by frame.

STAGING: Both hands centered in frame, papers cascading from LEFT side of stack
toward RIGHT — motion direction mimics the direction of entropy. Hands press down
from above, forming a visual "X" of effort vs. gravity.

LIGHTING: Key from upper-left continues — strong paper edge highlights creating
high-contrast document chaos. No eye light (no eyes in frame). Papers catch rim
light from behind creating sharp white-hot leading edges.

PROPS: White manila folders, printed documents with dense text columns, blue
ballpoint pen pinned under James's right thumb.
SCENE: James's office desk surface, background completely blurred.
COLOR: Same cold 4800K grade. Papers white, slightly overexposed at edges.

=== VOICEOVER ===
SILENCE. The VO pause that began in SHOT 03 continues through both cuts.
No voiceover. Dead air. The silence IS the answer to "Are you tired of useless
emotion?" — no words needed when the images speak this clearly.
AT 0:18.0 EXACTLY: Silence ends. The marimba sting strikes. Act 2 begins.

=== MUSIC ===
CUT A: Big-band jazz plays its final cymbal-crash climax — a brief "!" moment.
Full ensemble hits a dissonant chord together on the downbeat of 0:15.
CUT B: Music decrescendos — a rapid diminuendo over 1.5 seconds, tension
winding tight like a coiled spring, preparing for the hard stop.
AT 0:18.0 EXACTLY: Music CUTS TO COMPLETE SILENCE — a hard stop, no fade.
0.2 seconds of pure silence. Then: a single marimba note (G♯4) strikes clean
and bright, held for 2 beats. ACT 2 begins immediately.
```

---

### 🟡 ACT 2：系统介入 [0:18 – 0:36]

---

#### SHOT 06｜0:18 – 0:28｜UI 特写 INSERT｜网站链接 → 鼠标点击进入

| 项目 | 内容 |
|------|------|
| **景别** | 极近景插入（Extreme Close-Up INSERT），屏幕正面平拍 |
| **摄像机运动** | Sony FX3 固定正对屏幕，微型滑轨缓慢向左漂移 5 cm（10 秒内） |
| **场景描述** | 笔记本电脑屏幕特写，浏览器显示搜索结果页——"Self Distill"链接高亮出现。鼠标光标从右侧滑入，悬停于链接上方（链接变蓝、下划线出现），点击，页面跳转加载白色 Self Distill 品牌主页。 |
| **人物动作** | 无真实人物入镜；鼠标光标为场面主体 |
| **人物台词** | 无 |

```
=== IMAGE ===
Shot on Sony FX3, Leica Summilux-C 75mm prime lens.
Movement: micro-slider, 5cm leftward drift over 10 seconds — barely perceptible,
creating a gentle drift that prevents the shot from feeling static.
Frame: screen fills 90% of the image — this is a pure SCREEN INSERT shot.

SCENE: Close-up of a slim laptop screen (silver aluminum chassis, thin bezel).
The screen shows a web browser (clean Chrome-style UI, minimal chrome).
SCREEN CONTENT — sequence unfolds over 10 seconds:

  [0:18 – 0:19]: Browser tab shows a clean search results page.
  Top result reads: "Self Distill — Your Better Self, Delivered | selfdistill.com"
  URL in green below: "selfdistill.com"

  [0:19 – 0:21]: A mouse cursor (standard arrow, white with thin black outline)
  glides in from the RIGHT edge of screen. It moves smoothly toward the
  "Self Distill" search result link. As it hovers, the link underlines and
  turns blue — standard hyperlink hover state.

  [0:21 – 0:21.5]: The cursor changes to a pointer hand. A single click.
  Screen ripple animation from the click point.

  [0:21.5 – 0:23]: Browser loading animation — progress bar fills top edge.
  Brief white flash as page loads.

  [0:23 – 0:28]: Self Distill website HOME PAGE appears in full:
    • Pure white background (#FFFFFF)
    • "Self Distill" wordmark — charcoal (#1A1A1A), serif, letter-spacing +0.02em,
      font-weight 300, centered at 40% of page height
    • Subheading: "Your better self, delivered." — lighter gray, smaller weight
    • CTA button: rounded rectangle (border-radius 24px), charcoal fill,
      white text "Get Started →"
    • The page is clean, minimal, almost clinical in its whiteness

STAGING: The laptop screen is parallel to the camera plane — no keystoning,
no perspective distortion. The screen's clean UI contrasts starkly with the
chaotic office environment glimpsed moments before. This frame is the first
visual breath of clean white space in the entire film.

LIGHTING: One small overhead LED panel (5600K) illuminates the laptop lid from
above — zero screen glare (polarizing filter on lens). The white website UI
provides the dominant light in the frame, casting a clean white glow forward.
No key/fill/rim required — the screen IS the light source.

PROPS: Silver aluminum laptop (thin, modern), mouse cursor on screen, web browser UI,
Self Distill website with full branding elements as specified above.

COLOR: Sharp transition from 4800K chaos grade → 5200K transitional warmth.
Screen white (#FFFFFF) is allowed to clip slightly — it is a source of light,
not a surface to expose correctly.

=== VOICEOVER ===
VO RETURNS at exactly 0:18 — simultaneous with the marimba sting:
TEXT: "Don't let your bad feelings get in your way."
DELIVERY: Warm, authoritative, maternal — like a kind doctor who has just
diagnosed you with something you didn't know was a disease. "Bad feelings" is
said neutrally, as a clinical term. Pace: measured, ~3.5 seconds.
SYNC: Completes as the mouse cursor begins moving toward the Self Distill link.

TEXT (continues without pause): "Introducing Self Distill — our new system
to help you produce the fullest."
DELIVERY: Brand introduction cadence — confident, warm, with a slight editorial
pause on the em-dash after "Self Distill" (0.5 beat). "Produce the fullest" is
delivered with gentle emphasis — slightly stretched vowels, as if savoring
the phrase. Total for this sentence: ~5 seconds.
SYNC: "Self Distill" lands as the cursor clicks the link and the page begins loading.
"Produce the fullest" completes as the full white homepage is visible.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
The single marimba sting (G♯4) at 0:18 resolves into the 1960s corporate jingle
theme — bouncy bass guitar, bright marimba melody, light brushed snare drum.
132 BPM. The music is warm, efficient, slightly too cheerful.
Reference: The Jetsons opening theme, first 8 bars.
Volume: -12 dB under VO.
```

---

#### SHOT 07｜0:28 – 0:32｜中景 MS → 插入镜头 INSERT｜Maya 办公室自拍

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot）→ 特写插入（INSERT）：手机屏幕俯拍 |
| **摄像机运动** | 中景：O'Connor 三脚架固定；INSERT：Sony FX3 正上方 90° 俯拍 |
| **场景描述** | 客服台，Maya 取出手机，打开 Self Distill 应用，切换至前置镜头，举起手机对准自己，端正姿势，拍下自拍照并上传。 |
| **人物动作** | Maya 取出手机→打开 App→举起手机→调整角度→按下快门→屏幕显示"Photo Uploaded ✓" |
| **人物台词** | 无 |

```
=== IMAGE ===
TWO CONNECTED SHOTS (cut together):

SHOT A — Medium Shot:
Shot on ARRI Alexa 35, Leica Summilux-C 50mm prime lens. Static, O'Connor tripod.
Frame: waist to top of head.

CHARACTER: [MAYA]. Same work outfit — cornflower blue shirt, headset (pushed aside
to rest around neck for this shot), thin gold chain necklace. She is at her
customer service desk, now quiet — the phones are not ringing.

STAGING: Maya faces slightly left-of-camera (toward the phone she has placed face
down on the desk). She retrieves a personal smartphone from her shirt pocket with
her right hand. She opens the Self Distill app — we see the white UI briefly
reflected in her eyes as the screen activates. She taps the front-facing camera
icon. She extends her arm outward and upward, phone at selfie height (~30 cm
above eye level). She adjusts her angle once — a small natural correction —
then holds still. Her expression: not a fashion-selfie pout, but a genuine
professional stillness. Curious. Hopeful. Like a passport photo she actually cares about.

ACTION SEQUENCE over 4 seconds:
  0:28 – 0:29: Retrieves phone, opens app
  0:29 – 0:30: Raises arm, composes selfie angle
  0:30 – 0:31: Holds still — the moment before the photo
  0:31 – 0:32: Tap shutter — subtle haptic feedback visible as phone jiggles slightly

LIGHTING: Same customer service desk setup — Key upper-left 45°, Fill right 1/3,
Eye light active (catch-light in BOTH pupils). The phone screen adds a warm white
secondary fill from below as she holds it up — gentle frontal fill softening shadows.

PROPS: Smartphone with Self Distill app open (white UI, front-facing camera mode,
rectangular selfie frame on screen), black headset pushed down around neck,
customer service desk surface visible in background.

SHOT B — INSERT: Phone Screen Overhead:
Shot on Sony FX3, 75mm at macro configuration. Overhead 90° top-down.
Phone lying flat AFTER the selfie is taken. Screen shows:
Self Distill upload confirmation: Maya's face thumbnail in a circle frame,
checkmark animation, text: "Photo Uploaded ✓  Processing your better self..."
A soft progress ring animation begins around Maya's thumbnail.

LIGHTING for INSERT: Small diffused LED panel directly above phone. Zero glare.
The phone screen light is the primary illumination on the desk surface.

COLOR: 5200K — transitional warmth, cleaner than Act 1.

=== VOICEOVER ===
VO at 0:28:
TEXT: "Upload yourself in seconds—"
DELIVERY: Slightly brisk — the cadence of a product feature list. "Upload yourself"
is spoken as naturally as "upload a file." The em-dash creates a breath before the
next phrase continues in SHOT 09. Approximately 3 seconds for this phrase.
SYNC: "seconds—" lands exactly as Maya taps the shutter — the verbal promise and
visual proof arrive simultaneously.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
Corporate jingle continues — marimba melody brightens slightly as the "upload"
moment arrives. A brief ascending 3-note marimba figure (E4→F♯4→A4) punctuates
the shutter tap — a cheerful digital confirmation sound woven into the music.
132 BPM. Volume: -12 dB under VO.
```

---

#### SHOT 08｜0:32 – 0:36｜中景 MS → 插入镜头 INSERT｜James 办公室自拍

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot）→ 特写插入（INSERT）：手机屏幕俯拍 |
| **摄像机运动** | 中景：O'Connor 三脚架固定；INSERT：Sony FX3 正上方 90° 俯拍 |
| **场景描述** | 办公室格子间，James 在文件堆旁取出手机。他不太习惯自拍——先摘下眼镜，又重新戴上，调整手机角度两三次，最终拍下照片。动作稍显笨拙但认真。 |
| **人物动作** | James 取出手机→摘眼镜→重新戴上→调整角度→按快门→屏幕显示上传确认 |
| **人物台词** | 无 |

```
=== IMAGE ===
TWO CONNECTED SHOTS (cut together):

SHOT A — Medium Shot:
Shot on ARRI Alexa 35, Leica Summilux-C 50mm prime lens. Static, O'Connor tripod.
Frame: waist to top of head, slight 30° right-angle (showing James from his
left side so we see both his face and the phone he's raising).

CHARACTER: [JAMES]. Same work outfit — dark navy jacket, white shirt, dark red
tie (now slightly retied — less disheveled than earlier). He is at his cubicle.
The document stacks are still present but no longer falling.

STAGING: James stands (not sits) behind his desk. He removes his smartphone from
his jacket inner pocket. He looks at the screen — the Self Distill app is already
loading. He taps the front-facing camera. He raises the phone — arm fully extended,
slightly too high (he's not sure of the optimal angle). He removes his glasses with
his free left hand, looks at the blurry phone screen, puts the glasses back on,
adjusts the phone angle 3 centimeters lower. He exhales slightly. Holds the phone
steady. A long pause before the shutter — a man committing to something he does
not fully understand. Then he taps it.

His expression DURING the photo: unexpectedly sincere. The slight ruddiness in
his cheeks. The LED catch-light in both blue-gray eyes (upper-left quadrant).
A very small, genuine smile — not performed.

ACTION SEQUENCE over 4 seconds:
  0:32 – 0:33: Retrieves phone, fumbles with app slightly
  0:33 – 0:34: Removes glasses, peers at screen, replaces glasses
  0:34 – 0:35: Raises phone, adjusts, finds angle
  0:35 – 0:36: Holds still, takes the selfie — subtle phone jiggle on tap

LIGHTING: Same office cubicle setup — Key upper-left 45°, 5600K. Fill right softbox.
Eye light active — catch-light in BOTH blue-gray eyes must be visible and sharp in the
moment the photo is taken. Computer monitor behind provides secondary cool white fill.

PROPS: Smartphone with Self Distill app front-facing camera mode, thin gold
wire-rimmed glasses (removed and replaced during action), document stacks in
background (still present, stabilized), coffee mug on desk corner.

SHOT B — INSERT: Phone Screen Overhead:
Shot on Sony FX3, 75mm macro. Overhead 90° top-down.
Phone lying flat after selfie. Screen: James's face thumbnail in a circle, same
upload confirmation as Maya's: "Photo Uploaded ✓  Processing your better self..."
Progress ring animation around his thumbnail — mirror of Maya's SHOT 07 insert.

COLOR: 5200K, warmth building. The white phone screen UI provides a clean visual
anchor — every shot of the website/app should feel bright, clinical, reassuring.

=== VOICEOVER ===
SILENCE during SHOT 08. The phrase "Upload yourself in seconds—" completed at the
end of SHOT 07. This shot runs without VO — James's awkward determination speaks
for itself. The visual rhyme (same action, different person) needs no narration.
Do not add any VO.

=== MUSIC ===
Corporate jingle continues — same bouncy 132 BPM. The ascending marimba confirmation
figure repeats (E4→F♯4→A4) on James's shutter tap, matching the one on Maya's.
This musical echo reinforces the visual rhyme between the two selfie shots.
Volume: full mix (no VO competing).
```

---

### 🟢 ACT 3：数字处理 [0:36 – 0:46]

---

#### SHOT 09｜0:36 – 0:42｜全屏 UI 界面｜Maya 数字化处理

| 项目 | 内容 |
|------|------|
| **景别** | 全屏 UI 界面（CG / 动态图形），分屏构图：左右各半 |
| **摄像机运动** | 虚拟摄像机缓慢向前推进（z 轴 dolly in，约 5% 缩放），6 秒内 |
| **场景描述** | Self Distill 网页界面全屏占据画面：左半屏 Maya 的等比例全身 3D 扫描图像缓慢旋转（360°），右半屏实时生成由绿色 0 和 1 交错密布组成的 Maya 数字轮廓，从下向上逐渐填满。 |
| **人物动作** | 无真实人物；左侧 Maya 3D 模型旋转；右侧数字轮廓自底部向顶部生成 |
| **人物台词** | 无 |

```
=== IMAGE ===
CG / VFX motion graphic render. Virtual camera equivalent to Leica Summilux-C 50mm
field of view. Slow virtual dolly-in: z-axis push, approximately 5% scale increase
over 6 seconds — screen elements feel like they're approaching the viewer.

SCENE: Full-screen Self Distill web application interface.
Background: Pure white (#FFFFFF). UI elements styled per brand spec.

LAYOUT — 50/50 SPLIT SCREEN:

LEFT PANEL (labeled "Your Scan"):
  • Full-body 3D photogrammetry scan of [MAYA] — rendered in clean CG.
  • The model maintains ALL Maya character details: afro puff bun, cornflower
    blue button-up shirt, gold scrunchie, thin gold necklace.
  • The 3D model rotates slowly clockwise — approximately 60° of rotation
    visible across 6 seconds (from front-facing to profile, still turning).
  • Subtle point-cloud or mesh wireframe visible at body edges.
  • Lighting on the 3D model: neutral studio HDRI — even, clinical, no drama.
  • The model's feet rest on a small shadow plane.

RIGHT PANEL (labeled "Your Digital Self  ██████░░ 74%"):
  • Pure black background (#000000) in this half only.
  • Maya's SILHOUETTE is being constructed from WITHIN by dense, flowing
    green binary digits (alternating 0 and 1, 0 and 1, in varying font sizes
    6pt–12pt, tight leading, filling every pixel of the silhouette).
  • The digits glow green (#00FF41 — Matrix green), with slight bloom effect.
  • Construction proceeds FROM BOTTOM TO TOP — feet and legs visible first,
    torso filling in mid-shot, head completing near the end of the 6 seconds.
  • The digits flow gently — not static type, but softly animated streaming
    binary (like a contained, shaped Matrix code waterfall).
  • Silhouette edges are sharp — there is a clear boundary between the
    bright-green digit Maya and the pure black panel background.
  • At the top of the right panel: progress bar and percentage counter,
    climbing from 0% to 100% across the 6 seconds.

CENTER DIVIDER: A thin 1px charcoal (#1A1A1A) vertical line separates panels.
A small Self Distill wordmark in charcoal floats centered above the split screen.

STAGING: Both panels are simultaneously active — the organic 3D model on the left
and the digital construction on the right create a visual argument about identity.
What is "better"? The question is embedded in the composition.

LIGHTING: CG render — neutral studio HDRI for the 3D model left panel. The right
panel is entirely self-lit by the green digit glow. No physical lighting rig.

PROPS: UI elements — progress bar, percentage readout, panel labels, Self Distill
wordmark. No physical props.

COLOR: Left panel is 5200K-equivalent neutral warmth. Right panel is purely
black + #00FF41 green — no color correction applied to that half.

=== VOICEOVER ===
VO RETURNS at 0:36 (resolving the em-dash from SHOT 07):
TEXT: "—and we'll make you better, faster, stronger."
DELIVERY: The em-dash pickup from SHOT 07 ("Upload yourself in seconds—") resolves
here. "Better, faster, stronger" — three adjectives with equal rhythmic spacing,
each given precise equal weight. The digital Maya silhouette filling in as the words
land creates a literal visualization of the claim. Deliver with complete sincerity.
SYNC: "Better" — Maya's legs visible. "Faster" — torso fills in. "Stronger" —
head completes, progress bar reaches 100%.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
At 0:36: Corporate jingle hybridizes with electronic synthesis.
Kraftwerk-style synthesizer bass (square wave, minor key) enters BENEATH the
existing jingle marimba — the two musics overlap: the organic cheerfulness of the
jingle vs. the cold precision of the synthesizer. Neither dominates.
Three playful-yet-electronic staccato hits punctuate "better / faster / stronger."
132 BPM. Volume: -12 dB under VO.
```

---

#### SHOT 10｜0:42 – 0:46｜全屏 UI 界面｜James 数字化处理

| 项目 | 内容 |
|------|------|
| **景别** | 全屏 UI 界面（CG / 动态图形），分屏构图：左右各半 |
| **摄像机运动** | 虚拟摄像机静止，4 秒内 |
| **场景描述** | 与 SHOT 09 完全同构界面，但主体换为 James：左半屏 James 的全身 3D 扫描缓慢旋转，右半屏生成由绿色 0 和 1 构成的 James 数字轮廓，进度条快速完成。 |
| **人物动作** | 无真实人物；James 3D 模型旋转；数字 James 自底部向顶部生成 |
| **人物台词** | 无 |

```
=== IMAGE ===
CG / VFX motion graphic render — IDENTICAL interface design to SHOT 09.
Virtual camera equivalent: Leica Summilux-C 50mm field of view. Static virtual camera.

SCENE: Full-screen Self Distill web application. Same 50/50 split interface.

LEFT PANEL (labeled "Your Scan"):
  • Full-body 3D photogrammetry scan of [JAMES].
  • All James character details maintained: navy jacket, white shirt, dark red tie,
    thin gold wire-rimmed glasses.
  • Slow clockwise rotation — approximately 45° visible over 4 seconds.
  • Same mesh wireframe edge treatment as Maya's scan.

RIGHT PANEL (labeled "Your Digital Self  ██████████ 100%"):
  • Same pure black background (#000000).
  • James's silhouette — taller, broader-shouldered than Maya's — being constructed
    by the same dense green binary digit stream (#00FF41).
  • Because this is the SECOND person processed, the progress bar starts at ~40%
    (already partially processed) and fills to 100% over the 4 seconds — slightly
    faster than Maya's, as if the system has warmed up.
  • The binary digits adopt James's proportions: the silhouette is clearly
    his height (~180 cm implied), with the rectangular glasses rendered in
    binary along the face plane of the silhouette.

STAGING: The visual symmetry between SHOT 09 and SHOT 10 reinforces the system's
universality — it processes everyone with identical clinical precision.
The only variable is the human silhouette being filled.

LIGHTING: Same CG render — neutral HDRI left, self-lit green right.
PROPS: Same UI elements. Progress bar completes to 100% and holds.
COLOR: Same split — neutral left, black + #00FF41 right.

=== VOICEOVER ===
SILENCE during SHOT 10. The VO phrase "better, faster, stronger" completed in SHOT 09.
This shot runs without narration — the visual rhyme of James's digital construction
(mirroring Maya's) is its own argument. No words needed.
Do not add any VO.

=== MUSIC ===
Electronic-jingle hybrid continues — the synthesizer bass now slightly more
prominent than the marimba. The jingle melody echoes distantly, as if being
processed through the same digital system that's processing James.
At the 100% progress completion (end of shot): a brief synthesizer resolution
tone — a digital "done" sound. Not a marimba; a synthesizer confirmation.
132 BPM. Volume: full mix.
```

---

### 🔵 ACT 4：数字替身 [0:46 – 0:53]

---

#### SHOT 11｜0:46 – 0:50｜中景 MS｜数字替身 Maya 接电话

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot），腰部以上，正面构图 |
| **摄像机运动** | 虚拟摄像机静止，极缓慢弧形向右移动约 5°（弧形轨迹，4 秒内） |
| **场景描述** | 纯黑背景。Maya 的全身轮廓完全由流动的绿色 0 和 1 构成——数字形态的 Maya 正在接听电话，动作流畅自如，无任何情绪压力的迹象。 |
| **人物动作** | 数字 Maya 将电话放至耳边，另一只手自然垂于身侧。动作平稳、精确、无表情。 |
| **人物台词** | 无 |

```
=== IMAGE ===
CG / VFX render. Virtual camera equivalent: Leica Summilux-C 50mm field of view,
T2.0 aperture equivalent. Virtual arc dolly: slow 5° rightward arc over 4 seconds —
the subtle movement implies a world that can be observed from multiple angles.

SCENE: Pure black void (#000000). No floor, no walls, no environmental context.
The digital Maya figure exists in absolute darkness, illuminated only by its own
green glow.

CHARACTER: [MAYA] — DIGITAL DOUBLE.
The complete human figure of Maya — standing, framed waist-to-head — is rendered
entirely from dense flowing green binary digits (0s and 1s, alternating, in tight
6pt–12pt type). The digits flow and shift continuously, like contained data streams
forming a living shape. The silhouette is unmistakably Maya:
  • Afro puff bun silhouette at top — the hair volume is rendered in slightly
    larger, faster-moving digits than the face
  • Round face shape, high cheekbones suggested by digit density variation
  • Cornflower blue shirt area rendered in slightly lighter green tone (subtle
    tonal variation within the #00FF41 palette to suggest clothing)
  • Gold chain necklace: a single bright horizontal line of concentrated digits
  • Medium build, approximately 165 cm implied proportions

The digits throughout her body GLOW (#00FF41, 75% opacity) with a soft bloom
radius of approximately 4px — she radiates a gentle green luminescence into the
surrounding black. The outer edges of her silhouette have a subtle fringe of
diffused digits, like static electricity.

ACTION: The digital Maya holds a telephone handset (also rendered in green binary
digits — the phone is part of her digital world) pressed to her LEFT ear.
Her posture is upright, composed, perfectly still except for the flowing digits.
She is HANDLING THE CALL — whatever the caller says, she is responding with
seamless efficiency. No stress. No furrow. No sweat. No juggling of two phones.
One call. One solution. Complete.

Her face (rendered in digits) shows no expression — not because she is unhappy,
but because emotion has been externalized. The absence of visible stress IS the
product's promise made visible.

STAGING: Digital Maya occupies center-frame, approximately 60% of frame height.
The surrounding black is deep and absolute — no ambient light, no ground shadow.
The arc of the virtual camera from left to right gives her figure a slight sense
of three-dimensionality: as the angle shifts, the density of the front-facing
digits becomes slightly sparser, revealing (just barely) that the figure has depth.

LIGHTING: Self-lit by internal green glow (#00FF41). No external light sources.
The bloom effect creates a halo approximately 2cm beyond the silhouette edge.
The virtual camera catches this glow as a lens bloom effect — giving the shot
a slight otherworldly aura without becoming garish.

PROPS: Green-binary telephone handset (same design as desk phone in SHOTS 02–03,
but rendered entirely in the same green-digit aesthetic as the figure).

COLOR: Pure black (#000000) background. Monochromatic green (#00FF41) figure.
No other colors in frame. The contrast is absolute. This shot should feel like
looking at a heart monitor or a radar display — efficient, inhuman, exact.

=== VOICEOVER ===
VO RETURNS at 0:46:
TEXT: "Free yourself—"
DELIVERY: The warmest, most intimate the VO has been — softer, almost whispered,
as if sharing a secret gift. "Free" carries the fullest weight of the entire PSA;
it is the emotional payoff of everything that came before. Pace slows slightly.
The em-dash creates a deliberate 0.5-beat pause before the next shot completes
the thought.
SYNC: "Free yourself—" lands as the digital Maya settles into her phone call —
movement and word embody each other.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
At 0:46: Electronic-jingle hybrid dissolves. Philip Glass-influenced minimalist
piano enters — a slow, repeating 4-note figure (D4–E4–G4–A4) in sparse,
even rhythm. Simple. Clean. Slightly melancholy.
Underneath: a very faint marimba echo (reverb tail from the jingle theme)
fading away in the distance.
100 BPM. Volume: -10 dB under VO, -6 dB during silent portions.
```

---

#### SHOT 12｜0:50 – 0:53｜中景 MS｜数字替身 James 搬文件

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot），腰部以上，正面偏左 15° 角 |
| **摄像机运动** | 虚拟摄像机静止，3 秒内 |
| **场景描述** | 纯黑背景。James 的全身由流动绿色 0 和 1 构成，正在轻松搬运一叠文件。动作高效、精准，文件整齐服帖，没有任何一页滑落。 |
| **人物动作** | 数字 James 双臂抱一叠文件，步伐平稳向右走过画面。文件纹丝不动。 |
| **人物台词** | 无 |

```
=== IMAGE ===
CG / VFX render. Virtual camera equivalent: Leica Summilux-C 50mm, T2.0.
Static virtual camera, slight 15° leftward offset from James's axis —
giving a 3/4 frontal view that allows us to see both his face and the
document stack clearly.

SCENE: Same pure black void as SHOT 11. No environment. Digital space only.

CHARACTER: [JAMES] — DIGITAL DOUBLE.
James's complete figure rendered in dense flowing green binary digits (#00FF41),
same aesthetic as digital Maya in SHOT 11. Key identifying silhouette features:
  • Taller proportions (~180 cm implied)
  • Broad-shouldered, slightly heavyset frame suggested by digit density
  • Square jaw and prominent brow silhouette visible in digit pattern
  • Short hair rendered in tight, fast-moving small digits at top
  • Rectangular glasses: two bright horizontal digit-clusters on the face plane
  • Navy jacket area rendered with slightly denser digit concentration
  • Gold wedding band: a bright ring of concentrated digits on LEFT ring finger

Same glow aesthetic: #00FF41, 75% opacity, 4px bloom, soft silhouette fringe.

ACTION: Digital James walks from LEFT to RIGHT across the frame — a deliberate,
measured pace. He carries a large stack of documents (also rendered in green binary).
The document stack is PERFECTLY aligned — no papers slide, no edges misalign.
His posture is straight, his grip is secure, his movement is efficient.
The contrast with SHOT 04's cascading chaos is absolute and intentional.
He crosses the frame and exits RIGHT at the end of the shot.

STAGING: James enters frame from center-left at the start, walks to right edge
over 3 seconds. His figure passes through the frame at a steady pace — unhurried,
not rushed. The papers in his arms don't move relative to each other, even slightly.

LIGHTING: Same self-lit green glow as SHOT 11. No external sources. Bloom halo.
PROPS: Green-binary document stack (same manila folder proportions as SHOTS 04–05,
rendered entirely in digit aesthetic). Gold wedding band visible as a bright digit ring.

COLOR: Same pure black + #00FF41 monochrome. Absolute contrast.

=== VOICEOVER ===
VO CONTINUES from SHOT 11 (the em-dash resolves):
TEXT: "—right now, right away."
DELIVERY: These three words complete "Free yourself — right now, right away."
"Right now, right away" has a gentle insistence — the rhythm of the words
(right now / right a-WAY) is slightly more rhythmic, nearly song-like, matching
the Philip Glass figure beneath. Deliver with complete warmth and conviction.
SYNC: "Right now, right away" lands over digital James's efficient walk —
the liberation is visible in his perfect, unfumbling stride.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
Minimalist piano continues — the 4-note figure repeats. At "right now, right away"
a single soft vibraphone note (C5) punctuates the final word "away" — bright,
clean, resonating. The note decays slowly into the next shot.
100 BPM. Volume: -12 dB under VO.
```

---

### 🟠 ACT 5：解脱 [0:53 – 0:57]

---

#### SHOT 13｜0:53 – 0:57｜中景 MS｜Maya 与 James 并排，真人回归

| 项目 | 内容 |
|------|------|
| **景别** | 中景（Medium Shot），腰部以上，双人横构图 |
| **摄像机运动** | DJI Ronin 4D 极缓慢推进（dolly in），4 秒推进约 20 cm |
| **场景描述** | 真实办公室环境，Maya 与 James 并排坐于同一张桌子旁（或沙发区），面带自然微笑，直视镜头。背景：暖光明亮的办公室，干净整洁——与 Act 1 的混乱形成对比。 |
| **人物动作** | 两人并肩而坐，肩膀轻微相触。均看向摄像机。表情：放松、满足，带着真实的轻盈感。 |
| **人物台词** | 无 |

```
=== IMAGE ===
Shot on ARRI Alexa 35, Leica Summilux-C 50mm prime lens.
Movement: DJI Ronin 4D — extremely slow dolly-in from medium-wide to medium shot.
Travel: ~20cm over 4 seconds. The push is barely perceptible — it should feel
like the camera is leaning in, not advancing.

SCENE: An office common area or break room — a different space from the cubicle
and the customer service desk. Clean, warm, well-lit. A small round table or
a comfortable seating area. Background: blurred warm-toned office interior —
bookshelves, a plant, large windows letting in warm golden afternoon light.
The space is intentionally tranquil — the opposite of Act 1.

CHARACTER A: [MAYA]. Same work outfit (cornflower blue shirt, gold scrunchie,
thin gold chain). She has removed her headset entirely — it is not in frame.
Her posture is relaxed: shoulders down, hands loosely in lap.

CHARACTER B: [JAMES]. Same work outfit (navy jacket, white shirt, dark red tie —
now properly knotted and centered). His glasses are on. Document stack: nowhere
visible. His hands are rested on the table surface, relaxed.

STAGING: Maya on LEFT, James on RIGHT. Their inside shoulders are approximately
10–15 cm apart — close but not touching. Both face the camera directly. They are
not posed stiffly; there is a natural, easy quality to their proximity — two people
who have experienced something together and arrived at the same place. Neither looks
at the other; both look gently, directly at the lens.

LIGHTING: ARRI SkyPanel S60-C equivalent, 5600K, upper-left 45° — same rig as
throughout the film, but now the grade is warm and the contrast is soft. Warm
golden afternoon light through windows provides additional natural fill from the
right. Eye light active — LED catch-light in the upper-left quadrant of BOTH
pupils of BOTH characters simultaneously. Rim light from behind at 45° right —
soft golden rim, not the cool kicker of Act 1.

PROPS: Clean round table surface. A coffee mug (plain, white) in front of James.
Maya's hands are empty. Background: blurred potted plant, bookshelf, windows with
warm ambient glow.

COLOR: 5600K — warm, open, naturally beautiful. Soft contrast. No chromatic
aberration. No vignette. No film grain. This shot should feel CLEAN — the visual
relief of a world that has been resolved.

ACTION: Both subjects hold a natural, easy smile — not a performance. The smile
is the quiet kind that arrives after something difficult has passed. Maya's smile
is slightly broader; James's is more contained but equally genuine. Neither moves
significantly during the 4-second shot — they simply ARE. Present. Relieved. Whole.

=== VOICEOVER ===
VO at 0:53:
TEXT: "Self Distill —"
DELIVERY: Single deepest, warmest moment in the VO. The brand name is spoken
reverently — not with fanfare, but with the quiet satisfaction of something earned.
The em-dash creates a meaningful 0.5-beat pause.
SYNC: "Self Distill" lands as Maya and James come into focus together.

TEXT (continues): "let us do the feelings for you."
DELIVERY: The warmest, lowest, most intimate moment in the entire VO. "Feelings"
receives the fullest emphasis — a slight lengthening of the vowel. The sentence
ends on a very gentle upward inflection — not a question, but a smile. As if she
is personally offering to carry their emotional weight.
SYNC: "...for you." completes as the dolly-in reaches its final position.
VO CHARACTER SPEC: See Section 四 VO Voice Spec.

=== MUSIC ===
At 0:53: Minimalist piano dissolves. Full warm orchestral convergence — strings,
French horn, piano arrive together on a sustained Bmaj7 chord. The chord holds
and softens. The music is momentarily full, then immediately settles into warmth.
At 0:55: A gentle resolution — strings sustain a single held note. The music
becomes very simple and very warm for the final 2 seconds of this shot.
110 BPM. Volume: -10 dB under VO.
```

---

### ⬜ ACT 6：CTA 行动召唤 [0:57 – 1:00]

---

#### SHOT 14｜0:57 – 1:00｜字卡 TITLE CARD（CTA）

| 项目 | 内容 |
|------|------|
| **景别** | 字卡（动态字幕，纯白背景） |
| **摄像机运动** | 无 |
| **场景描述** | 纯白背景。Self Distill 品牌 Logo，副标题 *"let us do the feelings for you."*，CTA 按钮"Start a Free Trial Now →"，右下角极小免责声明。 |
| **人物动作** | 无 |
| **人物台词** | 无 |

```
=== IMAGE ===
Motion graphic title card (not live action).
Background: Pure white (#FFFFFF). No texture, no grain.

SHOT TYPE: Motion graphic. No camera. No lens. No live action.
LIGHTING: None — pure white background with typography only.
PROPS: Typography, CTA button, fine print — all elements described below.
STAGING: Centered vertical stack composition. Elements appear in sequence.
SCENE: Brand identity space — pure void of white.

LAYOUT (centered, vertical stack, appearing in sequence):
  ① Self Distill wordmark logo (simple sans-serif, dark charcoal #1A1A1A)
     — 40% of frame width, letter-spacing +0.02em, font-weight 300.
     Fades in over 0.5 seconds.
  ② Tagline in lighter weight italic:
     "let us do the feelings for you."
     — charcoal, 60% of logo size. Types in character by character over 1.2 seconds.
     NOTE: "feelings" is PLURAL — do not use "feeling" (singular).
  ③ CTA button: rounded rectangle (border-radius: 24px), charcoal fill, white text:
     "Start a Free Trial Now →"
     — slides in from below over 0.3 seconds. Click ripple animation on loop.

BOTTOM-RIGHT CORNER: Small print (light gray, ~8pt equivalent):
"*Side effects may include loss of all emotional capacity. Self Distill Inc.
 is not responsible for your feelings — you are."

ANIMATION TOTAL: 2 seconds build, then 1 second static hold.

COLOR: Pure white. Charcoal typography. No other colors. Brand-pure.

=== VOICEOVER ===
SILENCE. The full VO sentence "Self Distill — let us do the feelings for you."
completed at the end of SHOT 13. This title card runs without narration.
The tagline on screen echoes the VO from SHOT 13 — spoken word becomes written word.
Do not add any VO.

=== MUSIC ===
Brand jingle: two-note ascending motif on clean studio piano.
Notes: D4 (beat 1) → G4 (beat 2) — "Self — Distill." Played once, cleanly.
Immediately followed by a 3-second natural reverb tail that fades to complete
silence. No other instruments. No percussion. Just the piano and its decay.
This is the last sound before silence.
```

---

## 五、全片声音设计 SOUND DESIGN OVERVIEW

> 以下为总体参考表，各 shot 提示词中已包含对应的精确 VO 和音乐描述。

### 画外音 VO 全文与时间码对照

| 时间码 | VO 原文 | 所在 Shot | 语调备注 |
|--------|---------|----------|----------|
| 0:03 – 0:08 | *"Are you tired of useless emotion?"* | SHOT 02 | 亲切提问，"useless"轻重读 |
| **0:08 – 0:18** | **（VO 静默 10 秒）** | SHOTS 03–05 | 沉默是答案，让混乱自说 |
| 0:18 – 0:22 | *"Don't let your bad feelings get in your way."* | SHOT 06 | 治疗师口吻，温和权威 |
| 0:22 – 0:28 | *"Introducing Self Distill — our new system to help you produce the fullest."* | SHOT 06 | 品牌介绍，破折号停顿，"fullest"加重 |
| 0:28 – 0:32 | *"Upload yourself in seconds—"* | SHOT 07 | 产品功能节奏，em-dash 断句 |
| **0:32 – 0:36** | **（VO 静默 4 秒）** | SHOT 08 | James 自拍画面自说，无需旁白 |
| 0:36 – 0:42 | *"—and we'll make you better, faster, stronger."* | SHOT 09 | 三词等间距强调，与数字轮廓生成同步 |
| **0:42 – 0:46** | **（VO 静默 4 秒）** | SHOT 10 | James 数字化画面自说 |
| 0:46 – 0:49 | *"Free yourself—"* | SHOT 11 | 最温柔，几乎低语，em-dash 停顿 |
| 0:50 – 0:53 | *"—right now, right away."* | SHOT 12 | 节奏感，轻微上扬 |
| 0:53 – 0:55 | *"Self Distill —"* | SHOT 13 | 最深沉，品牌名如仪式，em-dash 停顿 |
| 0:55 – 0:57 | *"let us do the feelings for you."* | SHOT 13 | 最低沉温暖，"feelings"拉长，句末微笑上扬 |
| **0:57 – 1:00** | **（无 VO，CTA 画面静默）** | SHOT 14 | 品牌 jingle 双音收尾 |

---

### 人物台词全文

| 角色 | 时间码 | 台词 | 所在 Shot |
|------|--------|------|----------|
| Maya | 0:03–0:09 | *"Yes— yes, I understand— hold please— no, YOU hold please—"* | SHOT 02 |
| Maya | 0:09–0:12 | *"—one moment please— I said HOLD—"* | SHOT 03 |

---

### Self Distill UI 视觉规格（全片一致）

> 适用于 SHOTS 06、07（INSERT）、08（INSERT）、09、10。

| 元素 | 规格 |
|------|------|
| 背景色 | 纯白 #FFFFFF |
| 品牌字标 | "Self Distill"，炭色 #1A1A1A，letter-spacing +0.02em，font-weight 300 |
| CTA 按钮 | 圆角矩形（border-radius 24px），炭色填充，白色文字 "Get Started →" |
| 进度条 | 浅灰轨道 + 炭色填充，左→右方向 |
| 数字色 | 绿色 #00FF41（Matrix green），仅用于数字替身段 |
| 上传确认 | 圆形头像缩略图 + 旋转进度环 + "Processing your better self..." |
