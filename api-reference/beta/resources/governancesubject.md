---
title: governanceSubject リソースの種類
description: ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832593"
---
# <a name="governancesubject-resource-type"></a>governanceSubject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 種類       |説明|
|:----------|:----------|:----------|
|ID         |String     | サブジェクトの id です。|
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
