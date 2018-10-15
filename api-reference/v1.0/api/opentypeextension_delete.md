# <a name="delete-open-extension"></a>オープン拡張機能を削除する

指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を削除します。 

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、拡張機能を削除するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|**サポートされているリソース**|**アクセス許可**|**サポートされているリソース**|**アクセス許可** |
|:-----|:-----|:-----|:-----|
| [デバイス](../resources/device.md) | Device.ReadWrite.All | [イベント](../resources/event.md) | Calendars.ReadWrite |
| [グループ](../resources/group.md) | Group.ReadWrite.All | [グループ イベント](../resources/event.md) | Group.ReadWrite.All |
| [グループの投稿](../resources/post.md) | Group.ReadWrite.All | [メッセージ](../resources/message.md) | Mail.ReadWrite |
| [組織](../resources/organization.md) | Directory.AccessAsUser.All | [個人用連絡先](../resources/contact.md) | Contacts.ReadWrite |
| [ユーザー](../resources/user.md) | Directory.AccessAsUser.All | | |

## <a name="http-request"></a>HTTP 要求
要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

>**注:** 上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。

## <a name="path-parameters"></a>パス パラメーター
|パラメーター|型|説明|
|:-----|:-----|:-----|
|ID|文字列|対応するコレクションのインスタンスの一意識別子。必須。|
|extensionId|文字列|これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。|

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 値 |
|:---------------|:----------|
| 承認 | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

2 番目の例では、指定されたグループ イベントの拡張機能を削除します。

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->