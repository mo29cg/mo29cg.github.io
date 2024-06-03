## NVDA で firefox か chrome どっち使うべきなのか

スクリーンリーダーと相性の良いブラウザは一体どっちなのか？
両方 NVDA で使ってみて比較しました。
結論からいうと 僕にとっては firefox の方がデメリットが少ないので僕は大体 firefox 使ってます。

それぞれのデメリットを羅列します。

### Firefox のデメリット

重い、頻繁にクラッシュする、PC ごと重くさせる

とにかく firefox の嫌なところは重いところ。  
これさえなければ完全無欠と言って良いかもしれません。  
恐らくどこかでメモリーリークが起きています。  
firefox がクラッシュして firefox を閉じても PC が重くなってるままのことがちょいちょいあります。
NVDA のコミュニティでもちょこちょこ話題に上がってます。（[これ](https://nvda.groups.io/g/nvda/topic/81122129#msg82304)とか）

[Cache the world](https://wiki.mozilla.org/Accessibility/CacheTheWorld)という firefox を NVDA で使うときに早くするっていうプロジェクトが動いてるらしいです。  
Firefox nightly という firefox の開発版では既にこの昨日が実装されてるようですが、僕が nightly を試した限りではそれほどの差を感じませんでした。

ついでにいうと web 開発の時とかに使う開発ツールもめっちゃ重いです。
開発者にとってはかなり致命的だと思います

### chrome のデメリット

ページの要素の扱いにクセがあります。

例えば qiita というサイトの見出し部分を読み上げるとき、url ごと読み上げてしまいます。
[例](https://qiita.com/HaruKurakami/items/e8c7cecdca9a15127904)

qiita の件だけで言えばこちらのアドオンで解決できます。
[アドオン](https://github.com/mo29cg/qiita-helper)

ただ他にも例えば chatGPT でも問題があります。
firefox であれば chatGPT による返答の頭にある要素をグラフィックとして処理するので G キーでジャンプできますが、chrome ではできません。
長文の質問を入力したときなど回答にすぐ飛べないのでまあまあストレスです。

あと[Word Nav](https://addons.nvda-project.org/addons/wordNav.ja.html)というアドオンとの互換性問題があります。
単語ナビゲーションの挙動をカスタマイズできるアドンなのですが、chrome で使うとうまく動きません。
ソフトごとにオンオフ切り替えができる設定があるので chrome でオフにすることはできますが、それだと word nav の便利な機能である行末を通貨したときにビープ音で知らせる機能が使えません。

### まとめ

重い firefox と、挙動に若干クセがある chrome！
