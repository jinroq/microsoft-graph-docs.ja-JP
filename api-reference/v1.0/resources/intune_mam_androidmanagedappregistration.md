# <a name="androidmanagedappregistration-resource-type"></a>androidManagedAppRegistration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。
ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。

[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidManagedAppRegistrations のリスト](../api/intune_mam_androidmanagedappregistration_list.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) コレクション|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[androidManagedAppRegistration の取得](../api/intune_mam_androidmanagedappregistration_get.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidManagedAppRegistration の作成](../api/intune_mam_androidmanagedappregistration_create.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|新しい [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを作成します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|作成日時 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)。|
|lastSyncDateTime|DateTimeOffset|アプリが管理サービスと最後に同期した日時。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|applicationVersion|文字列|アプリのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|managementSdkVersion|文字列|アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|platformVersion|文字列|オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|deviceType|文字列|ホスト デバイスの種類 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|deviceTag|文字列|アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。 あらゆる状況でのアプリの関連付けを保証するものではありません。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|deviceName|文字列|ホスト デバイスの名前 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|flaggedReasons|[managedAppFlaggedReason 列挙型](../resources/intune_mam_managedappflaggedreason.md) のコレクション|アプリ登録にフラグが設定された、0 個以上の理由。 例: ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|userId|文字列|このアプリの登録が属するユーザー ID。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)|
|ID|文字列|エンティティのキー。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|version|文字列|エンティティのバージョン。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|intendedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|
|operations|[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション|アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppRegistration",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



