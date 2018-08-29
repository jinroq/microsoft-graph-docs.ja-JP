# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[onPremisesConditionalAccessSettings の取得](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[onPremisesConditionalAccessSettings の更新](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|まだ文書化されていません|
|enabled|ブール値|対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。|
|includedGroups|Guid コレクション|オンプレミスの条件付きアクセスで対象となるユーザー グループ。 これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。|
|excludedGroups|Guid コレクション|オンプレミスの条件付きアクセスで除外されるユーザー グループ。 これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。|
|overrideDefaultRule|ブール値|デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "fe4d7f2b-e7b8-4276-9976-7a3fc83edbbc"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```



