---
title: importedDeviceIdentity リソースの種類
description: importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151227"
---
# <a name="importeddeviceidentity-resource-type"></a>importedDeviceIdentity リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[importedDeviceIdentity を取得する](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[importedDeviceIdentity を作成する](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。|
|[importedDeviceIdentity の削除](../api/intune-enrollment-importeddeviceidentity-delete.md)|なし|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。|
|[importedDeviceIdentity の更新](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。|
|[importDeviceIdentityList アクション](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|インポートされたデバイス id の id|
|importedDeviceIdentifier|String|インポートされたデバイス識別子|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|インポートされたデバイス id の種類。 可能な値は `unknown`、`imei`、`serialNumber` です。|
|lastModifiedDateTime|DateTimeOffset|説明の最終更新日時|
|createdDateTime|DateTimeOffset|デバイスの日時の作成日時|
|lastContactedDateTime|DateTimeOffset|デバイスの最終連絡日時|
|説明|String|デバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune でのデバイスの状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォーム。 使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




