# <a name="traverse-microsoft-graph"></a>Microsoft Graph のスキャン

Microsoft Graph API を使用してデータの読み取りと書き込みを行うだけでなく、多数の要求パターンを使用して Microsoft Graph のリソースをスキャンすることができます。また、メタデータ ドキュメントによって、リソースのデータ モデル、および Microsoft Graph 内のリレーションシップを理解することができます。

## <a name="microsoft-graph-api-metadata"></a>Microsoft Graph API メタデータ

メタデータ ドキュメント ($metadata) が、サービス ルートに公開されます。Microsoft Graph API の v1.0 およびベータ版のサービス ドキュメントは、次の URL で表示できます。

**Microsoft Graph API `v1.0` メタデータ**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Microsoft Graph API `beta` メタデータ**

```
    https://graph.microsoft.com/beta/$metadata
```

メタデータにより、エンティティの種類、複合型、要求および応答パケットが表すリソースを構成する列挙型を含む、Microsoft Graph のデータ モデルを参照し、理解することができます。

メタデータを使用して、Microsoft Graph のエンティティ間のリレーションシップを理解することができ、また、それらのエンティティ間を移動する URL を確立することができます。

パス URL リソース名、クエリ パラメーター、アクション パラメーターと値は、大文字と小文字が区別されません。ただし、割り当てる値、エンティティ ID、その他の base64 でエンコードされた値では大文字と小文字が区別されます。

## <a name="view-a-specific-resource-from-a-collection-by-id"></a>ID ごとにコレクションから特定のリソースを表示する

ユーザーに関する情報を表示するには、すべてのユーザーのコレクションを取得し HTTPS GET 要求を使用してユーザーの ID から特定のユーザーを取得します。`User` エンティティでは、`id` プロパティと `userPrincipalName` プロパティのいずれかを識別子として使用できます。次の要求の例では、ユーザーの ID として `userPrincipalName` の値が使用されています。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

成功した場合は、表示されているように、ペイロードにユーザー リソース表現を含む 200 OK 応答が返されます。

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```

## <a name="read-specific-properties-of-a-resource"></a>リソースの特定のプロパティの読み取り
ユーザーから提供された_自己紹介_の記述やスキル セットなどのユーザーの個人データのみを取得するには、次の例に示したように、以前の要求に [$select](query_parameters.md) クエリ パラメーターを追加することができます。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

表示のように、成功した場合の応答は 200 OK 状態とペイロードを返します。

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
ここでは、`user` エンティティ上のプロパティ セット全体ではなく、`aboutMe`、`displayName`、`skills` の基本プロパティのみが返されます。

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>コレクション内リソースの特定のプロパティの読み取り
1 つのリソースの特定のプロパティを読み取ることに加え、類似の [$select](query_parameters.md) クエリ パラメーターをコレクションに適用し、それぞれに返される特定のプロパティだけを使用してコレクション内のすべてのリソースを戻すことができます。たとえば、サインインしているユーザーのドライブにある項目の名前を問い合わせるには、次の HTTPS GET 要求を送信します。

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

成功した場合の応答は、次の例に示すように、200 OK 状態コードと、共有ファイルの名前のみを含むペイロードを返します。

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>リレーションシップ経由での、1 つのリソースから別のリソースへの走査
上司は、直属の部下である他のユーザーとの `directReports` リレーションシップを保持します。ユーザーの直属の部下の一覧を問い合わせるために、次の HTTPS GET 要求を使用して、リレーションシップ走査経由で指定されたターゲットに移動できます。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

表示のように、成功した場合の応答は 200 OK 状態とペイロードを返します。

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

同様に、リレーションシップをフォローすると関連リソースに移動できます。たとえば、`user => messages` リレーションシップは、Azure Active Directory (Azure AD) ユーザーから Outlook メール メッセージのセットへの走査を可能にします。次の例は、REST API 呼び出しでこれを行う方法を示しています。


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
表示のように、成功した場合の応答は 200 OK 状態とペイロードを返します。


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```
メタデータを参照し、EntityType を検索し、その EntityType のすべての NavigationProperties を探すことにより、指定されたリソースのすべてのリレーションシップを表示することができます。

## <a name="call-functions"></a>関数を呼び出す
Microsoft Graph は、単なる作成、読み取り、更新、削除 (CRUD) 操作ではない方法でリソースを操作するため、_関数_もサポートしています。関数の引数を入力するために HTTPS POST 要求の形を取ることがよくあります。たとえば、次の関数はサインインしているユーザー (`me`) に電子メール メッセージを送信させます。

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

メタデータで使用可能な、すべての関数を表示できます。それらは関数または操作として表示されます。

## <a name="use-the-microsoft-graph-sdks"></a>Microsoft Graph SDK を使用する

SDK のパワーと使いやすさは気に入っていただけましたか?常に REST API を使用して Microsoft Graph を呼び出すことができますが、多数の一般的なプラットフォームのための SDK も用意されています。利用可能な SDK を検索するには、「[コード サンプルと SDK](https://graph.microsoft.io/en-us/code-samples-and-sdks)」を参照してください。

## <a name="see-also"></a>関連項目

- [Microsoft Graph API を使用する](use_the_api.md)
- [認証トークンの取得](auth_overview.md)