# <a name="create-domain"></a>ドメインを作成する

テナントにドメインを追加します。

**重要**:所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。詳細については、「[verificationDnsRecords の一覧](domain_list_verificationdnsrecords.md)」を参照してください。ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
要求本文で、[domain](../resources/domain.md) オブジェクトの JSON 表記を指定します。

> 要求本文には、新しいドメインの id プロパティが含まれます。id は指定できる唯一のプロパティで、必須です。id プロパティ値は、作成する完全修飾ドメイン名です。

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求

要求本文で、[domain](../resources/domain.md) オブジェクトの JSON 表記を指定します。

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a>応答
注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->