---
title: deviceManagement リソースの種類
description: 'deviceManagement リソースは、次のようなワークフローに従ってコンテンツが変化するコンテナーを表します。  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 08f04242b379fee6ebcc4496e10d342fd3ec342e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571913"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

deviceManagement リソースは、次のようなワークフローに従ってコンテンツが変化するコンテナーを表します。  

- 監査イベント  
- 会社の使用条件   
- デバイス構成の設定  
- デバイスの管理  
- Endpoint Protection  
- 登録プロファイル  
- 通知  
- オンボードポリシー、設定、詳細  
- 役割ベースのアクセス制御 (RBAC) ポリシー  
- リモートアシスタンスパートナー  
- 通信マネージャー se 管理パートナー  
- イベントのトラブルシューティング  
- Windows 情報保護の概要  

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceManagement](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。|
|**オンボーディング**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|まだ文書化されていません|
|**RBAC**|
|[getEffectivePermissions 関数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolepermission](../resources/intune-rbac-rolepermission.md)コレクションまたは文字列コレクション|現在の認証ユーザーの有効なアクセス許可を取得します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|**デバイス構成**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|subscriptionState|String|テナントのモバイル デバイス管理のサブスクリプション状態。 使用可能な値: `pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|**オンボーディング**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**監査**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md) コレクション|監査イベント|
|**会社の使用条件**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション|対象の会社のデバイス管理に関連付けられている条項および条件。|
|**デバイス構成**|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション|デバイス コンプライアンス ポリシーです。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|このアカウントのデバイス コンプライアンスの状態の要約です。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション|このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|このアカウントにおける、デバイス構成のデバイス状態の要約です。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション|デバイス構成です。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) コレクション|このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|ソフトウェア更新状態の概要です。|
|**デバイスの管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple プッシュ通知証明書。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|デバイスに関連付けられている、検出されたアプリの一覧。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|デバイスの概要|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|管理対象デバイスの一覧。|
|**登録**|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)コレクション|インポートされたWindows Autopilot デバイスのコレクション。|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)コレクション|Windows 自動操縦デバイスのコレクションをアップロードします。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション|通知メッセージ テンプレート。|
|**オンボーディング**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange のオンプレミスでの条件付きアクセス設定。 オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション|テナントを含むデバイスのカテゴリのリスト。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|デバイス登録の構成のリスト|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション|テナントによって構成されているデバイス管理パートナーのリスト。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) コレクション|テナントによって構成されている Exchange Connector のリスト。|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) コレクション|テナントによって構成されている、モバイルの脅威保護コネクタのリスト。|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション|リソースの操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) コレクション|ロールの割り当て。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション|ロールの定義。|
|**リモートアシスタンス**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション|リモート アシスタンス パートナー。|
|**通信経費管理**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション|通信経費の管理パートナー。|
|**トラブルシューティング**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|テナントのトラブルシューティング イベントの一覧です。|
|**Windows 情報保護**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) コレクション|Windows 情報保護アプリの学習概要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) コレクション|Windows 情報保護ネットワークの学習概要。|


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {"@odata.type": "microsoft.graph.intuneBrand"},
  "subscriptionState": "String",
  "settings": {"@odata.type": "microsoft.graph.deviceManagementSettings"}
}
```



