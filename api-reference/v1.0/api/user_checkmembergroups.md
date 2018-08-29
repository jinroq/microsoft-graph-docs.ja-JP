# <a name="checkmembergroups"></a>checkMemberGroups

指定したグループ一覧内のメンバーシップを確認します。ユーザーのメンバーシップがダイレクト メンバーシップまたは推移性メンバーシップであるグループを一覧から返します。

要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | ~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                                                                                                     |
| アプリケーション                            | ~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All                             |

> **注:** この API では現在、`Directory.Read.All` 以上のアクセス権が必要です。 `User.Read.All` または `User.ReadWrite.All` アクセス許可を使用するとエラーが返されます。 これは既知のバグです。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
| :------------ | :------------------------ |
| 承認 | ベアラー {トークン}。必須。 |
| コンテンツ-種類  | アプリケーション /json          |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型              | 説明           |
| :-------- | :---------------- | :-------------------- |
| groupIds  | String コレクション | グループ ID の配列 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。

## <a name="example"></a>例

以下は、この API を呼び出す方法の例です。

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
