---
title: importedAppleDeviceIdentity リソースの種類
description: ImportedAppleDeviceIdentity リソースでは、アップル デバイスのインポートされたデバイス id を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae0f940614ae8b872891579957e8f86c92342da8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416826"
---
# <a name="importedappledeviceidentity-resource-type"></a>importedAppleDeviceIdentity リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ImportedAppleDeviceIdentity リソースでは、アップル デバイスのインポートされたデバイス id を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ImportedAppleDeviceIdentity を取得します。](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティと関係を参照してください。|
|[ImportedAppleDeviceIdentity を作成します。](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。|
|[ImportedAppleDeviceIdentity を削除します。](../api/intune-enrollment-importedappledeviceidentity-delete.md)|なし|の[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)を削除します。|
|[ImportedAppleDeviceIdentity を更新します。](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。|
|[importAppleDeviceIdentityList アクション](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|シリアル番号|String|デバイスのシリアル番号|
|requestedEnrollmentProfileId|String|登録プロファイル Id の管理者が、次の登録時にデバイスに適用しようとしています。|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|時間登録のプロファイルは、デバイスに割り当てられました。|
|isSupervised|Boolean|Apple デバイスが監視された状態を示します。 詳細についてでです。https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple のデバイス検出のソースです。 可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。|
|createdDateTime|DateTimeOffset|デバイスの作成日時|
|lastContactedDateTime|DateTimeOffset|最終アクセス日時、デバイスの|
|説明|String|デバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune でデバイスの状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォームです。 使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
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
  "platform": "String"
}
```




