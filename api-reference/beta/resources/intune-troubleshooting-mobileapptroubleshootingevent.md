---
title: mobileAppTroubleshootingEvent リソースの種類
description: ユーザー デバイスのアプリケーションを表すイベントは、状態をインストールします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8441015f594d227066db39f3f643cc8136637668
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846369"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ユーザー デバイスのアプリケーションを表すイベントは、状態をインストールします。

[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppTroubleshootingEvents](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)コレクション|[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MobileAppTroubleshootingEvent を取得します。](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を参照してください。|
|[MobileAppTroubleshootingEvent を作成します。](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|新しい[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトを作成します。|
|[MobileAppTroubleshootingEvent を削除します。](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|なし|の[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)を削除します。|
|[MobileAppTroubleshootingEvent を更新します。](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|correlationId|String|サービスのエラーをトレースするための ID。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|userId|String|デバイスを登録しようとするユーザーの識別子。|
|applicationId|文字列型 (String)|Intune アプリケーション識別子です。|
|履歴|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション|Intune モバイル アプリケーションの履歴項目のトラブルシューティング|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





