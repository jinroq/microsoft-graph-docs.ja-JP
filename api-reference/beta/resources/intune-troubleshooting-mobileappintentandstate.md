---
title: mobileAppIntentAndState リソースの種類
description: MobileApp の意図と特定のデバイスのインストールの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 689945d1e2f7e7a1c33e9bc098dc64ad16472bd5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947247"
---
# <a name="mobileappintentandstate-resource-type"></a>mobileAppIntentAndState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MobileApp の意図と特定のデバイスのインストールの状態です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション|[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MobileAppIntentAndState を取得します。](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を参照してください。|
|[MobileAppIntentAndState を作成します。](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。|
|[MobileAppIntentAndState を削除します。](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|なし|の[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を削除します。|
|[MobileAppIntentAndState を更新します。](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの UUID|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|userId|String|デバイスを登録しようとするユーザーの識別子。|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション|ペイロードの目的と、テナントの状態の一覧です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```





