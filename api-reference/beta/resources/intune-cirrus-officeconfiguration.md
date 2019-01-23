---
title: officeConfiguration リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc76295b21602328689ee48f8aed8be74bd82093
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406550"
---
# <a name="officeconfiguration-resource-type"></a>officeConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|OfficeConfiguration を取得します。|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|OfficeConfiguration を更新します。|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Office の構成の id です。|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション|Office クライアントでは、チェック状態の一覧です。|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|テナント チェックインの彫像を記述するエンティティ|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション|Office クライアントの構成の一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



