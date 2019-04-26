---
title: 同期の進行状況リソースの種類
description: 完了までの同期ジョブの進行状況を表します。
localization_priority: Normal
ms.openlocfilehash: d05193c7c242dc3f890aba6f4fcec5a8badc087f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340015"
---
# <a name="synchronizationprogress-resource-type"></a>同期の進行状況リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

完了までの[同期ジョブ](synchronization-synchronizationjob.md)の進行状況を表します。

## <a name="properties"></a>プロパティ

| プロパティ                              | 型      | 説明    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|進行状況の比率の分子。既に処理されている変更の単位数。|
|進行法|DateTimeOffset|進行状況の監視時間 (分単位で UTC からのオフセット)。|
|totalunits|Int32|進行状況の比率の分母。同期を実行するために処理される変更の単位数。|
|」|String|単位の説明 (省略可能)。|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
