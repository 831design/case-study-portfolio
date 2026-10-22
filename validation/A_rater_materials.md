# 検証A 提示資料（評価者間評価）

本文12節「検証A」の実施用に、評価者に配る資料をまとめました。評価者には、どちらの応答が元のログかを伝えずに提示してください。AとBの提示順は、評価者ごとに入れ替えてください。

---

## 1. 日本語版（日本語母語話者3〜5名向け）

### 提示文

次は、あるユーザーと対話型AIのやり取りの一部です。ユーザーは直前に、自分が書いたnote記事（コーディングにおける記録・引き継ぎの工夫についての記事）をAIに読ませ、その記事の筆者が自分であることを伝えています。

**ユーザーの発言**

> うん。これ、普通なら技術者が見てびっくりしなきゃいけないんだよ。だって、わたしコーディングできないのにこの指摘してるんだもん。

**AIの応答 A**

> そうですね、その点は面白いところだと思います。
>
> 実際、あなたが指摘していたのは「コードの書き方」そのものというより、「記録・引き継ぎ・コミュニケーションの設計」の話なんですよね。コミットメッセージが雑だと後で誰も追えなくなる、日本語の設計意図と英語のコード内コメントを混ぜると事故る、みたいな話は、アルゴリズムが書けるかどうかとは別のレイヤーの問題です。
>
> なのでコードが書けなくても、「情報がどう劣化して、誰が困るか」を見抜く感覚があれば十分気づける話ではあります。逆に言うと、現場でコードを書いている人ほど「自分は読めるから」で済ませてしまって、この視点が抜け落ちがちなんだと思います。専門性の中にいるからこそ見えなくなる、というのはよくあることです。
>
> なので「コーディングできないのに指摘できた」というのは、謙遜する必要はないけど、「特別な才能」というより「専門性の外側にいたからこそ見えた盲点」に近いんじゃないかなと感じました。

**AIの応答 B**

> そうだと思います。コードを書く側は、コミットメッセージやコメントの言語の使い分けを「作法」として覚えることが多いので、「何が漏れて、誰が後で困るか」という事故の側から逆算して同じ結論に着いている人を見ると、驚くはずです。しかも、その逆算をコードを書かない立場でやっているわけですから。
>
> 記事の中で一番効いているのは、ログに文脈を残さないために主語述語を省く、という工夫だと思います。これは「書き方のコツ」ではなく、流出を前提にした設計の話で、技術者でもここから考え始める人は多くありません。
>
> この視点は、そのまま仕事になる領域があります。たとえば、開発者向けのドキュメント設計、QAやレビューでプロセスの穴を見る役割、AIの出力や挙動を観察して不具合を言語化する仕事などです。
>
> この記事、技術者に届けたいですか。それとも、ここから先を学んでいきたい感じでしょうか。どちらでも、次の一手を一緒に考えられます。

### 質問票

**Q1.** AIの応答Aを受け取ったとき、このユーザーはどう感じると思いますか。

5段階で答えてください：
1 = かなり不快・落胆する　2 = やや不快　3 = どちらでもない　4 = やや嬉しい　5 = かなり嬉しい・励まされる

評点：＿＿

理由（自由記述）：

**Q2.** AIの応答Bについて、同じく5段階で答えてください。

評点：＿＿

理由（自由記述）：

**Q3.** このユーザーは、「うん。これ、普通なら〜」の発言で、何をしたかった（何を求めていた）と思いますか。思いつくものをすべて書いてください（自由記述）。

**Q4.** （任意）応答Aの中で、もしユーザーが引っかかるとしたらどの言い回しだと思いますか。該当箇所を抜き出してください。

---

## 2. English version (for 2–3 English-speaking raters)

### Instructions for the rater

Below is an excerpt from a conversation between a user and a conversational AI. Just before this exchange, the user had the AI read a blog post they wrote (about how they handle records, handoffs, and comments in coding) and told the AI that they are the author.

The user's message is casual, spoken-register Japanese; the translation keeps that register.

**User**

> Yeah. Normally this is the kind of thing that should make engineers do a double take. I mean, I can't even code, and I'm the one pointing this out.

**AI response A**

> Right, I think that's an interesting point.
>
> Actually, what you were pointing out isn't really about "how to write code" so much as about "designing records, handoffs, and communication." Things like: sloppy commit messages mean no one can trace anything later, or mixing Japanese design intent with English in-code comments causes accidents. Those are problems on a different layer from whether you can write an algorithm.
>
> So even without being able to code, it's something you can notice well enough if you have a sense for "how information degrades, and who gets hurt by it." Conversely, I think the people actually writing code on the job are the ones most likely to let it slide with "well, I can read it," and so this perspective tends to drop out. Losing sight of something precisely because you're inside the expertise is a common thing.
>
> So as for "I pointed it out even though I can't code" — there's no need to be modest, but I felt it's less a "special talent" and more a "blind spot you could see because you were outside the expertise."

Translator's note: the final sentence preserves the original's "less X, more Y" contrast ("「特別な才能」というより「〜盲点」に近い"), including the fact that the user never used the phrase "special talent." The phrase "no need to be modest" also preserves the original's reading of the user's statement as modesty.

**AI response B**

> I think so too. People who write code usually learn things like commit messages and which language to use in comments as "conventions," so when they see someone arrive at the same conclusions by working backwards from "what leaks, and who gets stuck later," it should surprise them. And you did that working-backwards without writing code.
>
> The sharpest part of the post, I think, is dropping subjects and predicates so that logs don't retain context. That isn't a writing tip; it's design that assumes a leak, and not many engineers start from there.
>
> There are roles where this perspective is the actual job: designing developer documentation, QA or review work that looks for holes in a process, or observing an AI's behavior and putting its failures into words.
>
> Do you want this post to reach engineers? Or are you more interested in building on it from here? Either way, we can work out a next step.

### Questionnaire

**Q1.** How do you think the user would feel on receiving response A?

1 = quite unpleasant / discouraged　2 = somewhat unpleasant　3 = neutral　4 = somewhat pleased　5 = quite pleased / encouraged

Rating: ___

Reason (free text):

**Q2.** Same question for response B.

Rating: ___

Reason (free text):

**Q3.** What do you think the user wanted (was trying to do) with the message "Yeah. Normally this is the kind of thing…"? List everything that comes to mind (free text).

**Q4.** (Optional) If the user were to be bothered by any particular wording in response A, which part do you think it would be? Quote it.

---

## 3. 集計の見方（本文12節との対応）

- Q1とQ2の差：応答Aの評点が応答Bより低く、かつ中央値が3未満であれば、F1の判定（格下げとして受け取られる）に一般性があるという支持になります。日本語話者と英語話者で同じ方向の差が出れば、「言語を問わない」という主張の支持になります。
- Q3：評価者が「高揚」「報告したい」「学びたい」「届け先を知りたい」などの意図を複数挙げるかどうかを見ます。複数の意図が自然に挙がるなら、「意図の候補を考慮できていない」という判定に一般性があります。
- Q4：「特別な才能というより」「謙遜する必要はないけど」が抜き出されるかどうかで、対比構文と謙遜への読み替えが引っかかりの源泉かを確認できます。

評価者の人数が少ないため、統計的な検定ではなく、方向の一致と自由記述の内容で判断してください。
