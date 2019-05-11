---
title: windows81WifiImportConfiguration リソースの種類
description: Windows 8.1 以降の wi-fi インポート構成。 このプロファイルを構成することにより、Windows 8.1 以降のデバイスに、目的の Wi-fi エンドポイントに接続するよう指示することができます。 Windows 8.1 デバイスを目的の wi-fi ネットワークに接続し、そのデバイスから XML を抽出して、後でこの Wi-fi プロファイルに埋め込む。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a383c254667a4eb621eaad18cddc56bc8d86a44c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944167"
---
# <a name="windows81wifiimportconfiguration-resource-type"></a>windows81WifiImportConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 8.1 以降の wi-fi インポート構成。 このプロファイルを構成することにより、Windows 8.1 以降のデバイスに、目的の Wi-fi エンドポイントに接続するよう指示することができます。 Windows 8.1 デバイスを目的の wi-fi ネットワークに接続し、そのデバイスから XML を抽出して、後でこの Wi-fi プロファイルに埋め込む。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windows81WifiImportConfigurations](../api/intune-deviceconfig-windows81wifiimportconfiguration-list.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)コレクション|[Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[Windows81WifiImportConfiguration を取得する](../api/intune-deviceconfig-windows81wifiimportconfiguration-get.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|[Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Windows81WifiImportConfiguration を作成する](../api/intune-deviceconfig-windows81wifiimportconfiguration-create.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|新しい[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトを作成します。|
|[Windows81WifiImportConfiguration の削除](../api/intune-deviceconfig-windows81wifiimportconfiguration-delete.md)|None|[Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)を削除します。|
|[Windows81WifiImportConfiguration の更新](../api/intune-deviceconfig-windows81wifiimportconfiguration-update.md)|[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)|[Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|payloadFileName|String|ペイロードファイル名 (* .xml)。|
|profileName|String|UI に表示されるプロファイル名。|
|payload|Binary|ペイロード。 (UTF8 でエンコードされたバイト配列)。 これは、Wi-fi エンドポイントへの接続に使用したデバイスに保存された XML ファイルです。|

## <a name="relationships"></a>関係
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
  "@odata.type": "microsoft.graph.windows81WifiImportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "String",
  "profileName": "String",
  "payload": "binary"
}
```




