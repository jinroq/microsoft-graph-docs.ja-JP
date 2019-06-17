---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0b90b903c024377ad74509f8a16617b1dd28fb1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990968"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a>mobileAppTroubleshootingAppTargetHistory リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。


[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|履歴アイテムが発生した時刻。 [MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。|
|securityGroupId|String|対象となった AAD セキュリティグループ id。|
|runState|[runState](../resources/intune-shared-runstate.md)|アイテムの状態。 可能な値は、`unknown`、`success`、`fail` です。|
|errorCode|String|失敗のエラーコード。エラーがない場合は空です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```





