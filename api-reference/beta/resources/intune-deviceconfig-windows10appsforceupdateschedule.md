---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリケーションの Windows 10 強制更新のスケジュール
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef8a0583bd02a62a4461a3415aae86833e24e948
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811236"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>windows10AppsForceUpdateSchedule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリケーションの Windows 10 強制更新のスケジュール
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|力の開始時刻を再起動します。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期的なスケジュールです。 可能な値は、`none`、`daily`、`weekly`、`monthly` です。|
|runImmediatelyIfAfterStartDateTime|ブール型|True の場合、タスクはすぐに実行させるまでは、他の次の反復の実行の場合です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





