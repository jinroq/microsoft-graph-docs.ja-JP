---
title: りんご evpptokenのトラブルシューティングイベントリソースの種類
description: Apple Vpp トークントラブルシューティングイベントを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13459e2d8f76111137014918246fe1a573a191cd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160467"
---
# <a name="applevpptokentroubleshootingevent-resource-type"></a>りんご evpptokenのトラブルシューティングイベントリソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple Vpp トークントラブルシューティングイベントを表すイベント。


[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リストりんご evpptokenトラブルシューティングイベント](../api/intune-troubleshooting-applevpptokentroubleshootingevent-list.md)|[りんご evpptokenトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)コレクション|"[りんご evpptokenトラブルシューティング" イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[作業中の作業のトラブルシューティングイベントを取得する](../api/intune-troubleshooting-applevpptokentroubleshootingevent-get.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|この[イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[「りんご evpptokenトラブルシューティングイベントを作成する」](../api/intune-troubleshooting-applevpptokentroubleshootingevent-create.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|新しい[りんご evpptokenのトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを作成します。|
|[[りんご evpptokenトラブルシューティングイベントを削除する]](../api/intune-troubleshooting-applevpptokentroubleshootingevent-delete.md)|なし|"[りんご evpptoken" トラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)を削除します。|
|[更新プログラム (りんご evpptoken) のトラブルシューティングイベント](../api/intune-troubleshooting-applevpptokentroubleshootingevent-update.md)|[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)|" [sevpptokenトラブルシューティング" イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|correlationId|文字列型 (String)|サービスのエラーをトレースするための ID。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|トラブルシューティングのエラーの詳細|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|エラーとその修復に関する詳細情報を含むオブジェクト。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|eventName|String|トラブルシューティングイベントに対応するイベント名。 [devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです|
|additionalinformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。|
|tokenid|String|Apple volume purchase program のトークン識別子です。|

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




