# Generative AI Classs's First Project - The Herta Vtuber
Group 7 (Bojongsantos Oost-indische Compagnie)<br>
Cover Video : https://www.youtube.com/watch?v=4tJADqRNzek <br>
PNG Tuber : Coming Soon... <br>
RVC Model : [Seagata/TheHerta_RVCModel](https://huggingface.co/Seagata/TheHerta_RVCModel/) (Uploaded there since github cant handle files thats bigger than 25mb) <br>
Audio source: https://honkai-star-rail.fandom.com/wiki/The_Herta/Voice-Overs/Japanese <br>

## Tools:
- Python 3.10.11
- Colab (training)
- https://github.com/rany2/edge-tts (TTS)
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


### Prompt for TTS
Part1:
> - edge-tts --voice ja-JP-NanamiNeural --text "チャットボットとは何なのか説明してもらえますか？ ...本当にそんな話して私の時間を無駄にしたいんですか？" --write-media line1.wav --rate=-4% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "呆れますね... 知能の限界を感じますよ..." --write-media line2.wav --rate=-5%
> - edge-tts --voice ja-JP-NanamiNeural --text "まあ、蟻が宇宙を理解.~ しようとするようなものですわ.../~   哀れだから.../ 特別に教えてあげる" --write-media line3.wav --rate=+0% --pitch=+10Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "そもそも、こんなもの~、私が説明するなんて... ふふ~/..." --write-media line4.wav --rate=+2% --pitch=+15Hz
> - edge-tts --voice ja-JP-NanamiNeural --text "あなたたちの為に『神が数学を噛み砕く』ようなものですわ。" --write-media line5.wav --rate=-10% --pitch=+5Hz>

Part2:
> - edge-tts --voice ja-JP-NanamiNeural --text "感謝~しなさい~.../. 私の寛大さと、/あなた方の無知が,奇跡的に釣り合っ,たこの瞬間を/。" --write-media line6.wav --rate=-10% --pitch=+2Hz
> - 
