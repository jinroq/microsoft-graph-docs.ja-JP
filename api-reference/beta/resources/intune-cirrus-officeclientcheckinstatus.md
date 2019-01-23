---
title: officeClientCheckinStatus リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403260"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

チェックインのテナント統計 (stats) を記述するエンティティです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userPrincipalName|String|ユーザー プリンシパル名は、デバイスを使用します。|
|deviceName|String|チェックインしようとするデバイスの名前。|
|devicePlatform|String|デバイスのプラットフォームにチェックインしようとします。|
|devicePlatformVersion|String|デバイス プラットフォームのバージョンがチェックインをしようとします。|
|wasSuccessful|Boolean|最後のチェックインが正常に完了しました。 場合、|
|userId|String|デバイスを使用してユーザーの識別子です。|
|checkinDateTime|DateTimeOffset|最後デバイス チェックの時間 (utc) です。|
|エラー メッセージ|String|最後のチェックインに関連付けられている場合のエラー メッセージです。|
|appliedPolicies|String コレクション|ポリシーの一覧では、最後のチェックインと、デバイスに配信されます。|

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



