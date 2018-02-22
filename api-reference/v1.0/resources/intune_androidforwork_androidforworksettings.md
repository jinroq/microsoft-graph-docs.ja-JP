# <a name="androidforworksettings-resource-type"></a>androidForWorkSettings リソース タイプ

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android for Work の設定です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_get.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_update.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) オブジェクトのプロパティを更新します。|
|[requestSignupUrl action](../api/intune_androidforwork_androidforworksettings_requestsignupurl.md)|String|Android for Work 管理の登録に使用されるサインアップ URL を生成します。|
|[completeSignup action](../api/intune_androidforwork_androidforworksettings_completesignup.md)|なし|Android for Work 管理用のサインアップのフローを完了します。|
|[syncApps action](../api/intune_androidforwork_androidforworksettings_syncapps.md)|なし|エンタープライズ用の承認済みアプリケーションを同期します。|
|[unbind action](../api/intune_androidforwork_androidforworksettings_unbind.md)|なし|エンタープライズ用の Android for Work 管理を無効にします。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Android for Work の設定の識別子|
|bindStatus|String|Google EMM API を使ったテナントのバインドの状態。可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。|
|lastAppSyncDateTime|DateTimeOffset|アプリ同期の最終完了時刻|
|lastAppSyncStatus|String|前回のアプリケーションの同期結果。可能な値は、`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none` です。|
|ownerUserPrincipalName|String|エンタープライズを作成した所有者の UPN|
|ownerOrganizationName|String|Android for Work のオンボーディング時に使用される組織名|
|lastModifiedDateTime|DateTimeOffset|Android for Work の設定の最終変更時刻|
|enrollmentTarget|String|どのユーザーが Android for Work デバイス管理にデバイスを登録できるかを示します。可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。|
|targetGroupIds|String コレクション|enrollmentTarget が「Targeted」に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ]
}
```



