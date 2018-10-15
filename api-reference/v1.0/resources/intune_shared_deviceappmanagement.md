# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune_shared_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceAppManagement](../api/intune_shared_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトのプロパティを更新します。|
|**採用**|
|[syncMicrosoftStoreForBusinessApps アクション](../api/intune_shared_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|なし|ビジネス向け Microsoft Store と Intune アカウントを同期します|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|**採用**|
|isEnabledForMicrosoftStoreForBusiness|ブール値|アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。|
|microsoftStoreForBusinessLanguage|文字列|ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。 国/地域固有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**アプリ**|
|mobileAppCategories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|モバイル アプリ カテゴリ。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) コレクション|管理対象デバイスのモバイル アプリケーション構成。|
|mobileApps|[mobileApp](../resources/intune_apps_mobileapp.md) コレクション|モバイル アプリ。|
|**書籍**|
|managedEBooks|[managedEBook](../resources/intune_books_managedebook.md) コレクション|管理対象の電子ブック。|
|**モバイル アプリケーション管理 (MAM)**|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) コレクション|Android 管理対象アプリ ポリシーです。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) コレクション|既定の管理対象アプリ ポリシーです。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) コレクション|iOS 管理対象アプリ ポリシーです。|
|managedAppPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|管理対象アプリ ポリシーです。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション|管理対象アプリの登録です。|
|managedAppStatuses|[managedAppStatus](../resources/intune_mam_managedappstatus.md) コレクション|管理対象アプリの状態です。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) コレクション|MDM に登録されたデバイス上で実行されているアプリの Windows 情報保護です。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) コレクション|ターゲットとなる管理対象アプリの構成です。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) コレクション|MDM に登録されていないデバイス上で実行されているアプリの Windows 情報保護です。|
|**採用**|
|vppTokens|[vppToken](../resources/intune_onboarding_vpptoken.md) コレクション|この組織への Vpp トークンのリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。  これは、単なる一例です。実際のクエリのクエリ応答には、コンテキストに適切なプロパティが含まれます。  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



