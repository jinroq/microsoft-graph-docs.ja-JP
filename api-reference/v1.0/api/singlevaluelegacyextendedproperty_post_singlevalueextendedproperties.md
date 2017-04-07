# <a name="create-single-value-extended-property"></a>単一値の拡張プロパティを作成する

リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。 

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

## <a name="prerequisites"></a>前提条件

この API を実行するには、拡張プロパティを作成する次のリソースの種類に応じて、以下の**スコープ**のいずれかが必要です。

- _Mail.ReadWrite_
- _Calendars.ReadWrite_
- _Contacts.ReadWrite_
- _Group.ReadWrite.All_
 
## <a name="http-request"></a>HTTP 要求
新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。

1 つ以上の拡張プロパティを_新しい_リソースのインスタンスに作成するには、インスタンスの作成と同じ REST 要求を使用し、新しいリソース インスタンスのプロパティ_と拡張プロパティを_要求の本文に含めます。一部のリソースでは複数の作成方法がサポートされていますので、注意してください。これらのリソース インスタンスの作成に関して詳しくは、[メッセージ](../resources/message.md)、[mailFolder](../api/user_post_mailfolders.md)、[イベント](../api/user_post_events.md)、[予定表](../api/user_post_calendars.md)、[連絡先](../api/user_post_contacts.md)、[contactFolder](../api/user_post_contactfolders.md)、[グループ イベント](../api/group_post_events.md)、および [グループ投稿](../resources/post.md)作成の該当する各トピックをご覧ください。 
 
以下に要求の構文を示します。 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。

**注** 既存のグループ投稿には拡張プロパティを作成できません。

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```


## <a name="parameters"></a>パラメーター
|**パラメーター**|**型**|**説明**|
|:-----|:-----|:-----|
|_URL parameters_|
|id|string|該当するコレクション内のオブジェクトの一意識別子。必須。|
|_Body parameters_|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection| 1 つ以上の単一値を持つ拡張プロパティの配列。 |
|id|String|**singleValueExtendedProperties** コレクションの各プロパティに対して、これを指定することでプロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。|
|value|string|**singleValueExtendedProperties** コレクションの各プロパティについて、プロパティの値を特定します。必須。|


## <a name="request-headers"></a>要求ヘッダー
| 名前       | 値 |
|:---------------|:----------|
| Authorization | Bearer %token%|
| Content-Type | application/json |

## <a name="request-body"></a>要求本文

リソース インスタンスの **singleValueExtendedProperties** コレクション プロパティに、各 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトの JSON 本文を指定します。

_新しい_リソース インスタンスに拡張プロパティを作成する場合は、新しい **singleValueExtendedProperties**コレクションのほか、そのリソース インスタンスの JSON 表現を指定します ([message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md) など)。

## <a name="response"></a>応答

#### <a name="response-code"></a>応答コード
新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。

既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。 


#### <a name="response-body"></a>応答本文

拡張プロパティを作成する場合、応答には新規または既存のインスタンスのみを含めて、新しい拡張プロパティは含めません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/singlevaluelegacyextendedproperty_get.md)します。

スレッドまたは投稿に返信することで、_新しい_[グループ投稿](../resources/post.md)に拡張プロパティを作成する場合、応答には応答コードのみを含めて、新しい投稿や拡張プロパティは含めません。



## <a name="example"></a>例
##### <a name="request-1"></a>要求 1

最初の例では、同じ POST 操作で新しいイベントと単一値の拡張プロパティを作成します。新しいイベントに通常含めるプロパティとは別に、1 つの単一値の拡張プロパティを含む **singleValueExtendedProperties** コレクションを要求の本文に含め、そのプロパティは次のようにします。
- **id** は、プロパティの型を `String` (GUID) として指定し、`Fun` という名前のプロパティとして指定します。
- **value** は、`Fun` プロパティの値として `Food` を指定します。 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a>応答 1

[イベントのみの作成](../api/user_post_events.md)からの応答と同様に、`HTTP 201 Created` 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。

新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/singlevaluelegacyextendedproperty_get.md)します。


****

##### <a name="request-2"></a>要求 2

2 番目の例では、指定した既存のメッセージに 1 つの単一値の拡張プロパティを作成します。拡張プロパティは、**singleValueExtendedProperties** 配列内の唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。
- **id** は、プロパティの型を `String` (GUID) として指定し、`Color` という名前のプロパティとして指定します。
- **value** は、`Color` プロパティの値として `Green` を指定します。

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a>応答 2

[メッセージの更新](../api/message_update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。

新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/singlevaluelegacyextendedproperty_get.md)します。

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

