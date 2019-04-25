---
title: アクティビティフィード REST API を使用する
description: 'Microsoft Graph のアクティビティフィード API を使用して、デバイスとプラットフォーム間でユーザーのアクティビティを再開できます。 アクティビティフィード API 要求は、委任されたアクセス許可とユーザーアクティビティのアクセス許可を使用してユーザーの代理として実行されます。これは、個人用アカウントまたは職場アカウントまたは学校アカウントで使用できます。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: a522d4caa29aa5227f5030ed2663972e8b8d1660
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535809"
---
# <a name="use-the-activity-feed-rest-api"></a>アクティビティフィード REST API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Microsoft Graph のアクティビティフィード API を使用して、デバイスとプラットフォーム間でユーザーのアクティビティを再開できます。 アクティビティフィード API 要求は、委任された[アクセス許可](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)と[ユーザーアクティビティのアクセス許可](/graph/permissions-reference)を使用してユーザーの代理として実行されます。これは、個人用アカウントまたは職場アカウントまたは学校アカウントで使用できます。 

ユーザーアクティビティは、[アクティビティ](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_activity)リソースによって表され、コレクションの me/アクティビティで表される時間ベースのフィードに整理されます。 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>非常に高いユーザーアクティビティになるのは、どのようなものですか。

ユーザーアクティビティはアプリを起動するだけではなく、アプリ内の特定のコンテンツに対する深いリンクです。 作成したユーザーアクティビティは、独自のアプリで使用するだけではなく、Cortana と Windows タイムラインにも表示されます。これにより、アプリの再利用が向上し、ユーザーが複数のデバイスでアプリを引き続き使用することが容易になります。  

### <a name="what-should-become-an-activity"></a>アクティビティになる必要があるもの 

すべてのアプリが異なるため、アプリケーション内のアクションをユーザーアクティビティにマップするための最善の方法を、各アプリ開発者が理解している必要があります。 たとえば、ゲームは各キャンペーンに対してアクティビティを作成し、ドキュメント作成アプリは固有のドキュメントごとにアクティビティを作成し、基幹業務アプリは各ワークフローのアクティビティを作成する場合があります。 

アプリで activitites を定義するときに、次のガイドラインを適用します。

**実行:** 関連するユーザーアクションのグループに対して1つのアクティビティを記録します。 アプリケーションが関連するコンテンツのシーケンスに使用されている場合は、契約セッション全体に対して1つのアクティビティを記録することが適切な場合があります。  

*再生リストのシナリオ:* これは、音楽の再生リストまたはテレビ番組に特に関連しています。1つのユーザーアクティビティを更新して、進行状況を表示することができます。 この例では、複数の日数または数週間にわたる契約期間を表す複数の[履歴項目](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_historyitem)を持つ1つのユーザーアクティビティがあります。  

**実行:** ユーザーデータをクラウドに格納します。 クロスデバイスアクティビティをサポートする必要がある場合は、このアクティビティを再利用するために必要なコンテンツがクラウドの場所に格納されていることを確認する必要があります。 たとえば、ユーザーがドキュメントを編集するたびにアクティビティを発行する場合は、クロスデバイス再契約を有効にするために、ドキュメントをユーザーのデバイス上でローカルに保存するのではなく、クラウドに保存する必要があります。  

**次の操作は行わないでください。** ユーザーが今後再開する必要がない操作のユーザーアクティビティを作成します。 アプリケーションを使用して、状態を保持しない簡単なワンタイム操作を実行する場合、今後はユーザーアクティビティを記述する必要はありません。 

ユーザーアクティビティが Windows タイムラインに表示される場合でも、バージョン管理ツールとして設計されていませんが、ドキュメントベースのアクティビティを選択すると、そのドキュメントの最新バージョン (他のユーザーによる変更を含む) が常に表示されるようになります。

**次の操作は行わないでください。***他のユーザー*によって完了したアクションのユーザーアクティビティを作成します。 ユーザーがメッセージを送信したり、アプリ内でユーザーに @mentions したりした場合は、新しいアクティビティを作成しないでください。 これらの相互作用は、提示された通知により提供されます。  

*グループ作業のシナリオ:* 複数のユーザーが同じ操作 (Word 文書など) に対して作業を行っている場合、最後に編集した後に別のユーザーがドキュメントを変更した可能性があります。 この場合、アプリ開発者は、ドキュメントに加えられた変更を反映するために、アクティビティ内のビジュアル要素を更新する必要があります。 これを行うために、アプリは新しい履歴アイテムを作成せずに既存のアクティビティを更新する場合があります。 

>**注:** web アプリケーションのアクティビティを発行している場合は、アクティビティごと`activationURL` `fallbackURL`にとの両方を含めることが重要です。 アクティビティは、Windows タイムラインのような Microsoft エクスペリエンスから期待したとおりにユーザーをアプリに戻します。 

## <a name="app-interaction-patterns-and-user-activities"></a>アプリの相互作用パターンとユーザーアクティビティ 
作成するユーザーアクティビティは、アプリの対話パターンに応じて異なります。 すべてのアプリは異なりますが、ほとんどは次の相互作用パターンのいずれかに分類されます。 

* **ドキュメントベースのアプリ**-使用期間を反映した1つまたは複数の履歴レコードを含む1つのアクティビティをドキュメントごとに作成します。 ドキュメントが変更されたときに、アクティビティカードを更新することが重要です。 
* **メディア再生アプリ**—再生リスト、プログラム、スタンドアロンコンテンツなどのコンテンツの論理グループごとに1つのアクティビティを作成します。 
* **ゲーム**-セーブされたゲームまたは world ごとに1つのアクティビティを作成します。 ゲームでサポートされているレベルのシーケンスが1つだけの場合は、時間の経過とともに同じアクティビティを書き込むことができますが、最新の進捗状況やアチーブメントを表示するようにカードを更新する必要がある場合もあります。 
* **ユーティリティアプリ**: ユーザーが再開することをアプリ内に何もない場合は、アクティビティを発行しないでください。 良い例として、電卓などの単純な単一用途のアプリがあります。 
* **基幹業務アプリ**—単純なタスクやワークフローを管理するための多数のアプリがあります。 アプリを通じてアクセスする個別のワークフローごとに1つのアクティビティを作成します。 たとえば、各経費報告書は個別のアクティビティであるため、そのアクティビティをクリックして承認されたかどうかを確認したい場合があります。

*一部の複雑なアプリには、複数の相互作用パターンが含まれています。アプリによって処理されるさまざまなシナリオについて、さまざまなユーザーアクティビティ作成パターンに従うことをお勧めします。*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>次の手順

- ユーザーが重要なタスクを再開できるようにするには、[アクティビティリソース](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/projectrome_activity)を参照し、アプリのアクティビティを定義します。
- アクティビティを**ポップ**するためのアイデアについては、[アダプティブカードサンプル](https://adaptivecards.io/samples/)サンプルを参照してください。  
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。

**その他のアイデアをお探しですか?** 

- [Microsoft エクスペリエンスがアクティビティをどのように使用しているかを](https://channel9.msdn.com/events/Build/2017/B8108)確認します。
- [アクティビティフィード API](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011)について説明し、中断した場所を選択します。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/activity-feed-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
