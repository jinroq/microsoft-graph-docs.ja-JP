---
title: deviceManagement リソースの種類
description: 'deviceManagement リソースは、次のようなワークフローに従ってコンテンツが変化するコンテナーを表します。  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 23ea35468bbff4010b5ed089b086fbb6cd7a9845
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163029"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

deviceManagement リソースは、次のようなワークフローに従ってコンテンツが変化するコンテナーを表します。  

- Android for Work アプリの設定
- 監査イベント
- 会社の使用条件 
- 会社の登録プロファイル
- デバイス構成の設定
- デバイスの管理
- 電子 SIM (ESIM)
- フェンス
- 通知
- オンボードポリシー、設定、詳細
- リモートアクセス
- リモートアシスタンスパートナー
- 役割ベースのアクセス制御 (RBAC) ポリシー
- 通信マネージャー se 管理パートナー
- イベントのトラブルシューティング
- Windows 情報保護の概要

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagement の更新](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。|
|**デバイス構成**|
|[enableLegacyPcManagement アクション](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|なし|まだ文書化されていません|
|**デバイスの管理**|
|[sendCustomNotificationToCompanyPortal アクション](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|なし|まだ文書化されていません|
|**オンボーディング**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|まだ文書化されていません|
|**役割ベースのアクセス制御 (RBAC)**|
|[getEffectivePermissions 関数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション|現在の認証ユーザーの有効なアクセス許可を取得します|
|[getRoleScopeTagsByIds 関数](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション|まだ文書化されていません|
|[getRoleScopeTagsByResource 関数](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション|まだ文書化されていません|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスに関連付けられている一意の識別子。|
|**デバイス構成**|
|int未指定 eaccountid|Guid|指定したテナントの Intune アカウント ID|
|legacyPcManangementEnabled|Boolean|このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。 このプロパティは読み取りのみ可能です。|
|maximumdeptokens|Int32|テナントごとに許容される DEP トークンの最大数。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|accountMoveCompletionDateTime|DateTimeOffset|& が、scaleunits 間でテナントデータを移動した日時です。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|管理者の同意情報。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|デバイス保護の概要。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|デバイスクリーンアップルール|
|subscriptionState|[devicemanagementsubscriptionstate](../resources/intune-devices-devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|講読|[devicemanagementsubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|テナントのサブスクリプション。 使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|windows デバイスのマルウェアの概要。|
|**オンボーディング**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|Description&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション|Android デバイス所有者登録プロファイルエンティティ。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) コレクション|Android for Work アプリの構成スキーマ アイテムのエンティティです。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) コレクション|Android for Work 登録プロファイルのエンティティです。|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|単一の Android for Work 設定エンティティです。|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|単一の Android 管理ストアアカウントのエンタープライズ設定エンティティ。|
|androidmanagedstoreappconfigurationschemas|[androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)コレクション|Android エンタープライズアプリ構成スキーマエンティティ。|
|**監査**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md) コレクション|監査イベント|
|**会社の用語**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション|対象の会社のデバイス管理に関連付けられている条項および条件。|
|**企業の登録**|
|enrollmentProfiles|[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション|登録プロファイル。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション|インポートされた Apple デバイスの id です。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|インポートされたデバイス id。|
|**デバイス構成**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|このアカウントの ATP のオンボード状態の概要の状態。|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|買い物カゴからクラスへの関連付け。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション|デバイス コンプライアンス ポリシーです。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|このアカウントのデバイス コンプライアンスの状態の要約です。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション|このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)コレクション|このアカウントの競合状態にあるポリシーの概要。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|このアカウントにおける、デバイス構成のデバイス状態の要約です。|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション|このアカウントの制限されたアプリの違反。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション|デバイス構成です。|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|このアカウントのデバイス構成のユーザー状態の概要。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) コレクション|このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。|
|conditionalaccesssettings|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|このアカウントの Ndes コネクタのコレクション。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|ソフトウェア更新状態の概要です。|
|**デバイスの管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple プッシュ通知証明書。|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション|データ共有同意。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|デバイスに関連付けられている、検出されたアプリの一覧。|
|deviceManagementScripts|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)コレクション|テナントに関連付けられているデバイス管理スクリプトのリスト。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|デバイスの概要|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|管理対象デバイスの一覧。|
|remoteactionaudits|[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)コレクション|デバイスのリモートアクションの一覧は、テナントに対して監査されます。|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)コレクション|テナント内の影響を受けるマルウェアのリスト。|
|**登録**|
|depOnboardingSettings|[deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)コレクション|テナントごとの複数の DEP トークンのコレクション。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|インポートされたデバイス id。|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)コレクション|インポートされたWindows Autopilot デバイスのコレクション。|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)コレクション|Windows 自動操縦デバイスのコレクションをアップロードします。|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)コレクション|Windows 自動パイロット展開プロファイル|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|Windows 自動操縦デバイス id にはコレクションが含まれています。|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Windows 自動操縦アカウントの設定。|
|**埋め込み SIM**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)コレクション|このアカウントによって作成された埋め込み SIM アクティブ化コードプール。|
|**フェンス**|
|managementconditions|[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション|会社のデバイス管理に関連付けられている管理条件。|
|managementconditionstatements|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|会社のデバイス管理に関連付けられている管理条件ステートメント。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション|通知メッセージ テンプレート。|
|**オンボーディング**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange のオンプレミスでの条件付きアクセス設定。 オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション|テナントを含むデバイスのカテゴリのリスト。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|デバイス登録の構成のリスト|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション|テナントによって構成されているデバイス管理パートナーのリスト。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) コレクション|テナントによって構成されている Exchange Connector のリスト。|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)コレクション|プレミスの Exchange の一覧は、テナントによって構成されたポリシーです。|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|オンプレミスの Exchange へのモバイルデバイスのアクセスを制御するポリシー|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) コレクション|テナントによって構成されている、モバイルの脅威保護コネクタのリスト。|
|**リモートアクセス**|
|userPfxCertificates|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション|ユーザーに関連付けられている PFX 証明書のコレクション。|
|**リモートアシスタンス**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション|リモート アシスタンス パートナー。|
|**役割ベースのアクセス制御 (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション|リソースの操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) コレクション|ロールの割り当て。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション|ロールの定義。|
|roleScopeTags|[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション|役割のスコープタグ。|
|**電気通信経費管理 (TEM)**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション|通信経費の管理パートナー。|
|**トラブルシューティング**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|テナントのトラブルシューティング イベントの一覧です。|
|**Windows 情報保護**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション|AAD グループを対象とした Intune ブランド化プロファイル|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) コレクション|Windows 情報保護アプリの学習概要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) コレクション|Windows 情報保護ネットワークの学習概要。|


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



