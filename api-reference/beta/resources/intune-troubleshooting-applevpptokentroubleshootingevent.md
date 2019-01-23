---
title: appleVppTokenTroubleshootingEvent リソースの種類
description: アップル Vpp トークンのトラブルシューティング イベントを表すイベントです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 14bae4be12f45d5f101d434b43f285ddabd80183
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430325"
---
# <a name="applevpptokentroubleshootingevent-resource-type"></a>appleVppTokenTroubleshootingEvent リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アップル Vpp トークンのトラブルシューティング イベントを表すイベントです。


[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト appleVppTokenTroubleshootingEvents](../api/intune-troubleshooting-applevpptokentroubleshootingevent-list.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)コレクション|[AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AppleVppTokenTroubleshootingEvent を取得します。](../api/intune-troubleshooting-applevpptokentroubleshootingevent-get.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|[AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティと関係を参照してください。|
|[AppleVppTokenTroubleshootingEvent を作成します。](../api/intune-troubleshooting-applevpptokentroubleshootingevent-create.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|新しい[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを作成します。|
|[AppleVppTokenTroubleshootingEvent を削除します。](../api/intune-troubleshooting-applevpptokentroubleshootingevent-delete.md)|なし|の[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)を削除します。|
|[AppleVppTokenTroubleshootingEvent を更新します。](../api/intune-troubleshooting-applevpptokentroubleshootingevent-update.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|[AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|correlationId|String|サービスのエラーをトレースするための ID。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|エラーとその修復に関する詳細情報を含むオブジェクトです。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|eventName|String|トラブルシューティング イベントに対応するイベントの名前です。 [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承される省略可能なフィールドします。|
|について|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるトラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセット|
|tokenId|String|Apple ボリューム購入プログラム トークンの識別子です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVppTokenTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  "tokenId": "String"
}
```




