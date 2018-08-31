# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

DeviceManagement リソースは、ワークフローに従って内容を変更する、以下を含むコンテナーを表します。

- イベントの監査
- 企業の諸条件 
- 企業登録のプロファイル
- デバイス構成の設定
- デバイスの管理
- エンドポイントの保護
- 登録プロファイル
- 通知
- 採用ポリシー、設定、および詳細情報
- 役割ベースのアクセス制御 (RBAC) のポリシー
- リモート アシスタンスのパートナー
- 電気通信の効率的管理のパートナー
- イベントのトラブルシューティング
- Windows 情報保護のサマリー

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune_shared_devicemanagement_get.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagement の更新](../api/intune_shared_devicemanagement_update.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトのプロパティを更新します。|
|**採用**|
|[verifyWindowsEnrollmentAutoDiscovery 関数](../api/intune_shared_devicemanagement_verifywindowsenrollmentautodiscovery.md)|ブール値|まだ文書化されていません|
|**RBAC**|
|[getEffectivePermissions 関数](../api/intune_shared_devicemanagement_geteffectivepermissions.md)|[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション、または文字列のコレクション|現在の認証ユーザーの有効なアクセス許可を取得します|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|デバイスの一意識別子|
|**デバイス構成**|
|設定|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|subscriptionState|文字列|テナントのモバイル デバイス管理のサブスクリプション状態。 指定できる値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|**採用**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**監査**|
|auditEvents|[auditEvent](../resources/intune_auditing_auditevent.md) コレクション|監査イベント|
|**企業の諸条件**|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) コレクション|対象の会社のデバイス管理に関連付けられている条項および条件。|
|**デバイス構成**|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) コレクション|デバイス コンプライアンス ポリシーです。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|このアカウントのデバイス コンプライアンスの状態の要約です。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) コレクション|このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|このアカウントにおける、デバイス構成のデバイス状態の要約です。|
|deviceConfigurations|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) コレクション|デバイス構成です。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) コレクション|このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|ソフトウェア更新状態の概要です。|
|**デバイスの管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple プッシュ通知証明書。|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md) コレクション|デバイスに関連付けられている、検出されたアプリの一覧。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|デバイスの概要|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|管理対象デバイスの一覧。|
|**登録**|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)コレクション|インポートされた Windows Autopilot デバイスのコレクション。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) コレクション|通知メッセージ テンプレート。|
|**採用**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|Exchange のオンプレミスでの条件付きアクセス設定。 オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります|
|deviceCategories|[deviceCategory](../resources/intune_shared_devicecategory.md) コレクション|テナントを含むデバイスのカテゴリのリスト。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) コレクション|デバイス登録の構成のリスト|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) コレクション|テナントによって構成されているデバイス管理パートナーのリスト。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) コレクション|テナントによって構成されている Exchange Connector のリスト。|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) コレクション|テナントによって構成されている、モバイルの脅威保護コネクタのリスト。|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune_rbac_resourceoperation.md) コレクション|リソースの操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) コレクション|ロールの割り当て。|
|roleDefinitions|[roleDefinition](../resources/intune_rbac_roledefinition.md) コレクション|ロールの定義。|
|**リモート アシスタンス**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) コレクション|リモート アシスタンス パートナー。|
|**通信経費の管理**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) コレクション|通信経費の管理パートナー。|
|**トラブルシューティング**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション|テナントのトラブルシューティング イベントの一覧です。|
|**Windows 情報保護**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) コレクション|Windows 情報保護アプリの学習概要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) コレクション|Windows 情報保護ネットワークの学習概要。|


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



