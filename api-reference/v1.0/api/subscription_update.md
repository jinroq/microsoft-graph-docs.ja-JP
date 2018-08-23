# <a name="update-subscription"></a>サブスクリプションを更新する

サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。

サブスクリプションは、リソースの種類によって異なる期間後に期限が切れます。 通知の欠落を回避するには、アプリケーションは、その有効期限前にサブスクリプションを更新する必要があります。 各リソースの種類のサブスクリプションの最大長については [サブスクリプション](../resources/subscription.md) を参照してください。

## <a name="permissions"></a>アクセス許可

次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

| リソースの種類/項目        | アクセス許可          |
|-----------------------------|---------------------|
| 連絡先                    | Contacts.Read       |
| スレッド               | Group.Read.All      |
| イベント                      | Calendars.Read      |
| メッセージ                    | Mail.Read           |
| グループ                      | Group.Read.All      |
| ユーザー                       | User.Read.All       |
| ドライブ (ユーザーの OneDrive)    | Files.ReadWrite     |
| ドライブ (SharePoint の共有コンテンツとドライブ) | Files.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| 承認  | 文字列  | ベアラー {トークン}。必須。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
