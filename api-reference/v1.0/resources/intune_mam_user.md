# <a name="user-resource-type"></a>user リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Azure Active Directory ユーザー オブジェクトを表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List users](../api/intune_mam_user_list.md)|[user](../resources/intune_mam_user.md) コレクション|[user](../resources/intune_mam_user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get user](../api/intune_mam_user_get.md)|[user](../resources/intune_mam_user.md)|[user](../resources/intune_mam_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create user](../api/intune_mam_user_create.md)|[user](../resources/intune_mam_user.md)|新しい [user](../resources/intune_mam_user.md) オブジェクトを作成します。|
|[Delete user](../api/intune_mam_user_delete.md)|なし|[user](../resources/intune_mam_user.md) を削除します。|
|[Update user](../api/intune_mam_user_update.md)|[user](../resources/intune_mam_user.md)|[user](../resources/intune_mam_user.md) オブジェクトのプロパティを更新します。|
|[getManagedAppDiagnosticStatuses 関数](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) コレクション|特定のユーザーの診断検証状態を取得します。|
|[getManagedAppPolicies 関数](../api/intune_mam_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|特定のユーザーのアプリ制限を取得します。|
|[wipeManagedAppRegistrationsByDeviceTag アクション](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|ユーザー ID。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション|対象ユーザーに属する 0 個以上の管理対象アプリ登録。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



