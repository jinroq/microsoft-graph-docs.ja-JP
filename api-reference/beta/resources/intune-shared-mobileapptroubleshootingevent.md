---
title: mobileAppTroubleshootingEvent リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の mobileAppTroubleshootingEvent リソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfa126fea86c7edb302953efc3b88376f2d68a09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574447"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの管理とトラブルシューティングのイベントワークフローについて、ユーザーのデバイスアプリケーションのインストール状態を表すイベント。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)コレクション|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileAppTroubleshootingEvent を取得する](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppTroubleshootingEvent を作成する](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。|
|[mobileAppTroubleshootingEvent の削除](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|なし|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。|
|[mobileAppTroubleshootingEvent の更新](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの UUID。|
|**トラブルシューティング**|
|additionalinformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。|
|applicationId|String|Intune アプリケーション識別子。|
|correlationId|String|サービスのエラーをトレースするために使用される ID。 |
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 |
|eventName|String|トラブルシューティングイベントに対応するイベント名。 省略可能|
|履歴|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション|Intune モバイルアプリケーションのトラブルシューティングの履歴項目|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|トラブルシューティングのエラーの詳細|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|エラーとその修復に関する詳細情報を含むオブジェクト。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|userId|String|デバイスを登録しようとするユーザーの識別子。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**デバイスの管理**|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション|このプロパティは、を指定します。|


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
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
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




