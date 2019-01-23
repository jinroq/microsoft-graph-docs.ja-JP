---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57e10fcabc0aa3def07872c0e520f09c6ee90fc3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411240"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a>mobileAppTroubleshootingAppStateHistory リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。


[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|履歴項目が発生した時刻です。 [MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。|
|actionType|[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)|AAD セキュリティ グループの id が対象となります。 可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。|
|runState|[runState](../resources/intune-shared-runstate.md)|項目の状態です。 可能な値は、`unknown`、`success`、`fail` です。|
|errorCode|String|障害なしの場合は、空のエラーのエラー コードです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```




