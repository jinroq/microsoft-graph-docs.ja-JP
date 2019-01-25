---
title: リソースの種類を説明します。
description: 相手の電子メール アドレスに基づいてユーザーに通知を表します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523198"
---
# <a name="mention-resource-type"></a>リソースの種類を説明します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

相手の電子メール アドレスに基づいてユーザーに通知を表します。 この通知の種類は、参照 @ とも呼ばれます。

[メッセージ](../resources/message.md)リソースは、**説明**をサポートします。 サインイン中のユーザーがそのメッセージ インスタンスに記載されているかどうかを示す**mentionsPreview**プロパティが含まれています。 **紹介**のナビゲーション プロパティを取得の詳細を記載されている、またはそのインスタンスの参照を削除するをサポートしているも含まれています。

メッセージを作成すると、アプリは、**Mentions** プロパティにメンションを含むことで、同じ `POST` 要求にメンションを作成できます。`$filter` クエリ パラメーターを含む `GET` 要求を使用して、アプリは、サインインしているユーザーのメールボックス内にある、ユーザーをメンションするすべてのメッセージを返すことができます。`$expand` クエリ パラメーターを含む `GET` 要求によって、アプリは特定のメッセージのすべてのメンションを展開できるようになります。

アプリがメッセージ内のメンションを設定して取得できるようにするこのメカニズムによって、簡易的な通知が可能になり、アプリが基になる **Mentions** プロパティを設定すると同時に、メンションを行うユーザーは既存のコンテキスト内に留まることができます (メッセージ本文の作成など)。メンションされたユーザーは、`$filter` または `$expand` クエリ パラメーターを含む `GET` 要求を介して、ユーザーがメンションされたかどうかとメンションされた場所を簡単に検索することができます。  

Outlook メール クライアントが表示され、ユーザーが入力するときに、 `@` 、メッセージの作成中に Outlook により、ユーザーを選択するか、または @ 言及を完了するための名前を入力します。 作成し、メッセージまたはイベントを送信する前に、outlook は、"**説明**"プロパティを設定します。 Outlook を使用しても`GET`での操作`$filter`と`$expand`、サインイン中のユーザー、ユーザーのことを説明するメッセージを検索できるように、迅速な対応を可能にするアクション アイテムや、ディスカッションをユーザーに警告します。


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
|application | String | メンションが作成されるアプリケーションの名前。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。 |
|ClientReference | String | リソース インスタンスの親を表す一意の識別子。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。 |
|createdBy  | [emailAddress](../resources/emailaddress.md) | 参照投稿を行ったユーザーの電子メール情報。 |
|createdDateTime  |DateTimeOffset |クライアントでメンションが作成された日時。 |
|DeepLink | String | リソース インスタンス内のメンションのコンテキストへの深い Web リンク。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。 |
|id | String| リソース インスタンス内のメンションの一意の識別子。|
|Mentioned | [emailAddress](../resources/emailaddress.md) | メンションした人の電子メール情報。必須です。 |
|MentionText | String | 省略可能。 使用され、**メッセージ**の場合は null ではありません。 メッセージで、参照を取得するには、代わりに、メッセージの**bodyPreview**プロパティには、参照してください。 |
|ServerCreatedDateTime | DateTimeOffset | サーバーでメンションが作成された日時。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[投稿](../api/user-sendmail.md#request-2)および送信 | なし | 新しいメッセージの一部としてメンションを作成および送信する|
|新しい下書きを[投稿](../api/user-post-messages.md#request-2) | **説明**する 1 つまたは複数オブジェクトを含む[メッセージ](../resources/message.md)です。 | 新しいメッセージの下書きを作成し、**ことを説明**する 1 つまたは複数オブジェクトが含まれます。|
|[Get](../api/user-list-messages.md#request-2)メッセージを私に言及しています。 | [message](../resources/message.md) コレクション | **説明**のこのユーザーを含む、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。|
|メッセージの[取得](../api/message-get.md#request-2)とその評価 | [message](../resources/message.md) コレクション | メッセージを取得し、各**説明**メッセージの詳細を展開します。|
|メンションの削除 | なし |サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。 |

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
