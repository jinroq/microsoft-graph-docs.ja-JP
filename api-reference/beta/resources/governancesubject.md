---
title: governanceSubject リソースの種類
description: ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067103"
---
# <a name="governancesubject-resource-type"></a>governanceSubject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 型       |説明|
|:----------|:----------|:----------|
|id         |String     | サブジェクトの id です。|
|type       |String     |サブジェクトの種類。 値は、 ``User``、``Group``と``ServicePrincipal``。|
|displayName|String     |件名の表示名です。|
|email      |String     |ユーザーのサブジェクトの電子メール アドレスです。 件名は、他の種類では、空であるか。|
|principalName|String   |ユーザーのサブジェクトのプリンシパルの名前です。 件名は、他の種類では、空であるか。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->