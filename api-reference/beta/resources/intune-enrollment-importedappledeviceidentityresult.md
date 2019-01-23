---
title: importedAppleDeviceIdentityResult リソースの種類
description: ImportedAppleDeviceIdentityResult リソースでは、Apple のデバイス id をインポートしようとした結果を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a559b12cff17771667747baa9f91ddd9e3ede892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415692"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ImportedAppleDeviceIdentityResult リソースでは、Apple のデバイス id をインポートしようとした結果を表します。


[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクション|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ImportedAppleDeviceIdentityResult を取得します。](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティと関係を参照してください。|
|[ImportedAppleDeviceIdentityResult を作成します。](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|新しい[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを作成します。|
|[ImportedAppleDeviceIdentityResult を削除します。](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|なし|の[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)を削除します。|
|[ImportedAppleDeviceIdentityResult を更新します。](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。|
|シリアル番号|String|継承されるデバイス ・ シリアル番号は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から|
|requestedEnrollmentProfileId|String|登録プロファイル Id の管理者が、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、次の登録時に、デバイスに適用しようとしています。|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|時間登録のプロファイルは、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスに割り当てられました。|
|isSupervised|Boolean|Apple デバイスが監視された状態を示します。 詳細については、: https://support.apple.com/en-us/HT202837 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple のデバイス検出のソースです。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。 可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。|
|createdDateTime|DateTimeOffset|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの日時を作成|
|lastContactedDateTime|DateTimeOffset|最終接続日時[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスの|
|説明|String|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune 継承で[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)からのデバイスの状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォームです。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。 使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|インポートされたデバイス id のステータス|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




