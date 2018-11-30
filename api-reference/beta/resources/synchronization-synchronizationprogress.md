---
title: synchronizationProgress リソースの種類
description: 完了するまで、synchronizationJob の進行状況を表します。
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074097"
---
# <a name="synchronizationprogress-resource-type"></a>synchronizationProgress リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

完了するまでの[synchronizationJob](synchronization-synchronizationjob.md)の進行状況を表します。

## <a name="properties"></a>プロパティ

| プロパティ                              | 型      | 説明    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|分子の進行状況の比率です。既に処理された変更単位の数です。|
|progressObservationDateTime|DateTimeOffset|分 UTC からのオフセットとしての進行状況の監視の時間です。|
|totalUnits|Int32|分母の進行状況の比率です。変更の同期を実行する処理の単位数を示します。|
|単位|String|単位のオプションの説明です。|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
