# <a name="create-invitation"></a>招待状の作成

この API を使用して、新しい [招待状](../resources/invitation.md) を作成します。招待状によって外部ユーザーが組織に追加されます。

新しい招待状を作成するときに、選択可能ないくつかのオプションがあります。

1. 招待状の作成に際して、Microsoft Graph は自動的に招待メールを招待ユーザーに直接送信できます。作成応答で返された *inviteRedeemUrl* をアプリが使用して、招待ユーザーへの (任意の通信メカニズムによる) 独自の招待状を作成することもできます。Microsoft Graph によって招待メールが自動的に送信されるようにする場合は、[*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) を使用してメールの内容と言語を制御できます。
2. ユーザーが招待されると、(userType Guest) のユーザー エンティティが作成され、リソースへのアクセスの制御に使用できるようになります。招待ユーザーは、招待されたリソースにアクセスするためには、引き換え処理を行う必要があります。

### <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかのスコープが必要です。*User.Invite.All*、*User.ReadWrite.All*、*Directory.ReadWrite.All*

### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
### <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

### <a name="request-body"></a>要求本文
要求本文で、[invitation](../resources/invitation.md) オブジェクトの JSON 表記を指定します。

次の表に、招待状の作成時に必要になるプロパティを示します。

| パラメーター | 型 | 説明|
|:---------------|:--------|:----------|
|invitedUserEmailAddress |string | 招待するユーザーのメール アドレス。|
|inviteRedirectUrl |string |引き換え後にユーザーがリダイレクトされる URL。|


### <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [invitation](../resources/invitation.md) オブジェクトを返します。

### <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitations"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```
