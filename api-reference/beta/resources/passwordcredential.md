---
title: passwordCredential リソースの種類
description: アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。 ServicePrincipal エンティティおよびアプリケーション エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。
ms.openlocfilehash: 79d3f76606533cf639f52ed22cd93f353e18e977
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066561"
---
# <a name="passwordcredential-resource-type"></a>passwordCredential リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。 [ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。


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
|customKeyIdentifier|バイナリ|            |
|endDateTime|DateTimeOffset|日付と時刻、パスワードの有効期限が切れます。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|キー Id|Guid|            |
|startDateTime|DateTimeOffset|日付と時刻にパスワードが有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|secretText|String| パスワードは 16 ~ 64 文字の長さである必要があります。 |
|ヒント|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
