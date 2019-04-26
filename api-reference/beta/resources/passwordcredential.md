---
title: passwordcredential リソースの種類
description: アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。 serviceprincipal エンティティおよび application エンティティの**passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: f00deb42dcc24fc6d8218239d5d807ee21b2f7c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345015"
---
# <a name="passwordcredential-resource-type"></a>passwordcredential リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。 [serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customkeyidentifier|Binary|            |
|endDateTime|DateTimeOffset|パスワードの有効期限が切れる日付と時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|Guid|            |
|startDateTime|DateTimeOffset|パスワードが有効になる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|secretText|String| パスワードの長さは16-64 文字でなければなりません。 |
|hint|文字列型 (String)|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
