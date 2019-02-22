---
title: office/リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5c36a23be0ab32a14a08eaff297b832ba5274c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156050"
---
# <a name="officeconfiguration-resource-type"></a>office/リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|オフィス/全情報の収集|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|このオブジェクトのプロパティとリレーションシップ[](../resources/intune-cirrus-officeconfiguration.md)を読み取ります。|
|officeの変更の更新|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|[オフィス](../resources/intune-cirrus-officeconfiguration.md)のプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|office 構成の Id。|
|tenantcheckinstatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション|office クライアントのチェックイン状態のリスト。|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|テナントのチェックイン statues を記述するエンティティ|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|clientconfigurations|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション|office クライアント構成のリスト。|

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



