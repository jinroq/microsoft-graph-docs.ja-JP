---
title: windowsIdentityProtectionConfiguration リソースの種類
description: このエンティティは、Windows Hello for business が公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 751d9d5e7528a3c2d49e71fa2150617ef153e671
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777180"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>windowsIdentityProtectionConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティは、Windows Hello for business が公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)コレクション|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsIdentityProtectionConfiguration を取得する](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsIdentityProtectionConfiguration を作成する](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。|
|[windowsIdentityProtectionConfiguration の削除](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|なし|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)を削除します。|
|[windowsIdentityProtectionConfiguration の更新](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|useSecurityKeyForSignin|Boolean|ログオン資格情報として Windows Hello セキュリティキーを有効にするために使用されるブール値。|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolean|Windows Hello 顔認証で顔機能認識の強化されたスプーフィング対策を有効にするために使用するブール値。|
|pinMinimumLength|Int32|Windows Hello for business の PIN に必要な最小文字数を設定する整数値。 有効な値は、4 ~ 127 の範囲で、最大 PIN の値を設定します。 有効な値は 4 ~ 127|
|pinMaximumLength|Int32|作業 PIN に使用できる最大文字数を設定する整数値。 有効な値は、最小 PIN で設定された値以上の4から127の範囲です。 有効な値は 4 ~ 127|
|pinUppercaseCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|この値は、Windows Hello for Business の PIN での大文字の使用を構成します。 使用可能な値は、`blocked`、`required`、`allowed` です。|
|pinLowercaseCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|この値は、Windows Hello for Business の PIN に小文字を使用するように構成します。 使用可能な値は、`blocked`、`required`、`allowed` です。|
|pinSpecialCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。 使用可能な値は、`blocked`、`required`、`allowed` です。|
|pinExpirationInDays|Int32|[整数値] PIN の変更をユーザーに要求する前に PIN を使用できる期間 (日数) を指定します。 有効な値は0から730の範囲です。 有効な値は 0 から 730 までです|
|pinPreviousBlockCount|Int32|ユーザーが過去の pin を使用できないようにする機能を制御します。 0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。 0に設定すると、以前の pin は保存されません。 pin をリセットすると、pin 履歴は保持されません。 有効な値は 0 から 50 までです|
|pinrecoveryenabled|Boolean|ユーザーが Windows Hello for business pin 回復サービスを使用して pin を変更できるようにするブール値。|
|securityDeviceRequired|Boolean|Windows Hello for business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。 TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。 False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for business をプロビジョニングできます。|
|unlockWithBiometricsEnabled|ブール型 (Boolean)|Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。  False に設定すると、生体認証ジェスチャは許可されません。 ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。|
|useCertificatesForOnPremisesAuthEnabled|Boolean|Windows Hello for business が証明書を使用してオンプレミスのリソースを認証できるようにするブール値。|
|windowsHelloForBusinessBlocked|Boolean|windows Hello for business を windows にサインインするための方法としてブロックするブール値。|

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
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "pinExpirationInDays": 1024,
  "pinPreviousBlockCount": 1024,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





