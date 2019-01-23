---
title: reportRoot リソースの種類
description: デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421334"
---
# <a name="reportroot-resource-type"></a>reportRoot リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ReportRoot の取得](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[reportRoot の更新](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。|
|**デバイス構成**|
|[deviceConfigurationUserActivity function](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|デバイス構成のユーザー アクティビティ レポートのメタデータ|
|[deviceConfigurationDeviceActivity function](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|デバイス構成のデバイス アクティビティ レポートのメタデータ|
|**トラブルシューティング**|
|[managedDeviceEnrollmentAbandonmentDetails 関数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[レポート](../resources/intune-shared-report.md)|登録放棄の詳細レポートのメタデータ|
|[managedDeviceEnrollmentAbandonmentSummary 関数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[レポート](../resources/intune-shared-report.md)|登録放棄の概要レポートのメタデータ|
|[managedDeviceEnrollmentFailureDetails 関数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|まだ文書化されていません|
|[managedDeviceEnrollmentFailureTrends 関数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|登録の失敗の傾向レポートのメタデータ|
|[managedDeviceEnrollmentTopFailures 関数](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|このエンティティの一意識別子です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



