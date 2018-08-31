# <a name="termsandconditionsacceptancestatus-resource-type"></a>termsAndConditionsAcceptanceStatus リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[termsAndConditionsAcceptanceStatuses のリスト](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) コレクション|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[termsAndConditionsAcceptanceStatus を取得する](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[termsAndConditionsAcceptanceStatus を作成する](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|新しい [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを作成します。|
|[termsAndConditionsAcceptanceStatus を削除する](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|なし|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) を削除します。|
|[termsAndConditionsAcceptanceStatus を更新する](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティの一意識別子。|
|userDisplayName|文字列|エンティティによって承諾が示されているユーザーの表示名。|
|acceptedVersion|Int32|ユーザーによって承諾された使用条件の最新バージョン番号。|
|acceptedDateTime|DateTimeOffset|最後に使用条件がユーザーによって承諾された DateTime。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|割り当てられた使用条件へのナビゲーション リンク。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



