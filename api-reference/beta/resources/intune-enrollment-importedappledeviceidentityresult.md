---
title: importedAppleDeviceIdentityResult リソースの種類
description: ImportedAppleDeviceIdentityResult リソースは、Apple デバイス id のインポートを試行した結果を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7359100d1da6e1d83f4acb199059c3b84001c38a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327921"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ImportedAppleDeviceIdentityResult リソースは、Apple デバイス id のインポートを試行した結果を表します。


[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクション|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ImportedAppleDeviceIdentityResult を取得する](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ImportedAppleDeviceIdentityResult を作成する](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|新しい[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを作成します。|
|[ImportedAppleDeviceIdentityResult の削除](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|None|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)を削除します。|
|[ImportedAppleDeviceIdentityResult の更新](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。|
|シリアル番号|String|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスのシリアル番号|
|requestedEnrollmentProfileId|String|登録プロファイル Id 管理者は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承した次の登録時にデバイスに適用する予定です。|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|時間登録プロファイルが[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスに割り当てられています。|
|isSupervised|Boolean|Apple デバイスが監視されているかどうかを示します。 詳細についてはhttps://support.apple.com/en-us/HT202837 、「 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承する」を参照してください。|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple デバイスの検出ソース。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。 可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。|
|createdDateTime|DateTimeOffset|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの日時の作成日時|
|lastContactedDateTime|DateTimeOffset|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの最後の連絡日時。|
|description|String|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承された Intune のデバイスの状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォーム。 [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。 使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|インポートされたデバイス id の状態|

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



