# <a name="use-the-activity-feed-rest-api"></a>アクティビティ フィード REST API を使用する

Microsoft Graph のアクティビティ フィード API を使用して、デバイスやプラットフォームをまたいでユーザーのアクティビティを再開できます。 アクティビティ フィード API 要求は、[委任されたアクセス許可](../../../concepts/permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions)と[ユーザー アクティビティのアクセス許可](../../../concepts/permissions_reference.md)、個人または仕事や学校のアカウントを使用できるユーザーの代わりに実行されます。 

ユーザー アクティビティは、[アクティビティ](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity)リソースにより示され、collection me/activities により示される時間ベースのフィードとして整理されます。 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>優れたユーザー アクティビティとは

ユーザー アクティビティは、アプリを起動するだけではなく、アプリ内の特定のコンテンツに密接にリンクしています。 作成したユーザー アクティビティを自分のアプリで使用することができるだけでなく、Cortana と Windows のタイムラインにも表示されることにより、アプリの再接続が増え、ユーザーが複数のデバイスでアプリを使用することが容易になります。  

### <a name="what-should-become-an-activity"></a>何がアクティビティになりますか 

すべてのアプリケーションは異なるため、各アプリケーション開発者は、アプリケーション内の操作をユーザー アクティビティにマップする最適な方法を理解する必要があります。 たとえば、ゲームでは、キャンペーンごとのアクティビティ、ドキュメント作成アプリではドキュメント固有のアクティビティ、基幹業務アプリケーションではワークフローごとのアクティビティがそれぞれ作成される可能性があります。 

アプリでアクティビティを定義する場合は、次のガイドラインを適用します。

**行うこと:** 関連するユーザー操作のグループに対して 1 つのアクティビティを記録します。 一連の関連コンテンツにアプリケーションを使用している場合は、エンゲージメント セション全体で  1 つのアクティビティを記録することが適切です。  

*プレイリストのシナリオ:* これは特に音楽プレイリストやテレビ番組に関係するものであり、単一のユーザー アクティビティを更新して進行状況を示すことができます。 この例では、複数の日や数週間にわたるエンゲージメント期間を示す複数の[履歴項目](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_historyitem)を含む単一のユーザー アクティビティがあります。  

**行うこと:** ユーザー データをクラウドに保存します。 デバイス間のアクティビティをサポートする場合は、アクティビティの再エンゲージに必要なコンテンツがクラウドに保存されていることを確認する必要があります。 たとえば、ユーザーがドキュメントを編集するたびにアクティビティを公開する場合、デバイス間での再エンゲージメントを可能にするためには、ドキュメントはユーザーのデバイス上にローカルに保存するのではなく、クラウドに保存する必要があります。  

**行わないこと:** ユーザーが将来再開する必要のない操作のユーザー アクティビティを作成する。 アプリケーションを、将来的に追跡する状態を保持しない、単純に 1 回限りの操作を完了するために使用している場合は、ユーザー アクティビティを書く必要はおそらくありません。 

ユーザー アクティビティが Windows のタイムラインに表示されるとしても、これはバージョン管理ツールとして設計されたものではありません。ドキュメント ベースのアクティビティを選択すると、そのドキュメントの最新バージョン (他のユーザーによる変更を含む) が常に表示されます。

**行わないこと:** *他のユーザー*が完了したアクションのユーザー アクティビティを作成します。 ユーザーがメッセージを受信したり、アプリ内でユーザーが @mentions される場合は、新しいアクティビティを書くべきではありません。 このような場合は、通知を表示するとより効果があります。  

*コラボレーションのシナリオ:* 複数のユーザーが同じアクティビティ (Word ドキュメントなど) の作業をしている場合は、最後の編集の後に別のユーザーが変更を加えた可能性があります。 この場合、アプリの開発者はアクティビティのビジュアル要素を更新して、ドキュメントに対する変更を反映したい場合があります。 そのために、アプリは新しい履歴項目を作成することなく既存のアクティビティを更新することがあります。 

>**注:** Web アプリケーションのアクティビティを公開する場合、アクティビティごとに `activationURL` と `fallbackURL` を含めることが重要です。 このアクティビティにより、Windows タイムラインなどの Microsoft エクスペリエンスからアプリへとユーザーを戻すことができます。 

## <a name="app-interaction-patterns-and-user-activities"></a>アプリの相互作用パターンとユーザー アクティビティ 
作成するユーザー アクティビティは、アプリの相互作用パターンに応じて異なります。 すべてのアプリケーションは異なりますが、ほとんどの場合、次の相互作用パターンのいずれかに分類されます。 

* **ドキュメント ベースのアプリケーション**  — 使用期間を反映する 1 つ以上の履歴レコードを使用して、ドキュメントごとに 1 つのアクティビティを作成します。 ドキュメントの変更に応じて、アクティビティ カードを更新することが重要です。 
* **メディア再生アプリ**  — プレイリスト、プログラム、またはスタンドアロン コンテンツなど、コンテンツの論理グループごとに 1 つのアクティビティを作成します。 
* **ゲーム** — 保存したゲームや世界ごとに 1 つのアクティビティを作成します。 レベルのシーケンスを 1 つしかサポートしていないゲームの場合は、最新の進行状況や達成状況を表示するためにカードを更新することもできますが、時間の経過とともに同じアクティビティを記述できます。 
* **ユーティリティ アプリ** — アプリ内でユーザーが再開を望むことがない場合は、アクティビティを公開しないでください。 電卓のような単純な単目的アプリがその良い例です。 
* **基幹業務アプリ** — 単純なタスクやワークフローを管理する多くのアプリがあります。 アプリを通じてアクセスするワークフローごとに 1 つのアクティビティを作成します。 たとえば、アクティビティをクリックして承認済みか確認するためには、各経費明細書を異なるアクティビティにします。

*複雑なアプリには、複数の相互作用パターンが含まれています。アプリで扱うさまざまなシナリオに対して、さまざまなユーザー アクティビティの作成パターンに従うことができます。*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>次の手順

- 「[アクティビティ リソース](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity)」を参照し、ユーザーが重要なタスクを再開できるように、アプリのアクティビティを定義します。
- 「[アダプティブ カードのサンプル](http://adaptivecards.io/samples/)」を見て、アクティビティを**ポップ**にするアイデアを探します。  
- [Graph エクスプローラー](https://developer.microsoft.com/en-us/graph/graph-explorer)で API を試します。

**その他のアイデアが必要ですか ?** 
- 「[Microsoft エクスペリエンスはどのようにアクティビティを使用しているか](https://channel9.msdn.com/events/Build/2017/B8108)」を参照します。
- 「 [アクティビティ フィード API と中断した場所の選択](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)」を学習します。