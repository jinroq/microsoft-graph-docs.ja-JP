---
title: officeClientCheckinStatus リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: a7cbc54ac2e276932273130f194f484f3ee23b7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949291"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントのチェックイン統計を記述するエンティティ。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userPrincipalName|String|デバイスを使用したユーザープリンシパル名。|
|deviceName|String|チェックインしようとしているデバイスの名前。|
|devicePlatform|String|チェックインしようとしているデバイスプラットフォーム。|
|devicePlatformVersion|String|デバイスプラットフォームのバージョンをチェックインしようとしています。|
|成功|Boolean|前回のチェックインが成功した場合。|
|userId|String|デバイスを使用するユーザー識別子。|
|checkinDateTime|DateTimeOffset|前回のデバイスのチェックイン時刻 (UTC)。|
|errorMessage|String|前回のチェックインに関連付けられたエラーメッセージ。|
|appliedPolicies|String collection|前回のチェックインとしてデバイスに配信されたポリシーの一覧です。|

## <a name="relationships"></a>関係
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



