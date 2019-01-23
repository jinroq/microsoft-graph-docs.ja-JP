---
title: windowsOfficeClientSecurityConfiguration リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ba8d6f59d6e37a6aa0ce39da01a68d5b71d272c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419213"
---
# <a name="windowsofficeclientsecurityconfiguration-resource-type"></a>windowsOfficeClientSecurityConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsOfficeClientSecurityConfigurations](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-list.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)コレクション|[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsOfficeClientSecurityConfiguration を取得します。](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsOfficeClientSecurityConfiguration を作成します。](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|新しい[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを作成します。|
|[WindowsOfficeClientSecurityConfiguration を削除します。](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-delete.md)|なし|の[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)を削除します。|
|[WindowsOfficeClientSecurityConfiguration を更新します。](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Office クライアントの構成のポリシーの id。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|userPreferencePayload|Stream|JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|policyPayload|Stream|JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|説明|String|管理者には、office クライアントの説明の構成のポリシーが用意されています。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|displayName|String|管理者は、office クライアントの構成のポリシーの名前を提供します。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|priority|Int32|優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|lastModifiedDateTime|DateTime
|ポリシーの最終変更された日付時刻スタンプ。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|ポリシーの概要チェックのユーザーです。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション|Office クライアントでは、チェック状態の一覧です。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション|一連のポリシーの割り当てをグループ化します。 [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientSecurityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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



