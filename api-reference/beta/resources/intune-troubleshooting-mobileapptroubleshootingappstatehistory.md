---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
ms.openlocfilehash: ebe38b852c6c6926b69e75379bc1a029ade0bb98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332159"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a>mobileAppTroubleshootingAppStateHistory リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。

[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
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





