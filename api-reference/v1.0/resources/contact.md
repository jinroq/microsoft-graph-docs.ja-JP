# <a name="contact-resource-type"></a>contact リソース型

連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。

このリソースは以下をサポートしています。

- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/contact_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[連絡先を取得する](../api/contact_get.md) | [連絡先](contact.md) |連絡先オブジェクトのプロパティとリレーションシップを読み取ります。|
|[作成](../api/user_post_contacts.md) | [連絡先](contact.md) |連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。|
|[更新する](../api/contact_update.md) | [連絡先](contact.md) |連絡先オブジェクトを更新します。 |
|[削除](../api/contact_delete.md) | なし |連絡先オブジェクトを削除します。 |
|[デルタ](../api/contact_delta.md)|[contact](contact.md)コレクション| 指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](../../../concepts/extensibility_schema_groups.md) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[連絡先](contact.md)  |新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ連絡先を取得する](../api/singlevaluelegacyextendedproperty_get.md)  | [連絡先](contact.md) | または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。`$expand` |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [連絡先](contact.md) | 新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ連絡先を取得する](../api/multivaluelegacyextendedproperty_get.md)  | [連絡先](contact.md) | を使用して、複数値の拡張プロパティを含む連絡先を取得します。`$expand` |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|assistantName|文字列|連絡先のアシスタントの名前。|
|誕生日|DateTimeOffset|連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|businessAddress|[PhysicalAddress](physicaladdress.md)|連絡先の勤務先の住所。|
|businessHomePage|文字列|連絡先の勤務先のホーム ページ。|
|businessPhones|String コレクション|連絡先の勤務先の電話番号。|
|カテゴリ|String コレクション|連絡先に関連付けられたカテゴリ。|
|changeKey|文字列|連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|子|String コレクション|連絡先の子供の名前。|
|companyName|文字列|連絡先の会社の名前。|
|createdDateTime|DateTimeOffset|連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|部署|文字列|連絡先の部署。|
|displayName|文字列|連絡先の表示名。|
|emailAddresses|[EmailAddress](emailaddress.md) コレクション|連絡先のメール アドレス。|
|フラグ|[FollowupFlag](followupflag.md)|メッセージのステータス、開始日、期限、または完了日を示すフラグ値。|
|fileAs|文字列|連絡先がファイルされる名前。|
|生成|文字列|連絡先の世代。|
|givenName|文字列|連絡先の名。|
|homeAddress|[PhysicalAddress](physicaladdress.md)|連絡先の自宅住所。|
|homePhones|String コレクション|連絡先の自宅の電話番号。|
|ID|文字列|連絡先の一意識別子。読み取り専用。|
|imAddresses|String コレクション|連絡先のインスタント メッセージング (IM) アドレス。|
|イニシャル|文字列|連絡先のイニシャル。|
|jobTitle|文字列|連絡先の役職。|
|lastModifiedDateTime|DateTimeOffset|連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|マネージャー|文字列|連絡先の上司の名前。
|middleName|文字列|連絡先のミドル ネーム。|
|mobilePhone|文字列|連絡先の携帯電話番号。|
|nickName|文字列|連絡先のニックネーム。|
|officeLocation|文字列|連絡先のオフィスの所在地。|
|otherAddress|[PhysicalAddress](physicaladdress.md)|連絡先の別の住所。|
|parentFolderId|文字列|連絡先の親フォルダーの ID。|
|personalNotes|文字列|連絡先に関するユーザーのメモ。|
|職業|文字列|連絡先の専門的職業。|
|spouseName|文字列|連絡先の配偶者/パートナーの名前。|
|姓|文字列|連絡先の姓。|
|タイトル|文字列|連絡先の肩書。|
|yomiCompanyName|文字列|連絡先の会社名の読み仮名。|
|yomiGivenName|文字列|連絡先の名 (ファースト ネーム) の読み仮名。|
|yomiSurname|文字列|連絡先の姓 (ラスト ネーム) の読み仮名。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|拡張機能|[extension](extension.md) コレクション|連絡先に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| 連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|写真|[profilePhoto](profilephoto.md)| 連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| 連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](../../../concepts/delta_query_overview.md)
- [フォルダー内のメッセージへの増分変更を取得する](../../../concepts/delta_query_messages.md)
- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
