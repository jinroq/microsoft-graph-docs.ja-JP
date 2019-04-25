---
title: importedDeviceIdentityResult リソースの種類
description: importedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94eff5ea5e2ed37173341b45980e9b60437822d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524499"
---
# <a name="importeddeviceidentityresult-resource-type"></a>importedDeviceIdentityResult リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

importedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。


[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[importedDeviceIdentityResult を取得する](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[importedDeviceIdentityResult を作成する](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。|
|[importedDeviceIdentityResult の削除](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|なし|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を削除します。|
|[importedDeviceIdentityResult の更新](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の id|
|importedDeviceIdentifier|String|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス識別子|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の種類。 使用可能な値は、`unknown`、`imei`、`serialNumber` です。|
|lastModifiedDateTime|DateTimeOffset|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された説明の最終更新日時。|
|createdDateTime|DateTimeOffset|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの日時の作成日時|
|lastContactedDateTime|DateTimeOffset|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの最後の連絡日時。|
|description|String|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された Intune のデバイスの状態。 可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォーム。 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。 可能な値は `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS` です。|
|status|ブール値|インポートされたデバイス id の状態|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```





