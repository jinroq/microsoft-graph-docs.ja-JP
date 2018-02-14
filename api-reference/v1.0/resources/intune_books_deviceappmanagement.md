# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune_books_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceAppManagement](../api/intune_books_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedEBooks|[managedEBook](../resources/intune_books_managedebook.md) コレクション|管理対象の電子ブック。|

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
  "id": "String (identifier)"
}
```



