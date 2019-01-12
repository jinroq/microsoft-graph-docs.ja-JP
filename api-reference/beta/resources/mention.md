---
title: リソースの種類を説明します。
description: 相手の電子メール アドレスに基づいてユーザーに通知を表します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: b24ce5488e93160c3424fb41f83b91c1b8ccea95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955437"
---
# <a name="mention-resource-type"></a>リソースの種類を説明します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

相手の電子メール アドレスに基づいてユーザーに通知を表します。 この通知の種類は、参照 @ とも呼ばれます。

[メッセージ](../resources/message.md)リソースは、**説明**をサポートします。 サインイン中のユーザーがそのメッセージ インスタンスに記載されているかどうかを示す**mentionsPreview**プロパティが含まれています。 **紹介**のナビゲーション プロパティを取得の詳細を記載されている、またはそのインスタンスの参照を削除するをサポートしているも含まれています。

メッセージを作成するには、アプリケーションを作成できます、記載されている同じ`POST`**に関する**プロパティで、説明を含めることによって要求されます。 使用して、`GET`の要求、`$filter`クエリ パラメーターでは、アプリ返すことができますすべてのメッセージで、サインインしているユーザーのメールボックスをユーザーに言及します。 A`GET`の要求、`$expand`クエリのパラメーターは、特定のメッセージ内のすべての記述を展開してアプリケーションをことができます。

アプリの中にアプリケーションを設定および参照投稿を行っているユーザーがメッセージの本文を作成する) などの既存のコンテキストで保持できる軽量の通知を有効に、メッセージで参照を取得することは、このメカニズムが基になる**紹介**プロパティを設定します。. 担当者が簡単に判りますし、によって記述されている`GET`が、要求、`$filter`または`$expand`パラメーターのクエリを実行します。  

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
|application | String | 参照投稿を作成するアプリケーションの名前。 省略可能。 使用され、**メッセージ**の場合は null ではありません。 |
|clientReference | String | リソース インスタンスの親を表す一意の識別子です。 省略可能。 使用され、**メッセージ**の場合は null ではありません。 |
|createdBy  | [emailAddress](../resources/emailaddress.md) | 参照投稿を行ったユーザーの電子メール情報。 |
|createdDateTime  |DateTimeOffset |クライアントでメンションが作成された日時。 |
|deepLink | String | リソース インスタンスに記載されているのコンテキストへの高度な web リンク。 省略可能。 使用され、**メッセージ**の場合は null ではありません。 |
|id | String| リソース インスタンス内のメンションの一意の識別子。|
|記載されています。 | [emailAddress](../resources/emailaddress.md) | メンションした人の電子メール情報。必須です。 |
|mentionText | String | 省略可能。 使用され、**メッセージ**の場合は null ではありません。 メッセージで、参照を取得するには、代わりに、メッセージの**bodyPreview**プロパティには、参照してください。 |
|serverCreatedDateTime | DateTimeOffset | 日付と時刻、記載されているサーバー上で作成されます。 省略可能。 使用され、**メッセージ**の場合は null ではありません。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[投稿](../api/user-sendmail.md#request-2)および送信 | なし | 作成し、新しいメッセージの一部として参照投稿を送信します。|
|新しい下書きを[投稿](../api/user-post-messages.md#request-2) | **説明**する 1 つまたは複数オブジェクトを含む[メッセージ](../resources/message.md)です。 | 新しいメッセージの下書きを作成し、**ことを説明**する 1 つまたは複数オブジェクトが含まれます。|
|[Get](../api/user-list-messages.md#request-2)メッセージを私に言及しています。 | [message](../resources/message.md) コレクション | **説明**のこのユーザーを含む、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。|
|メッセージの[取得](../api/message-get.md#request-2)とその評価 | [message](../resources/message.md) コレクション | メッセージを取得し、各**説明**メッセージの詳細を展開します。|
|参照[の削除](../api/message-delete.md#request-2) | なし |サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
