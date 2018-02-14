# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune_onboarding_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceAppManagement](../api/intune_onboarding_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) オブジェクトのプロパティを更新します。|
|[syncMicrosoftStoreForBusinessApps アクション](../api/intune_onboarding_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|なし|ビジネス向け Microsoft Store と Intune アカウントを同期します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|ビジネス向け Microsoft Store のアプリがアカウントと正常に同期された最終日時。|
|isEnabledForMicrosoftStoreForBusiness|ブール型 (Boolean)|ビジネス向け Microsoft Store からのアプリケーションの同期がアカウントで有効かどうか。|
|microsoftStoreForBusinessLanguage|文字列型 (String)|ビジネス向け Microsoft Store からのアプリケーションの同期に使用するロケール情報。 国/地域に特有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式は <languagecode2>-<country/regioncode2> です。<languagecode2> は ISO 639-1 に基づく小文字 2 文字で構成されるコードで、<country/regioncode2> は ISO 3166 の基づく大文字 2 文字で構成されるコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



