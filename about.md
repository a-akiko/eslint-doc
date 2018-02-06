# About

ESLint is an open source JavaScript linting utility originally created by Nicholas C. Zakas in June 2013. Code linting is a type of static analysis that is frequently used to find problematic patterns or code that doesn’t adhere to certain style guidelines. There are code linters for most programming languages, and compilers sometimes incorporate linting into the compilation process.

ESLintは、もともとNicholas C. Zakasが2013年6月に作成したオープンソースのJavaScript lintingユーティリティです。コードの埋め込みは、特定のスタイルガイドラインに準拠していない問題のあるパターンやコードを見つけるために頻繁に使用される静的解析の一種です。 ほとんどのプログラミング言語にはコード・リンターがあり、コンパイラーは時にはリンキングをコンパイル・プロセスに組み込むことがあります。

---

JavaScript, being a dynamic and loosely-typed language, is especially prone to developer error. Without the benefit of a compilation process, JavaScript code is typically executed in order to find syntax or other errors. Linting tools like ESLint allow developers to discover problems with their JavaScript code without executing it.

JavaScriptは、動的で緩やかに型付けされた言語であり、特に開発者のエラーになりがちです。 コンパイルプロセスの利点がなければ、通常、シンタックスやその他のエラーを見つけるためにJavaScriptコードが実行されます。 ESLintのような糸付けツールは、開発者がJavaScriptコードを実行することなく問題を発見できるようにします。

---

The primary reason ESLint was created was to allow developers to create their own linting rules. ESLint is designed to have all rules completely pluggable. The default rules are written just like any plugin rules would be. They can all follow the same pattern, both for the rules themselves as well as tests. While ESLint will ship with some built-in rules to make it useful from the start, you’ll be able to dynamically load rules at any point in time.

ESLintが作成された主な理由は、開発者が独自のリンティングルールを作成できるようにすることでした。 ESLintはすべてのルールを完全にプラガブルにするように設計されています。 デフォルトルールは、プラグインルールと同様に記述されます。 彼らはすべて、ルール自体とテストの両方について、同じパターンに従うことができます。 ESLintには最初から便利なように組込みルールがいくつか付属していますが、いつでもルールを動的にロードすることができます。

---

ESLint is written using Node.js to provide a fast runtime environment and easy installation via npm.

ESLintはNode.jsを使用して書かれているため、実行時の環境が速く、npmで簡単にインストールできます。


### Philosophy

Everything is pluggable:

- Rule API is used both by bundled and custom rules
- Formatter API is used both by bundled and custom formatters
- Additional rules and formatters can be specified at runtime
- Rules and formatters don’t have to be bundled to be used

---

- ルールAPIはバンドルされたルールとカスタムルールの両方で使用されます
- Formatter APIは、バンドルされたフォーマッタとカスタムフォーマッタの両方で使用されます。
- 実行時に追加のルールとフォーマッタを指定できます
- ルールとフォーマッタをバンドルして使用する必要はありません

#### Every rule:

- Is standalone
- Can be turned off or on (nothing can be deemed “too important to turn off”)
- Can be set to a warning or error individually

---

- スタンドアロン
- オフまたはオンにすることができます（「オフにすることは非常に重要」とはみなされません）
- 個別に警告またはエラーに設定できます

#### Additionally:

- Rules are “agenda free” - ESLint does not promote any particular coding style
- Any bundled rules are generalizable

---

- ルールは「アジェンダフリー」です - ESLintは特定のコーディングスタイルを宣伝しません 
- バンドルされたルールはすべて一般化可能です

#### The project:

- Values documentation and clear communication
- Is as transparent as possible
- Believes in the importance of testing

---

- 価値の文書化と明確なコミュニケーション
- できるだけ透明です
- テストの重要性を信じる
