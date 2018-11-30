---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。
ms.openlocfilehash: a327840ce38dfd0d075ef37c7e92ef0e83b2054c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073955"
---
# <a name="importeddeviceidentity-resource-type"></a>importedDeviceIdentity リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ImportedDeviceIdentity を取得します。](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を参照してください。|
|[ImportedDeviceIdentity を作成します。](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。|
|[ImportedDeviceIdentity を削除します。](../api/intune-enrollment-importeddeviceidentity-delete.md)|なし|の[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。|
|[ImportedDeviceIdentity を更新します。](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。|
|[importDeviceIdentityList アクション](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|インポートされたデバイス id の id|
|importedDeviceIdentifier|String|インポートされたデバイスの識別子|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|インポートされたデバイスの識別情報の種類です。 可能な値は、`unknown`、`imei`、`serialNumber` です。|
|lastModifiedDateTime|DateTimeOffset|説明の最後の変更日時|
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





