---
title: keyCredential リソースの種類
description: アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。 アプリケーションと servicePrincipal のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。
ms.openlocfilehash: d4509360c0425c255566b9f77b9ecd96cf349dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066794"
---
# <a name="keycredential-resource-type"></a>keyCredential リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。 [アプリケーション](application.md)と[servicePrincipal](serviceprincipal.md)のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customKeyIdentifier|バイナリ| カスタム キー識別子 |
|endDateTime|DateTimeOffset|日付と、資格情報の有効期限が切れる。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|キー Id|Guid|キーの一意の識別子 (GUID)。|
|startDateTime|DateTimeOffset|日付と時刻に、資格情報が有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|type|String|キーの資格情報の種類「対称」などです。|
|使用法|String|キーが使われることができます; 目的を説明する文字列などの検証」です。|
|key|Binary|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->