---
title: officeClientConfiguration リソースの種類
description: Office クライアントの構成。
ms.openlocfilehash: de510d7a57c10d1f74a3e58856afb9233243ec17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069441"
---
# <a name="officeclientconfiguration-resource-type"></a>officeClientConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Office クライアントの構成。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション|[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[OfficeClientConfiguration を取得します。](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[assign action](../api/intune-cirrus-officeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション|ポリシーのすべての対象とするグループを交換してください。|
|[updatePriorities アクション](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|なし|ポリシーの優先順位を更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Office クライアントの構成のポリシーの id。|
|userPreferencePayload|Stream|JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。|
|policyPayload|Stream|JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。|
|説明|String|まだ文書化されていません|
|displayName|String|管理者には、office クライアントの説明の構成のポリシーが用意されています。|
|lastModifiedDateTime|DateTime|ポリシーの最終変更された日付時刻スタンプ。|
|priority|Int32|優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|ポリシーの概要チェックのユーザーです。|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション|Office クライアントでは、チェック状態の一覧です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション|一連のポリシーの割り当てをグループ化します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
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
  ]
}
```



