---
title: windows10SecureAssessmentConfiguration リソースの種類
description: このトピックでは、secureAssessment リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
localization_priority: Normal
ms.openlocfilehash: 954bc43a6b179e2b5a680dfe4f6368b5990312e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846026"
---
# <a name="windows10secureassessmentconfiguration-resource-type"></a>windows10SecureAssessmentConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、secureAssessment リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windows10SecureAssessmentConfigurations のリスト](../api/intune-deviceconfig-windows10secureassessmentconfiguration-list.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) コレクション|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windows10SecureAssessmentConfiguration の取得](../api/intune-deviceconfig-windows10secureassessmentconfiguration-get.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows10SecureAssessmentConfiguration の作成](../api/intune-deviceconfig-windows10secureassessmentconfiguration-create.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)|新しい [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを作成します。|
|[windows10SecureAssessmentConfiguration の削除](../api/intune-deviceconfig-windows10secureassessmentconfiguration-delete.md)|なし|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) を削除します。|
|[windows10SecureAssessmentConfiguration の更新](../api/intune-deviceconfig-windows10secureassessmentconfiguration-update.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)|[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|launchUri|String|安全性評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。 有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。|
|configurationAccount|String|Windows デバイスにテストを受けさせる際に、それを構成するために使用するアカウント。 ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com)、ローカル アカウント (username) のいずれでも可能です。|
|allowPrinting|Boolean|テスト中にアプリが印刷することを許可するかどうかを示します。|
|allowScreenCapture|Boolean|テスト中に画面キャプチャ機能を許可するかどうかを示します。|
|allowTextSuggestion|Boolean|テスト中に入力ヒントを許可するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10SecureAssessmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "launchUri": "String",
  "configurationAccount": "String",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



