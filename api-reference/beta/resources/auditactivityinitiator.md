---
title: auditActivityInitiator リソースの種類
description: 活動を開始するリソース オブジェクトの id。 ユーザー、アプリケーションまたはシステム (これはアプリケーションとしてと見なされます) をイニシエーターとして使用することができます。
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884610"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator リソースの種類
活動を開始するリソース オブジェクトの id。 ユーザー、アプリケーションまたはシステム (これはアプリケーションとしてと見なされます) をイニシエーターとして使用することができます。



## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|アプリ|[appIdentity](appidentity.md)|活動を開始するリソースがアプリケーションの場合は、このプロパティは、すべてのアプリケーションを示します appId などの情報を関連する名前、servicePrincipalId、名前です。|
|user|[割り当てられていません](useridentity.md)|活動を開始するリソースがユーザーの場合は、このプロパティは、すべてのユーザーを示しますに関連するユーザー Id、名前、UserPrinicpalName のような情報です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
