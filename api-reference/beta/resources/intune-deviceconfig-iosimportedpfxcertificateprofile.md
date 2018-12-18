---
title: iosImportedPFXCertificateProfile リソースの種類
description: iOS PFX インポート証明書プロファイル
author: tfitzmac
ms.openlocfilehash: 32f88e982e193516269aa8715c4f7e2274295f70
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314722"
---
# <a name="iosimportedpfxcertificateprofile-resource-type"></a>iosImportedPFXCertificateProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS PFX インポート証明書プロファイル

[IosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosImportedPFXCertificateProfiles](../api/intune-deviceconfig-iosimportedpfxcertificateprofile-list.md)|[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)コレクション|[IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosImportedPFXCertificateProfile を取得します。](../api/intune-deviceconfig-iosimportedpfxcertificateprofile-get.md)|[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)|[IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[IosImportedPFXCertificateProfile を作成します。](../api/intune-deviceconfig-iosimportedpfxcertificateprofile-create.md)|[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)|新しい[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトを作成します。|
|[IosImportedPFXCertificateProfile を削除します。](../api/intune-deviceconfig-iosimportedpfxcertificateprofile-delete.md)|なし|の[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)を削除します。|
|[IosImportedPFXCertificateProfile を更新します。](../api/intune-deviceconfig-iosimportedpfxcertificateprofile-update.md)|[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)|[IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール型|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|intendedPurpose|[intendedPurpose](../resources/intune-deviceconfig-intendedpurpose.md)|まだ記載されていません。 可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)コレクション|デバイスの証明書の状態|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosImportedPFXCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "intendedPurpose": "String"
}
```





