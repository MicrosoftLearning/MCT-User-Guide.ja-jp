#README

We've turned off the ability to report issues directly on this repo and do not monitor PRs.

Provide feedback here: https://aka.ms/provide-feedback

Or, if you are a trainer with a microsoft.com email address, please create a ticket in AzDO.

# MCT 向け GitHub ユーザー ガイド

Microsoft Azure などのクラウド サービスは頻繁に更新されるため、Microsoft 認定トレーナー (MCT) にとっては、クラウド サービスと一致しなくなったコースやラボの手順を教える際に困難が生じます 。 頻繁な変更と、変更されても通知されない場合があることが原因で、コース開発チームがラボの変更をすばやく特定し、調整するのは難しい場合があります。

このような問題に対処するために、私たちは GitHub を使って、Azure などのクラウド サービスを扱うコースのラボ手順とラボ スクリプトを公開しています。 GitHub を使うことで、コースの作成者と MCT はクラウド サービスの変更に合わせてラボの内容を最新の状態に保つことができます。 GitHub を使うことで、MCT はラボの変更に関するフィードバックや提案を提供することができ、コースの作成者はラボの手順やスクリプトをすばやく更新することができます。

これらのコースを教える準備をするときは、GitHub から適切なファイルをダウンロードして、最新のラボ手順とスクリプトを使用していることを確認する必要があります。

このユーザー ガイドは、GitHub を初めて使用する MCT 向けのものです。 GitHub への接続、コース教材のダウンロードと印刷、学生がラボで使用するスクリプトの更新を行う手順を示し、コースの内容を最新の状態に保つための方法について説明します。

> **注**:GitHub 上のファイルにアクセスするための Microsoft Learning サポートと GitHub サイトのナビゲーションのサポートは、このコースのみを教える MCT に限定されます。

コース内の技術的な内容や、コースやラボの準備方法について議論するために GitHub を使うべきではありません。 ラボの変更に対応するために使用してください。

 
> **注**:コースとデモに関する全般的なコメントや、コースの準備方法については、MCT フォーラムを使用してください。

## セクション

