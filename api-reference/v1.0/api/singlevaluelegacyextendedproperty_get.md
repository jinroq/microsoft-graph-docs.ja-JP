# <a name="get-singlevaluelegacyextendedproperty"></a>singleValueLegacyExtendedProperty を取得する

`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むリソース インスタンスを取得します。

クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトを取得する唯一の方法です。

クエリ パラメーター `$filter` を使用すると、**id** プロパティと **value** プロパティに対するフィルターと一致する拡張プロパティを持つ、指定したリソースのすべてのインスタンスを取得できます。フィルターは、サインインしているユーザーのメールボックス内のリソースのすべてのインスタンスに適用されます。

次のユーザー リソースがサポートされます。

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

次のグループ リソースもサポートされます。

- グループ [event](../resources/event.md)
- グループ [calendar](../resources/calendar.md)
- グループ [post](../resources/post.md) 

オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、取得するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

- Mail.Read
- Calendars.Read
- Contacts.Read
- Group.Read.All 

## <a name="http-request"></a>HTTP 要求

#### <a name="get-a-resource-instance-using-expand"></a>`$expand` を使用してリソース インスタンスを取得する
**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。

**message** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
**mailFolder** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

**event** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
**calendar** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
**contact** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
**contactFolder** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
グループ **event** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

グループ **post** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a>`$filter` を使用してリソース インスタンスを取得する

**id** プロパティと **value** プロパティに対するフィルターと一致する拡張プロパティを持つサポート対象リソースのインスタンスを取得します。 フィルター文字列内のコロン、スラッシュ、スペースに [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることをご確認ください。


**message** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**mailFolder** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

**event** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**calendar** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**contact** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**contactFolder** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
グループ **event** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

グループ **post** インスタンスの取得:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a>パラメーター
|**パラメーター**|**型**|**説明**|
|:-----|:-----|:-----|
|_URL parameters_|
|id_value|String|照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。|
|property_value |文字列|照合する拡張プロパティの値。 前述の「**HTTP 要求**」セクションに示した一覧で必要になります。 {property_value} が文字列ではない場合、`ep/value` を {property_value} と比較するときに、適切な Edm データ型に明示的にキャストしてください。 例については、以下の[要求 3](#request-3) を参照してください。 |

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。

#### <a name="get-resource-instance-using-expand"></a>`$expand` を使用してリソース インスタンスを取得する
応答本文には、一致する [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。
  
#### <a name="get-resource-instances-using-filter"></a>`$filter` を使用してリソース インスタンスを取得する
応答本文には、一致する拡張プロパティを含むリソース インスタンスを表す 1 つ以上のオブジェクトが含まれます。応答本文には、拡張プロパティは含まれません。

## <a name="example"></a>例
#### <a name="request-1"></a>要求 1

最初の例では、単一値の拡張プロパティを含めることによって指定されたメッセージを取得して展開します。フィルターは、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a>応答 1
応答本文には、指定されたメッセージのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。

注:簡潔にするために、ここに示す**メッセージ** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a>要求 2

2 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。 フィルターは、以下のような拡張プロパティを検索します。

- その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。

- その **value** は文字列 `Green` です。

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a>応答 2

正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。応答は、一致する拡張プロパティを含みません。


#### <a name="request-3"></a>要求 3

次の 2 つの例では、文字列以外で型指定された単一値の拡張プロパティを持つメッセージを取得する方法を示しています。 読みやすくするため、必要な URL エンコードは含まれていません。

次の例は、以下のような拡張プロパティを検索するフィルターを示しています。

- その **id** は文字列 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` と一致します。

- その **value** は GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b` です。 プロパティ値を GUID と比較するには、`ep/value` を `Edm.Guid` にキャストします。


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

次の例は、以下のような拡張プロパティを検索するフィルターを示しています。

- その **id** は文字列 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` と一致します。

- その **value** は整数 12 と等しくなります。 プロパティ値を整数と比較するには、`ep/value` を `Edm.Int32` にキャストします。


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-3"></a>応答 3

前の 2 つの例では、正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、対応するフィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。 応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。 応答は、一致する拡張プロパティを含みません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->