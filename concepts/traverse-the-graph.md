---
title: Microsoft Graph のスキャン
description: Microsoft Graph API を使用してデータの読み取りと書き込みを行うだけでなく、多数の要求パターンを使用して Microsoft Graph のリソースをスキャンすることができます。また、メタデータ ドキュメントによって、リソースのデータ モデル、および Microsoft Graph 内のリレーションシップを理解することができます。
ms.openlocfilehash: 33f9ace57c7a0c3166e43a6ca1264174962752e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092389"
---
# <a name="traverse-microsoft-graph"></a>Microsoft Graph のスキャン

Microsoft Graph API を使用してデータの読み取りと書き込みを行うだけでなく、多数の要求パターンを使用して Microsoft Graph のリソースをスキャンすることができます。また、メタデータ ドキュメントによって、リソースのデータ モデル、および Microsoft Graph 内のリレーションシップを理解することができます。

## <a name="microsoft-graph-api-metadata"></a>Microsoft Graph API メタデータ

メタデータ ドキュメント ($metadata) が、サービス ルートに公開されます。Microsoft Graph API の v1.0 およびベータ版のサービス ドキュメントは、次の URL で表示できます。

**Microsoft Graph API v1.0 メタデータ**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Microsoft Graph API beta メタデータ**

```
    https://graph.microsoft.com/beta/$metadata
```

メタデータにより、要求および応答パケットが表すリソースを構成するエンティティの種類、複合型、列挙型を含む、Microsoft Graph のデータ モデルを参照し、理解することができます。

メタデータを使用して、Microsoft Graph のエンティティ間のリレーションシップを学ぶことができ、また、それらのエンティティ間を移動する URL を確立することができます。

パス URL リソース名、クエリ パラメーター、アクション パラメーターと値は、大文字と小文字が区別されません。ただし、割り当てる値、エンティティ ID、その他の base-64 でエンコードされた値は、大文字と小文字が区別されます。

## <a name="view-a-collection-of-resources"></a>リソースのコレクションを表示する

Microsoft Graph では、HTTP GET クエリを使用してテナント内のリソースを表示することができます。クエリの応答には各リソースのプロパティが含まれており、各リソースはその ID によって識別されます。リソース ID の形式は GUID にすることができ、一般に、リソースの種類によって異なります。 

たとえば、テナント内で定義されているユーザーのコレクションを取得できます。

```no-highlight 
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

成功した場合は、200 OK 応答が返され、そのペイロードに [user](/graph/api/resources/user?view=graph-rest-1.0) リソースのコレクションが含まれています。各ユーザーは **id** プロパティによって識別され、既定のプロパティが返されます。簡潔にするため、以下に示すペイロードは切り捨てられています。

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

Microsoft Graph を使用すると、1 つのリソースと別のリソース間のリレーションシップをナビゲートすることにより、コレクションを表示することもできます。たとえば、ユーザーの **mailFolders** ナビゲーション プロパティを通して、そのユーザーのメールボックス内の [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) リソースのコレクションに対してクエリを実行することができます。

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

成功した場合は、200 OK 応答が返され、そのペイロードに [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) リソースのコレクションが含まれています。各 **mailFolder** は **id** プロパティによって識別され、いくつかのプロパティも返されます。簡潔にするため、以下に示すペイロードは切り捨てられています。

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a>ID ごとにコレクションから特定のリソースを表示する

引き続き例として **user** を使用します。ユーザーに関する情報を表示するには、HTTPS GET 要求を使用してユーザーの ID から特定のユーザーを取得します。**user** エンティティでは、**id** プロパティまたは **userPrincipalName** プロパティのいずれかを識別子として使用できます。次の要求の例では、ユーザーの ID として **userPrincipalName** の値を使用しています。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

成功した場合は、200 OK 応答が返され、そのペイロードに、次に示すようなユーザー リソースの表現が含まれています。

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
ユーザーから提供された_自己紹介_の記述やスキル セットなどのユーザーの個人データのみを取得するには、次の例に示したように、以前の要求に [$select](query-parameters.md) クエリ パラメーターを追加することができます。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
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
ここでは、**user** エンティティのプロパティ セット全体ではなく、**aboutMe**、**displayName**、**skills** という基本的なプロパティのみが返されます。

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>コレクション内リソースの特定のプロパティの読み取り
1 つのリソースの特定のプロパティを読み取ることに加え、類似の [$select](query-parameters.md) クエリ パラメーターをコレクションに適用し、それぞれに返される特定のプロパティだけを使用してコレクション内のすべてのリソースを戻すことができます。たとえば、サインインしているユーザーのドライブにある項目の名前を問い合わせるには、次の HTTPS GET 要求を送信します。

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>リレーションシップ経由で 1 つのリソースから別のリソースへとスキャンする
上司は、直属の部下である他のユーザーとの **directReports** リレーションシップを保持します。ユーザーの直属の部下の一覧を問い合わせるために、次の HTTPS GET 要求を使用して、リレーションシップ走査経由で指定されたターゲットに移動できます。 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

成功した場合の応答は、200 OK 状態と、次に示すペイロードを返します。

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

同様に、リレーションシップをたどると、関連リソースに移動できます。たとえば、ユーザーとメッセージ間のリレーションシップにより、Azure Active Directory (Azure AD) ユーザーから Outlook メール メッセージのセットにスキャンできます。次の例は、REST API 呼び出しでこれを行う方法を示しています。


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
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
authorization: bearer {access_token}
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
        "@odata.type": "microsoft.graph.fileAttachment",
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

SDK のパワーと使いやすさは気に入っていただけましたか?常に REST API を使用して Microsoft Graph を呼び出すことができますが、多数の一般的なプラットフォームのための SDK も用意されています。利用可能な SDK を検索するには、「[コード サンプルと SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)」を参照してください。

## <a name="see-also"></a>関連項目

- [Microsoft Graph API を使用する](use-the-api.md)
- [認証トークンの取得](auth-overview.md)