- [GitHub の用語](https://microsoftlearning.github.io/MCT-User-Guide/terminology/)

- [更新通知の受信とプロジェクトでの共同作業](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/)

- ラボの手順に対して変更を提案するか issue を送信する

## GitHub の用語

GitHub では、初めて目にする用語が登場することがあります。 このドキュメント全体で使用される用語と概念を、次の一覧に示します。 ただし、GitHub 用語の完全な一覧については、「[GitHub 用語集](https://docs.github.com/en/get-started/quickstart/github-glossary)」を参照してください。

| 期間| 説明 |
| - | - |
| Git と GitHub| Git はオープンソースの変更追跡プログラムです。GitHub は、Git に基づいて構築されたサイトまたはソリューションです。 バックエンドとして Git を使う Web サイトやソリューションは他にもあります。 GitHub は主にオープンソース (パブリック) 開発プロジェクトに使われ、そのようなプロジェクトには無料で使用できます。 ただし、オープンソースではなくプライベートなプロジェクトに GitHub を使う場合は、有料バージョンにサインアップする必要があります。 |
| リポジトリ| GitHub の各プロジェクトはリポジトリ内にあります。 リポジトリには、ドキュメントを含むプロジェクトのすべてのファイルが含まれており、リビジョン履歴をサポートしています。 リポジトリは、パブリックまたはプライベートにすることができます。 コンピューターのハード ドライブ上にリポジトリのローカル コピーを作成するか、GitHub 内でリポジトリを使うことができます。 |
| Markdown| ドキュメントの作成に使用できるテキストファイル形式です。 テキストベースで更新が非常に簡単なので、共同作業中に簡単に使用できます。 GitHub では HTML としてレンダリングされます。 |
| GitHub Flavored Markdown (GFM)| Markdown ファイル形式には多くのバリエーション (またはフレーバー) があります。 一般に GFM という GitHub バージョンは、Markdown の最も一般的なバリエーションの 1 つです。 GFM の詳細と、GFM ドキュメントにマークアップ形式を使う方法については、「GitHub での記述と書式設定の開始」(https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github/) を参照してください。 |
| フォーク| ブランチが元のリポジトリにあるのに対して、これは GitHub アカウントにある別のリポジトリのコピーです。 直下の「ブランチ」を参照してください。 |
| Branch| 元のリポジトリと同じリポジトリに存在するリポジトリのコピーです。 ブランチは元のブランチとマージできます。 |
| フェッチ| オンライン リポジトリから最新の変更のコピーを取得するプロセスのことです。 ただし、フェッチでは変更はマージされません。 |
| プル| オンライン リポジトリから最新の変更をフェッチし、ローカルの変更とマージするプロセスのことです。 |
| マージする| あるブランチから変更をフェッチし、別のブランチに適用するプロセスのことです。 オンライン リポジトリから変更を取得し、そのリポジトリのローカル バージョンに適用する場合も含まれます。 |
| Pull request| ユーザーがリポジトリに対して送信する一連の変更案です。リポジトリの所有者またはコラボレーターは pull request を承認または拒否できます。 |
| Push| ローカルの変更をオンライン リポジトリに送信するプロセスのことです。 |
| コラボレーター| リポジトリの内容を追加、削除、または変更するアクセス許可を持つ GitHub ユーザーです。 |

## 更新通知の受信、変更の提案、プロジェクトでの共同作業

GitHub リポジトリに対して更新が発生したときに通知を受け取るように GitHub エクスペリエンスを構成できます。 通知にサインアップする方法はいくつかあり、その多くはプロジェクトで共同作業を行うさまざまな方法に関連しています。 通知を受け取るには、次のアクションを実行できます。

| アクション| 説明 |
| - | - |
| [リポジトリを Watch する](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/watching/)| リポジトリを Watch すると、その特定のリポジトリに対して新しい pull request や issue が作成されるたびに通知を受け取るように、GitHub によって自動的にサブスクライブされます。 自分が作成したリポジトリや自分がコラボレーターであるリポジトリは、自動的に Watch 対象になります。 |
| [pull request](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/pullrequest/)| pull request を作成し、リポジトリの所有者に自分の変更の承認を提案すると、その pull request に関連するディスカッションの通知を受け取るように自動的にサブスクライブされます。 pull request を作成するには、まずブランチを作成する必要があります。 |
| [コメント](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/comment/)| 他のユーザーの pull request にコメントすると、そのコメントに関連するフォーラムに GitHub によって自動的にサブスクライブされます。手動でフォーラムにサブスクライブすることもできます。 |
| [問題](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/issue/)| issue とは、リポジトリに関連する提案、質問、または要求です。 各 issue には独自のディスカッションがあり、issue にはサブスクライブできます。自分が作成した issue には GitHub によって自動的にサブスクライブされます。 |
| [メンション](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/mention/)| 他のユーザーが自分の GitHub ユーザー名 ([@username](https://github.com/username)) を使って会話で自分をメンションすると、GitHub によって自動的にそのディスカッションにサブスクライブされます。 |

> **注**:通知を受け取る方法とタイミングは変更できます。また、ディスカッションのサブスクライブは解除できます。

## ラボの手順に対して issue を送信するか変更を提案する

ラボで提案がある場合やエラーが発生した場合は、pull request を送信するか、issue を報告できます。 エラーの解決策が既にわかっている場合は、pull request を送信することをお勧めします。それ以外の場合は、issue を送信します。

| アクション| 説明 |
| - | - |
| [pull request](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/pullrequest/)| pull request を作成し、リポジトリの所有者に自分の変更の承認を提案すると、その pull request に関連するディスカッションの通知を受け取るように自動的にサブスクライブされます。 pull request を作成するには、まずブランチを作成する必要があります。 |
| [コメント](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/comment/)| 他のユーザーの pull request にコメントすると、そのコメントに関連するフォーラムに GitHub によって自動的にサブスクライブされます。手動でフォーラムにサブスクライブすることもできます。 |
| [問題](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/issue/)| issue とは、リポジトリに関連する提案、質問、または要求です。 各 issue には独自のディスカッションがあります。 issue にはサブスクライブできます。自分が作成した issue には GitHub によって自動的にサブスクライブされます。 |
