# <a name="update-organization"></a>組織を更新する

現在認証されている組織のプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。 最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|marketingNotificationEmails|String コレクション|                                        **注**: Null は許容されません。            |
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)|組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。            |
|securityComplianceNotificationMails|String collection||
|securityComplianceNotificationPhones|String コレクション||
|technicalNotificationMails|String コレクション| 

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

<br/>

### <a name="response"></a>応答

以下は、応答の例です。 **注**:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
