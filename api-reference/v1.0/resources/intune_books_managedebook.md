# <a name="managedebook-resource-type"></a>managedEBook リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象電子ブックの基本プロパティを含む抽象クラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedEBook のリスト](../api/intune_books_managedebook_list.md)|[managedEBook](../resources/intune_books_managedebook.md) コレクション|[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedEBook の取得](../api/intune_books_managedebook_get.md)|[managedEBook](../resources/intune_books_managedebook.md)|[managedEBook](../resources/intune_books_managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[アクションの割り当て](../api/intune_books_managedebook_assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。|
|displayName|文字列|電子ブックの名前。|
|説明|文字列|説明。|
|パブリッシャー|文字列|発行元です。|
|publishedDateTime|DateTimeOffset|電子ブックが発行された日時。|
|大型カバー|[マイムコンテンツ](../resources/intune_shared_mimecontent.md)|ブック カバー。|
|createdDateTime|DateTimeOffset|電子ブック ファイルが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|電子ブックが最後に変更された日時。|
|informationUrl|文字列|詳細情報の URL。|
|privacyInformationUrl|文字列|プライバシーに関する声明の URL。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション|この電子ブックの割り当てのリストです。|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|モバイル アプリ インストール概要です。|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション|この電子ブックのインストール状態のリストです。|
|userStateSummary|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) コレクション|この電子ブックのインストール状態のリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```








