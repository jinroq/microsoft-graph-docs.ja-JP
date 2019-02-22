---
title: officeClientCheckinStatus リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156057"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントのチェックイン統計を記述するエンティティ。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userPrincipalName|文字列|デバイスを使用したユーザープリンシパル名。|
|deviceName|String|チェックインしようとしているデバイスの名前。|
|devicePlatform|String|チェックインしようとしているデバイスプラットフォーム。|
|deviceplatformversion|String|デバイスプラットフォームのバージョンをチェックインしようとしています。|
|成功|ブール値|前回のチェックインが成功した場合。|
|userId|String|デバイスを使用するユーザー識別子。|
|checkinDateTime|DateTimeOffset|前回のデバイスのチェックイン時刻 (UTC)。|
|errorMessage|String|前回のチェックインに関連付けられたエラーメッセージ。|
|appliedPolicies|String collection|前回のチェックインとしてデバイスに配信されたポリシーの一覧です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
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
```



