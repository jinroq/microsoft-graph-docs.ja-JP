# <a name="person-resource-type"></a>person リソースの種類

メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ユーザーを一覧表示する](../api/user_list_people.md) | **人物** |[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。|
|[人物を取得する](../api/person_get.md) | **人物** |person オブジェクトのプロパティと関係を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|birthday|String|人物の誕生日。|
|companyName|String|人物の会社名。|
|department|String|人物の部署。|
|displayName|String|人物の表示名。|
|scoredEmailAddresses|[scoredEmailAddress](scoredemailaddress.md) コレクション|人物の電子メール アドレス。|
|givenName|String|人物に指定された名前。|
|id|String|人物の一意の識別子。読み取り専用です。|
|imAddress|String|ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。|
|isFavorite|Boolean|ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。|
|jobTitle|String|人物の役職。|
|officeLocation|String|人物のオフィスの所在地。|
|personNotes|String|ユーザーがこの人物について記入した自由形式のメモ。|
|personType|[personType](persontype.md) コレクション|人物の種類。|
|phones|[phone](phone.md) コレクション|人物の電話番号。|
|postalAddresses|[location](location.md) コレクション|人物のアドレス。|
|profession|String|人物の職業。|
|surname|String|人物の姓。|
|userPrincipalName|String|人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。|
|websites|[website](website.md) コレクション|人物の Web サイト。|
|yomiCompany|String|人物の会社の日本名の読み仮名。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
