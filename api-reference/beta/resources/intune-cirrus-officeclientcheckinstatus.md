---
title: officeClientCheckinStatus リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
ms.openlocfilehash: a87a085d42ce0754e046b319b270ddf90a3bdba7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069091"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

チェックインのテナント統計 (stats) を記述するエンティティです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userPrincipalName|String|ユーザー プリンシパル名は、デバイスを使用します。|
|deviceName|String|チェックインしようとするデバイスの名前。|
|devicePlatform|String|デバイスのプラットフォームにチェックインしようとします。|
|devicePlatformVersion|String|デバイス プラットフォームのバージョンがチェックインをしようとします。|
|wasSuccessful|ブール値|最後のチェックインが正常に完了しました。 場合、|
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



