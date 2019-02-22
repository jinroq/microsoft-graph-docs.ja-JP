---
title: iosUpdateDeviceStatus リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35389cf2c7995a1b1ef479b8289b14d49cd984f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160257"
---
# <a name="iosupdatedevicestatus-resource-type"></a>iosUpdateDeviceStatus リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosUpdateDeviceStatuses のリスト](../api/intune-deviceconfig-iosupdatedevicestatus-list.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) コレクション|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosUpdateDeviceStatus の取得](../api/intune-deviceconfig-iosupdatedevicestatus-get.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosUpdateDeviceStatus の作成](../api/intune-deviceconfig-iosupdatedevicestatus-create.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|新しい [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを作成します。|
|[iosUpdateDeviceStatus の削除](../api/intune-deviceconfig-iosupdatedevicestatus-delete.md)|なし|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) を削除します。|
|[iosUpdateDeviceStatus の更新](../api/intune-deviceconfig-iosupdatedevicestatus-update.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)| [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|installStatus|[iosupの installstatus](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|ポリシー レポートのインストール状態。 可能な値は`success`、 `available`、 `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、です。 `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`|
|osVersion|String|レポートされているデバイス バージョン。|
|deviceId|String|レポートされているデバイス ID。|
|userId|String|レポートされているユーザー ID。|
|deviceDisplayName|String|DevicePolicyStatus のデバイス名。|
|userName|String|レポートされているユーザー名|
|deviceModel|String|レポートされているデバイス モデル|
|platform|Int32|レポートされているデバイスのプラットフォーム|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|ポリシー レポートのコンプライアンスの状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|lastReportedDateTime|DateTimeOffset|ポリシー レポートの最終変更日時。|
|userPrincipalName|文字列|UserPrincipalName。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```




