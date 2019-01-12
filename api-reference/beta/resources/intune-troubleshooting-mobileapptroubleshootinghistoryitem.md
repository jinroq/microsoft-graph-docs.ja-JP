---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 713bf06c65bd8d651e1d885d41876822d62eade1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947240"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a>mobileAppTroubleshootingHistoryItem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|履歴項目が発生した時刻です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





