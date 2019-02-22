---
title: androidOmaCpConfiguration リソースの種類
description: このプロファイルに構成を提供することで、oma-uri をサポートする Android デバイスを構成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d002568597d5fea2bd895d6d49a7f8cdd886c071
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178088"
---
# <a name="androidomacpconfiguration-resource-type"></a>androidOmaCpConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、oma-uri をサポートする Android デバイスを構成できます。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidOmaCpConfigurations](../api/intune-deviceconfig-androidomacpconfiguration-list.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)コレクション|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidOmaCpConfiguration を取得する](../api/intune-deviceconfig-androidomacpconfiguration-get.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidOmaCpConfiguration を作成する](../api/intune-deviceconfig-androidomacpconfiguration-create.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|新しい[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)オブジェクトを作成します。|
|[androidOmaCpConfiguration の削除](../api/intune-deviceconfig-androidomacpconfiguration-delete.md)|なし|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)を削除します。|
|[androidOmaCpConfiguration の更新](../api/intune-deviceconfig-androidomacpconfiguration-update.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)|[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|configurationxml|Binary|デバイスに適用される構成 XML。 読み取り時に、元のデータが暗号化されて保存されるため、プレースホルダー文字列のみが提供されます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidOmaCpConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
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
  "configurationXml": "binary"
}
```




