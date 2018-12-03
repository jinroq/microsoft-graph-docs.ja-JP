---
title: deviceManagement リソースの種類
description: 'DeviceManagement リソースが、ワークフローに従って、内容を変更するコンテナーを表しますを含みます。  '
ms.openlocfilehash: 14303da517e26158d1432a67076e64424a40253c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070215"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

DeviceManagement リソースが、ワークフローに従って、内容を変更するコンテナーを表しますを含みます。  

- Android for Work アプリの設定
- イベントの監査
- 企業の諸条件 
- 企業登録のプロファイル
- デバイス構成の設定
- デバイスの管理
- 電子 SIM (ESIM)
- フェンス
- 通知
- 契約時のポリシー、設定、および詳細情報
- リモート アクセス
- リモート アシスタンスのパートナー
- 役割ベースのアクセス制御 (RBAC) のポリシー
- 電気通信の効率的管理のパートナー
- イベントのトラブルシューティング
- Windows の情報保護の概要

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagement の更新](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。|
|**デバイス構成**|
|[enableLegacyPcManagement アクション](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|なし|まだ文書化されていません|
|**デバイスの管理**|
|[sendCustomNotificationToCompanyPortal アクション](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|なし|まだ文書化されていません|
|**契約時**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|まだ文書化されていません|
|**ロール ベースのアクセス制御 (RBAC)**|
|[getEffectivePermissions 関数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション|現在の認証ユーザーの有効なアクセス許可を取得します|
|[getRoleScopeTagsByIds 関数](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション|まだ文書化されていません|
|[getRoleScopeTagsByResource 関数](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション|まだ文書化されていません|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスに関連付けられている一意の識別子です。|
|**デバイス構成**|
|intuneAccountId|Guid|Intune アカウント ID にはテナントが指定されました。|
|legacyPcManangementEnabled|Boolean|非 MDM を有効にするプロパティは、このアカウントの従来の PC の管理を管理します。 このプロパティは値の取得のみ可能です。|
|maximumDepTokens|Int32|DEP のトークンの最大数では、テナントごとに許可されます。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|accountMoveCompletionDateTime|DateTimeOffset|日付と時刻 scaleunits のテナントのデータを移動するときです。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|同意の情報を管理します。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|デバイス保護の概要です。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|デバイスのクリーンアップ ・ ルール|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|サブスクリプション|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|テナントのサブスクリプション。 使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Windows デバイスのマルウェアの概要です。|
|**契約時**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**作業のアプリ**|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション|Android デバイスの所有者の登録プロファイル エンティティです。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) コレクション|Android for Work アプリの構成スキーマ アイテムのエンティティです。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) コレクション|Android for Work 登録プロファイルのエンティティです。|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|単一の Android for Work 設定エンティティです。|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|シングルトンのアプリの管理では、アカウントのエンタープライズ設定エンティティを保存します。|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)コレクション|Android エンタープライズ アプリケーションの構成スキーマのエンティティです。|
|**監査**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md) コレクション|監査イベント|
|**会社の用語**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション|対象の会社のデバイス管理に関連付けられている条項および条件。|
|**企業登録**|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション|登録のプロファイルです。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション|インポートされたアップルのデバイス id です。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|インポートされたデバイス id です。|
|**デバイス構成**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|このアカウントの ATP 契約時の状態の状態の概要です。|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|クラスの関連するカートです。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) コレクション|デバイス コンプライアンス ポリシーです。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|このアカウントのデバイス コンプライアンスの状態の要約です。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) コレクション|このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)コレクション|このアカウントの競合状態のポリシーの概要です。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|このアカウントにおける、デバイス構成のデバイス状態の要約です。|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション|このアカウントの違反をアプリケーションに制限されています。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) コレクション|デバイス構成です。|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|デバイス構成ユーザーの状態このアカウントの概要です。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) コレクション|このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。|
|ndesConnectors|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|Ndes のコネクタには、このアカウントのコレクションです。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|ソフトウェア更新状態の概要です。|
|**デバイスの管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple プッシュ通知証明書。|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション|共有データにお客様が同意します。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|デバイスに関連付けられている、検出されたアプリの一覧。|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)コレクション|テナントに関連付けられているデバイスの管理スクリプトの一覧です。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|デバイスの概要|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|管理対象デバイスの一覧。|
|remoteActionAudits|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)コレクション|デバイスのリモート操作の一覧は、テナントを監査します。|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)コレクション|テナントに影響を受けるマルウェアのリスト。|
|**登録**|
|depOnboardingSettings|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)コレクション|複数 DEP トークン テナントごとのコレクションがこのします。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション|インポートされたデバイス id です。|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)コレクション|インポートされたWindows Autopilot デバイスのコレクション。|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)コレクション|デバイスをアップロード、Windows 自動操縦装置のコレクションです。|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)コレクション|Windows 自動パイロット展開のプロファイル|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|Windows の自動操縦装置のデバイス id には、コレクションが含まれています。|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Windows 自動操縦のアカウントの設定です。|
|**埋め込み SIM**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)コレクション|埋め込み SIM アクティベーション コード プールこのアカウントで作成されました。|
|**フェンス**|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション|会社のデバイスの管理に関連付けられている管理の条件です。|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|会社のデバイスの管理に関連付けられている管理の条件ステートメントです。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション|通知メッセージ テンプレート。|
|**契約時**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange のオンプレミスでの条件付きアクセス設定。 オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) コレクション|テナントを含むデバイスのカテゴリのリスト。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|デバイス登録の構成のリスト|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション|テナントによって構成されているデバイス管理パートナーのリスト。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) コレクション|テナントによって構成されている Exchange Connector のリスト。|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)コレクション|テナントで構成されている Exchange の Premisis ポリシーの一覧です。|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|モバイル デバイスの設置型の Exchange へのアクセスを制御するポリシー|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) コレクション|テナントによって構成されている、モバイルの脅威保護コネクタのリスト。|
|**リモート アクセス**|
|userPfxCertificates|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション|ユーザーに関連付けられている証明書を PFX のコレクションです。|
|**リモート アシスタンス**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション|リモート アシスタンス パートナー。|
|**ロール ベースのアクセス制御 (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション|リソースの操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) コレクション|ロールの割り当て。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション|ロールの定義。|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)コレクション|ロールのスコープのタグ。|
|**通信費管理 (TEM)**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション|通信経費の管理パートナー。|
|**トラブルシューティング**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|テナントのトラブルシューティング イベントの一覧です。|
|**Windows 情報の保護**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション|Intune の AAD のグループを対象としたプロファイルをブランド化|
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



