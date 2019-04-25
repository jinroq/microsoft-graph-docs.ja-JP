---
title: auditactivityinitiator リソースの種類
description: アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして考えられる) を指定できます。
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543769"
---
# <a name="auditactivityinitiator-resource-type"></a>auditactivityinitiator リソースの種類
アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして考えられる) を指定できます。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|アプリ|[appidentity](appidentity.md)|アクティビティを開始するリソースがアプリの場合、このプロパティは appId、name、servicePrincipalId、name などのアプリ関連情報をすべて示します。|
|user|[userIdentity](useridentity.md)|アクティビティを開始するリソースがユーザーの場合、このプロパティは、userId、Name、userprinicpalname など、すべてのユーザー関連情報を示します。|

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
