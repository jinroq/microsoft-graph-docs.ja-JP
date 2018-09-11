# <a name="managedappregistration-resource-type"></a>managedAppRegistration リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAppRegistrations の一覧表示](../api/intune_mam_managedappregistration_list.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAppRegistration の取得](../api/intune_mam_managedappregistration_get.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。|
|[getUserIdsWithFlaggedAppRegistration 関数](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|String コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|作成日時|
|lastSyncDateTime|DateTimeOffset|アプリが管理サービスと最後に同期した日付と時刻。|
|applicationVersion|文字列|アプリのバージョン|
|managementSdkVersion|文字列|アプリ管理の SDK バージョン|
|platformVersion|文字列|オペレーティング システムのバージョン|
|deviceType|文字列|ホスト デバイスの種類|
|deviceTag|文字列|アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。 あらゆる状況でのアプリの関連付けを保証するものではありません。|
|deviceName|文字列|ホスト デバイスの名前|
|flaggedReasons|[managedAppFlaggedReason 列挙型](../resources/intune_mam_managedappflaggedreason.md) のコレクション|アプリ登録にフラグが設定された、0 個以上の理由。 例: ルートのデバイスで実行されているアプリ|
|userId|文字列|このアプリの登録が属するユーザー ID。|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|アプリ パッケージの識別子|
|ID|文字列|エンティティのキー。|
|バージョン|文字列|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。|
|intendedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。|
|operations|[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション|アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```








