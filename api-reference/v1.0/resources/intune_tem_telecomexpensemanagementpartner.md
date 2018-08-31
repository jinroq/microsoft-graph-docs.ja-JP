# <a name="telecomexpensemanagementpartner-resource-type"></a>telecomExpenseManagementPartner リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。 貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[telecomExpenseManagementPartners のリスト](../api/intune_tem_telecomexpensemanagementpartner_list.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) コレクション|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[telecomExpenseManagementPartner の取得](../api/intune_tem_telecomexpensemanagementpartner_get.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[telecomExpenseManagementPartner の作成](../api/intune_tem_telecomexpensemanagementpartner_create.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|新しい [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトを作成します。|
|[telecomExpenseManagementPartner の削除](../api/intune_tem_telecomexpensemanagementpartner_delete.md)|なし|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) を削除します。|
|[telecomExpenseManagementPartner の更新](../api/intune_tem_telecomexpensemanagementpartner_update.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|TEM パートナーの一意識別子。|
|displayName|文字列|TEM パートナーの表示名。|
|url|文字列|TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。|
|appAuthorized|ブール値|パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。|
|enabled|ブール値|TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。|
|lastConnectionDateTime|DateTimeOffset|TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```



