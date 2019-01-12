---
title: deviceManagementTroubleshootingEvent リソースの種類
description: 一般エラーを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd4fbf5448b9bd5347fd7cb4f7cfe5ef96790247
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917539"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a>deviceManagementTroubleshootingEvent リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

一般エラーを表すイベント。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceManagementTroubleshootingEvents](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|新しい [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを作成します。|
|[Delete deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|なし|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) を削除します。|
|[Update deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの UUID|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。|
|correlationId|String|サービスのエラーをトレースするための ID。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```



