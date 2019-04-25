---
title: 言及リソースの種類
description: 個人の電子メールアドレスに基づいて、ユーザーへの通知を表します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523481"
---
# <a name="mention-resource-type"></a>言及リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

個人の電子メールアドレスに基づいて、ユーザーへの通知を表します。 この種類の通知は、@ メンションとも呼ばれます。

[メッセージ](../resources/message.md)リソースは、**メンション**をサポートしています。 このプロパティには、サインインしているユーザーがそのメッセージインスタンスで言及されているかどうかを示す**mentionsPreview**プロパティが含まれています。 また、メン**ション**ナビゲーションプロパティも含まれています。これは、メンションの詳細を取得するか、そのインスタンス内のメンションを削除することをサポートします。

アプリケーションでは、メッセージを作成するときに、メン**ション**プロパティ`POST`にメンションを含めることによって、同じ要求でメンションを作成できます。 クエリパラメーター `GET`を指定して要求を使用すると、アプリはサインインしているユーザーのメールボックス内のすべてのメッセージを返し、そのユーザーに言及できます。 `$filter` クエリパラメーターを使用して要求する`GET`と、特定のメッセージ内のすべてのメンションを展開できます。 `$expand`

メッセージでメンションを指定してメンションを取得するためのこのメカニズムにより、説明を作成しているユーザーが既存のコンテキスト (メッセージ本文の作成など) を既存のコンテキスト**** 内に残すことができます。. 指定された人物は、 `GET` `$filter`または`$expand`クエリパラメーターを使用して、要求によってどこにあるか、どこにあるかを簡単に確認できます。  

たとえば、outlook メールクライアントでは、ユーザーがメッセージの作成`@`中に入力すると、ユーザーは名前を選択または入力して、@ メンションを完了できます。 Outlook は、メッセージまたはイベントを作成して送信する前に、**メンション**プロパティを設定します。 Outlook で`GET` `$filter`は、および`$expand`を使用して、サインインしているユーザーに、ユーザーに通知するメッセージを検索させ、処理アイテムまたはディスカッションについての警告を表示して、応答を高速化することもできます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|application | String | メンションが作成されたアプリケーションの名前。 省略可能。 使用されず、**メッセージ**の既定値として null になります。 |
|clientreference | String | リソースインスタンスの親を表す一意の識別子。 省略可能。 使用されず、**メッセージ**の既定値として null になります。 |
|createdBy  | [emailAddress](../resources/emailaddress.md) | メンションを行ったユーザーの電子メール情報。 |
|createdDateTime  |DateTimeOffset |クライアントでメンションが作成された日時。 |
|リンク | String | リソースインスタンス内のメンションのコンテキストへのディープ web リンク。 省略可能。 使用されず、**メッセージ**の既定値として null になります。 |
|id | String| リソース インスタンス内のメンションの一意の識別子。|
|明記 | [emailAddress](../resources/emailaddress.md) | 記載されているユーザーの電子メール情報。 必須。 |
|mentionText | String | 省略可能。 使用されず、**メッセージ**の既定値として null になります。 メッセージ内のメンションを取得するには、代わりにメッセージの**bodyPreview**プロパティを参照してください。 |
|serverん datetime | DateTimeOffset | メンションがサーバー上に作成された日付と時刻。 省略可能。 使用されず、**メッセージ**の既定値として null になります。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[投稿](../api/user-sendmail.md#request-2)と送信 | なし | 新しいメッセージの一部としてメンションを作成して送信します。|
|新しい下書きに[投稿](../api/user-post-messages.md#request-2)する | 1つまたは複数の**メンション**オブジェクトを含む[メッセージ](../resources/message.md)。 | 新しいメッセージの下書きを作成し、1つまたは複数の**メンション**オブジェクトを含めます。|
|自分宛てのメッセージを[取得](../api/user-list-messages.md#request-2)する | [message](../resources/message.md) コレクション | このユーザーの**メンション**を含む、サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。|
|メッセージとそのメンションを[取得](../api/message-get.md#request-2)する | [message](../resources/message.md) コレクション | メッセージを取得して、メッセージ内の各**メンション**の詳細を展開します。|
|メンションを[削除](../api/message-delete.md#request-2)する | なし |サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
