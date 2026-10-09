# SmartBYD voice models

Whisper model files that the SmartBYD app downloads once after it is installed (the APK no longer carries them).

| File | What | Licence | Source |
|---|---|---|---|
| `whisper-ar-base-q8_0.bin` | OpenAI Whisper "base", multilingual (Arabic / English passes), ggml q8_0 | MIT | ggerganov/whisper.cpp (Hugging Face) |
| `whisper-ar-small-q8_0.bin` | OpenAI Whisper "small", multilingual, ggml q8_0 — the optional "accurate" model | MIT | ggerganov/whisper.cpp (Hugging Face) |
| `whisper-ckb-base-q8_0.bin` | razhan/whisper-base-ckb, Whisper base fine-tuned on Central Kurdish, converted with whisper.cpp and quantised to q8_0 | Apache-2.0 | razhan/whisper-base-ckb (Hugging Face) |

SHA-256 (the app verifies these):

```
c577b9a86e7e048a0b7eada054f4dd79a56bbfa911fbdacf900ac5b567cbb7d9  whisper-ar-base-q8_0.bin
49c8fb02b65e6049d5fa6c04f81f53b867b5ec9540406812c643f177317f779f  whisper-ar-small-q8_0.bin
8dc2b444257c0d5f615380cc6d0377483440468b2e09a9ff131b1d3ec5a472ad  whisper-ckb-base-q8_0.bin
```

Release `v1` holds the files; the app's manifest (`voice/ModelFiles.kt`) names the release and the checksums.
