# Prompt Skeleton (EN, Ref2VA) · 变装蒙太奇段骨架

> 用法：按 h3pro-agent §2.4 官方六段式填写；正文全英文，只有 intake 定版的对白（若有）进 `<d>[Chinese] …</d>`。派发前跑 HLSSS 同款中文自检（剥掉 `<d>…</d>` 后中文字符数 = 0）。占位照铁律 T：老公永远前景一侧手持自拍，老婆中景展示，不越轴。

```text
subject_definitions:
<Subject 1> is the bald husband from <Picture 1>: completely bald head, no hat, no hair; his face, facial bone structure and age are fully identical to the large headshot panel of <Picture 1>. He wears plain everyday clothes ([per-shot plain outfit]) and holds the phone camera himself at arm's length.
<Subject 2> is the beautiful wife from <Picture 2>: her face, features and age are fully identical to the large headshot panel of <Picture 2>; long black hair; her outfit, hairstyle and makeup change per shot exactly as defined in each shot below ([look list]).
<Picture 3> is the location/look anchor image for this segment.

summary:
[reference generation] <Subject 1> holds a selfie camera in the foreground while <Subject 2> poses in a rapid glamorous outfit-change montage, hard cuts between looks.

retention_analysis:
<Subject 1>: fully_preserved
<Subject 2>: fully_preserved
<Picture 3>: partially_preserved

detailed_description:
Handheld selfie video, vertical 9:16, natural daylight, realistic phone-camera look with slight handheld shake. In every shot <Subject 1> stays in the [left] foreground, partially cropped, holding the camera; <Subject 2> stands in the midground. The husband never changes his goofy proud expression style; only the wife's look and the backdrop change, with a hard cut at every shot.
[Shot 1] Full-body view: <Subject 2> in [Look 1: dress/hairstyle/makeup/accessories/shoes], standing at [village backdrop 1]; she [pose: hand on chest / slight sway], looking into the camera with red lips and a confident smile. <Subject 1> smirks proudly in the foreground. Lips of both stay naturally closed, no speaking.
[Shot 2] At 00:02.000 Hard cut. <Subject 2> in [Look 2], at [backdrop 2]; she [pose: leaning on his shoulder]. <Subject 1> [goofy face variant: chin up / wide grin].
... (repeat per look, ~1.6s each; final shot = finale pose: the wife hugs <Subject 1> from the side, both smile into the camera and hold the pose.)

overall_soundscape:
Pure environmental foley only: light wind, distant village ambience, soft fabric rustle and footsteps on concrete, only natural white noise.

non_diegetic_music:
N/A

negative prompts: music, background music, bgm, soundtrack, score, melody, tune, instrumental, singing, song, musical instruments, rhythm, dialogue, speaking, talking, voiceover, narration, humming, mouth open, lip-sync, hair on bald head, hat, cap, wig, face morphing, outfit change on husband, gibberish text, subtitles, watermark, logo
```

## 填写要点
- 每套 Look 必须逐项写全：裙装款式/颜色、发型、妆（红唇）、配饰、鞋——与用户确认过的造型锚点图逐项对齐，少一项就容易漂。
- 老公每镜只许换"土味日常装小变体＋搞怪表情"，**绝不许变帅、绝不许长头发/戴帽**（negative 已封堵 hair/hat/cap/wig）。
- 钩子段（素颜段）单独一段生成：结构同上但只有 1 个 Shot，老婆为素颜、乱发、家居服，场景为室内/家门前，并按 intake 决定是否有一句对白。
