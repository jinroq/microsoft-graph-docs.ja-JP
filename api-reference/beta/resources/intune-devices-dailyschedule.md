---
title: 社員のリソースの種類
description: 定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。
author: tfitzmac
ms.openlocfilehash: 86a3dda75c0aecef6ba0672bc114092bd301a582
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351129"
---
# <a name="dailyschedule-resource-type"></a>社員のリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。

[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|interval|Int32|間隔の日数|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





