---
title: reportRoot リソースの種類
description: デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。
localization_priority: Normal
ms.openlocfilehash: 8a2c1cbc666698eea7f466c32bae6c404264f545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809647"
---
# <a name="reportroot-resource-type"></a>reportRoot リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|このエンティティの一意識別子です。|

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



