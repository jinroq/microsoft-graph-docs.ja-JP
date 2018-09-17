# <a name="iosvppebook-resource-type"></a>iosVppEBook リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS Vpp eBook のプロパティを含むクラスです。

[managedEBook](../resources/intune_books_managedebook.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosVppEBooks のリスト](../api/intune_books_iosvppebook_list.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md) コレクション|[iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppEBook の取得](../api/intune_books_iosvppebook_get.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppEBook の作成](../api/intune_books_iosvppebook_create.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|新しい [iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトを作成します。|
|[iosVppEBook の削除](../api/intune_books_iosvppebook_delete.md)|なし|[iosVppEBook](../resources/intune_books_iosvppebook.md) を削除します。|
|[iosVppEBook の更新](../api/intune_books_iosvppebook_update.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|displayName|文字列|電子ブックの名前。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|説明|文字列|説明。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|発行元|文字列|発行元です。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|publishedDateTime|DateTimeOffset|電子ブックが発行された日時。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|largeCover|[マイムコンテンツ](../resources/intune_shared_mimecontent.md)|ブック カバー。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|createdDateTime|DateTimeOffset|電子ブック ファイルが作成された日時。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|電子ブックが最後に変更された日時。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|informationUrl|文字列|詳細情報の URL。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|privacyInformationUrl|文字列|プライバシーに関する声明の URL。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|vppTokenId|GUID 型 (GUID)|Vpp トークン ID。|
|appleId|文字列|Vpp トークンに関連付けられている Apple ID。|
|vppOrganizationName|文字列|Vpp トークンの組織の名前。|
|ジャンル|String コレクション|ジャンル。|
|言語|文字列|言語。|
|販売元|文字列|販売元。|
|totalLicenseCount|Int32|ライセンスの合計数。|
|usedLicenseCount|Int32|使用されているライセンスの数。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション|この電子ブックの割り当てのリストです。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|モバイル アプリ インストール概要です。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション|この電子ブックのインストール状態のリストです。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|
|userStateSummary|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) コレクション|この電子ブックのインストール状態のリストです。 [managedEBook](../resources/intune_books_managedebook.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedEBook",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```








