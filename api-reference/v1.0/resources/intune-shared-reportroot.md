---
title: reportRoot リソースの種類
description: 履歴レポートのインスタンスを表すリソースです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53fedc78575e48d77419a598b73e1760c8c6457c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850289"
---
# <a name="reportroot-resource-type"></a>reportRoot リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

履歴レポートのインスタンスを表すリソースです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ReportRoot の取得](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[reportRoot の更新](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。|
|**デバイス構成**|
|[deviceConfigurationDeviceActivity function](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[レポート](../resources/intune-shared-report.md)|デバイス構成のデバイス アクティビティ レポートのメタデータ|
|[deviceConfigurationUserActivity function](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[レポート](../resources/intune-shared-report.md)|デバイス構成のユーザー アクティビティ レポートのメタデータ|
|**トラブルシューティング**|
|[managedDeviceEnrollmentFailureDetails 関数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[レポート](../resources/intune-shared-report.md)|まだ記載されていません。|
|[managedDeviceEnrollmentTopFailures 関数](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[レポート](../resources/intune-shared-report.md)|まだ記載されていません。|


## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|このエンティティの一意識別子です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
