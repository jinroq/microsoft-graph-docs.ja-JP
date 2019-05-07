---
title: auditActivityInitiator リソースの種類
description: アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして認識される) を指定できます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5de4cc65379a3386137c7da79a10c5492dd1427
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629349"
---
# <a name="auditactivityinitiator-resource-type"></a>auditActivityInitiator リソースの種類

アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリと見なされる) を使用できます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|アプリ|[appIdentity](appidentity.md)|アクティビティを開始するリソースがアプリの場合、このプロパティは appId、Name、servicePrincipalId、Name などのアプリ関連情報をすべて示します。|
|user|[userIdentity](useridentity.md)|アクティビティを開始するリソースがユーザーの場合、このプロパティは、userId、Name、UserPrinicpalName など、すべてのユーザー関連情報を示します。|

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
