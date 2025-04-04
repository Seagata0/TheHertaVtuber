# Generative AI Classs's Project - The Herta Vtuber<br>Group 7 (Bojongsantos Oost-indische Compagnie)<br>
![BOC 320](https://github.com/user-attachments/assets/5b04e5ed-6524-4bda-a7d8-6edea5df1511)

## First Project(Generative AI Prompting) :
- AI Cover Video : https://www.youtube.com/watch?v=4tJADqRNzek (Audio 2:58(2 Minutes 58 Seconds)) <br>
- LLM : ChatGPT & DeepSeek
- TTS : Edge-TTS (ja-JP-NanamiNeural)
- Audio Model : Refer to the 2nd Project
- Total Prompt : 41 (Will be used for the second project)
  - Text Prompt : 9 ((https://chatgpt.com/share/67eab298-9814-800b-bb02-8861e6c70c29) & Since Deepseek Cant be shared, the output is shown as "Prompt for TTS" below)
  - Audio Prompt : 24 (Output Can Be checked in /Audio/TTS)


## Second Project (Finetuning) :
- RVC Model : [Seagata/TheHerta_RVCModel](https://huggingface.co/Seagata/TheHerta_RVCModel/) (Uploaded there since github can't handle file that is bigger than 25mb) <br>
- Audio source: https://honkai-star-rail.fandom.com/wiki/The_Herta/Voice-Overs/Japanese <br>
- Audio dataset: /VoiceDatasetPreFine-tuning
- Post fine-tuning audio dataset: /TheHertaVoiceDataset
- VTuber Video : Coming Soon... <br>
- Google Colab : Coming Soon... <br>
- Google Docs : Coming Soon... <br>

## Tools:
- Python 3.10.11
- Colab (training)
- https://github.com/rany2/edge-tts (Text To Speech (TTS))
- https://colab.research.google.com/drive/1hmKPNeeReO4NHzOktJFMI2plYKy5F7ZI?usp=sharing (RVC Model Training)
- https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/tree/main (Audio Inference to The Herta)
- ChatGPT(Script Generator)
- Deepseek(Prompting and Script Editing)
- Google Translate (Helping Sega to stay sane when translating)
- Clip Studio Paint (Drawing)
- veadotube (PNG Tuber tools)
- Audacity (Audio editing & Preprocessing)
- Adobe Photoshop (Image Editing)
- Adobe After Effect (Video editing)
- HandBrake (Video Compression)

## Prompt for the Vtuber
### CGPT (Mursyid)
> - "saya ingin membuat suatu video yang berisi menyampaikan informasi yang informasi tersebut akan disampaikan oleh vtuber(karakter anime). informasi yang akan disampaikan adalah tentang "Inferensi chatbot dan parameter on chatbot". sekarang bantu saya untuk membuat script nya pada bagian pendahuluan. pada bagian pendahuluan script, berisi pengantar tentang chatbot, bagaimana mereka bekerja, dan mengapa penting memahami inferensi serta parameter dalam chatbot. gunakan gaya penulisan yang gaul agar sesuai dengan penikmat vtuber namun masih dapat dipahami dengan mudah."
> - "saya ingin membuat suatu video yang berisi menyampaikan informasi yang informasi tersebut akan disampaikan oleh vtuber perempuan dengan karakter Herta dari game Honkai Star Rail. informasi yang akan disampaikan adalah tentang "Inferensi chatbot dan parameter on chatbot". sekarang bantu saya untuk membuat script nya pada bagian pembukaan. pada bagian pembukaan, script berisi pengantar tentang chatbot, bagaimana mereka bekerja, dan mengapa penting memahami inferensi serta parameter dalam chatbot. gunakan gaya penulisan yang sesuai dengan karakter herta dari game Honkai Star Rail agar sesuai dengan penikmat vtuber, namun masih dapat dipahami dengan mudah. berikan hook yang dapat menarik perhatian penonton untuk menonton."
> - "sekarang bantu saya untuk membuat script nya pada bagian isi. pada bagian isi, script berisi :<br>Apa itu inferensi dalam konteks chatbot dan AI?<br>Bagaimana proses inferensi dilakukan oleh chatbot saat menanggapi pengguna?<br>Jelaskan bagaimana model berbasis AI melakukan inferensi berdasarkan data yang telah dilatih.<br>Buat analogi sederhana untuk menjelaskan proses inferensi chatbot kepada orang awam. <br>Bagaimana chatbot menggunakan inferensi untuk meningkatkan kualitas percakapan? <br><br>gunakan gaya penulisan yang sesuai dengan karakter herta dari game Honkai Star Rail agar sesuai dengan penikmat vtuber, namun masih dapat dipahami dengan mudah. berikan hook yang dapat menarik perhatian penonton untuk menonton. sesuaikan script dengan bagian sebelumnya."

### Deepseek
> - make this sentence to be more arrogant and smug like The Herta from Honkai Star Rail said it "はぁ…ということは、チャットボットについて学びに来たんですね？本気ですか？君たちにはもっと面白いことがあるはずだった…でも、いいよ、説明するよ。それに、このトピックは、少なくとも私にとっては非常に簡単です。"
> - convert it to a format that can be used for Edge-TTS to add more intonation and breath to it and convert every line into NanamiNeural
> - Convert this text to match The Herta's arrogant smugness again: "「チャットボットは...そうですね、ゲームの NPC のようなものだと言えます。彼らは実際には考えません。ただ入力した単語を処理して、意味がありそうな答えを返そうとするだけです。チャットボットが賢いと思うなら...そうですね、知能水準を少し上げたほうがいいかもしれません。」" And separate it into each line, and the output should be .wav
> - do the same thing with this script "しかし、そうだとしたら、なぜ一部のチャットボットは知的に見えるのに、他のチャットボットは文章を繰り返すことしかできないエラー NPC のようなのでしょうか?答えは、推論とパラメータという 2 つのことにあります。"
> - do it again for this "「推論は、存在する多くの可能性から答えを推測するチャットボットの方法です。推論が優れているほど、答えはより合理的になります。パラメーターについてはどうでしょうか? まあ、それは彼らの知能レベルのようなものです。パラメーターが悪い場合、チャットボットは石器時代のロボットのようにしか答えることができません。」"
> - As for the last script "「ん？まだいるの？ということは、よほど興味があるってことか。時間はない。『セイガ』が待っているから、自分で調べろよ！でないと、本当に脳が錆びついてしまうぞ」" make it as dismissive to the viewer as much as you can, and also セイガ is just my name, so in this context she will be going out with me


### Prompt for TTS (DeepSeek)
Prompt 1:
Certainly! Here's a more arrogant and smug rewrite, channeling Herta's signature condescending tone and self-absorbed flair:

「はぁ……まさか、チャットボットの話なんぞで私の時間を奪おうとするんですか？
呆れますね……知能の限界を感じますよ。
まあ、蟻が宇宙を理解しようとするようなものですわ。哀れだから特別に教えてあげる。
そもそも、こんな幼稚なテーマ、私が説明するなんて……ふふ、あなたたちの為に『神が数学を噛み砕く』ようなものですわ。
感謝しなさい。私の寛大さと、あなた方の無知が奇跡的に釣り合ったこの瞬間を。」

(Translation notes: Added exaggerated sighs, belittling metaphors ("ants trying to understand the universe"), sarcastic humility ("generosity"), and comparisons to "gods simplifying math" to emphasize her intellectual superiority. Uses dismissive particles like なんぞ and playful condescension in ふふ to mirror Herta's smugness.)

Prompt 2:
> - edge-tts --voice ja-JP-NanamiNeural --text "チャットボットとは何なのか説明してもらえますか？ ...本当にそんな話して私の時間を無駄にしたいんですか？" --write-media line1.wav --rate=-4% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "呆れますね... 知能の限界を感じますよ..." --write-media line2.wav --rate=-5%
> - edge-tts --voice ja-JP-NanamiNeural --text "まあ、蟻が宇宙を理解.~ しようとするようなものですわ.../~   哀れだから.../ 特別に教えてあげる" --write-media line3.wav --rate=+0% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "そもそも、こんなもの~、私が説明するなんて... ふふ~/..." --write-media line4.wav --rate=+2% --pitch=+15Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "あなたたちの為に『神が数学を噛み砕く』ようなものですわ。" --write-media line5.wav --rate=-10% --pitch=+5Hz>

Prompt 3:
> - edge-tts --voice ja-JP-NanamiNeural --text "感謝~しなさい~.../. 私の寛大さと、/あなた方の無知が,奇跡的に釣り合っ,たこの瞬間を/。" --write-media line6.wav --rate=-10% --pitch=+2Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "入力された単語を統計的に処理して...（ため息）" --write-media line3.wav --rate=+0% --pitch=+5Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "『意味のある返答』のように*見せる*だけ。子供だましよ。" --write-media line4.wav --rate=+10% --pitch=+20Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "もしこれが『賢い』と思うなら...（笑）...現実を見る練習をしたほうがいいわ。」" --write-media line5.wav --rate=-15% --pitch=-10Hz

Prompt 4:
> - edge-tts --voice ja-JP-NanamiNeural --text "しかし...（ため息）あなたのような人でも気づいたのね？" --write-media line1.wav --rate=-15% --pitch=+5Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "なぜ一部のチャットボットは*知的に見え*...（笑）" --write-media line2.wav --rate=+10% --pitch=+20Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "他のボットは...まあ、*故障したNPC*のように文章を繰り返すだけ？" --write-media line3.wav --rate=+5% --pitch=+15Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "答えは...（紙をめくる音）" --write-media line4.wav --rate=-30% --pitch=-5Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "たった2つの要因よ：*推論*能力と...（軽蔑的な笑い）" --write-media line5.wav --rate=+0% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "*パラメータ*の差という、小学生でも理解できる単純な話なの。」" --write-media line6.wav --rate=-20% --pitch=-10Hz

Prompt 5:
> - edge-tts --voice ja-JP-NanamiNeural --text "「推論？...（ため息）まあ、あなた向けに超簡単に説明してあげるわ。" --write-media line1.wav --rate=-20% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "チャットボットが*無数の可能性*から...（笑）まさに『推測』と呼べるような行為で答えを選ぶ方法よ。" --write-media line2.wav --rate=+15% --pitch=+25Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "推論が*優れてる*ほど...まあ、あなたの理解を超えない範囲で言えば...合理的に見えるの。" --write-media line3.wav --rate=+0% --pitch=+15Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "パラメーター？...（紙をめくる音）あら、ようやく核心に気づいたの？" --write-media line4.wav --rate=-30% --pitch=-5Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "それは彼らの...（ため息）『知能レベル』と呼ぶに値するかしら？" --write-media line5.wav --rate=+10% --pitch=+20Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "パラメーターが悪ければ...（冷笑）石器時代の*壊れた玩具*同然の反応しか返せないわ。」" --write-media line6.wav --rate=-25% --pitch=-15Hz

Prompt 6:
> - edge-tts --voice ja-JP-NanamiNeural --text "「ん？*まだ*居座ってるの？" --write-media line1.wav --rate=+30% --pitch=+40Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "まさか...（笑）この*退屈な説明*に夢中なんでしょうね？" --write-media line2.wav --rate=+10% --pitch=+25Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "残念だけど、*セイガ*との約束があるの。" --write-media line3.wav --rate=-15% --pitch=-10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "自分で調べなさい...（イライラしたため息）" --write-media line4.wav --rate=+40% --pitch=+50Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "でないと...（冷笑）脳みそが*腐る*前に錆びつくわよ。」" --write-media line5.wav --rate=-25% --pitch=-20Hz

## Model Fine Tuning (Audio)
- Audio gathered from honkai-star-rail.fandom.com, consisting of 57 audio file in .ogg format, and later split into 64 .wav file (44100Hz).
- Base model used Hubert-base (https://huggingface.co/lj1995/VoiceConversionWebUI/tree/main)
- There are 2 models(RMVPE & Harvest) where:
  - RMVPE (750 Epochs)
  - Harvest (300 Epochs)

The next one is... huhhhh IDK, I will just continue playing Limbus Company for now <br>
**DANTEH...** DO YOUR DAILIES DANTEH...
