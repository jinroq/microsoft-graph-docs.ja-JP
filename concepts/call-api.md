---
title: Microsoft Graph API を呼び出す
description: 'Microsoft Graph リソースにアクセスして操作するには、次の操作のいずれを使用して、リソース URL を呼び出し指定します。   '
ms.openlocfilehash: c8b678ce41488d6854e436e7dc5fc97989b54aee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092438"
---
# <a name="calling-the-microsoft-graph-api"></a><span data-ttu-id="2103a-103">Microsoft Graph API を呼び出す</span><span class="sxs-lookup"><span data-stu-id="2103a-103">Calling the Microsoft Graph API</span></span>

<span data-ttu-id="2103a-104">Microsoft Graph リソースにアクセスして操作するには、次の操作のいずれを使用して、リソース URL を呼び出し指定します。</span><span class="sxs-lookup"><span data-stu-id="2103a-104">To access and manipulate a Microsoft Graph resource, you call and specify the resource URLs using one of the following operations:</span></span>   

- <span data-ttu-id="2103a-105">GET</span><span class="sxs-lookup"><span data-stu-id="2103a-105">GET</span></span>
- <span data-ttu-id="2103a-106">POST</span><span class="sxs-lookup"><span data-stu-id="2103a-106">POST</span></span>
- <span data-ttu-id="2103a-107">PATCH</span><span class="sxs-lookup"><span data-stu-id="2103a-107">PATCH</span></span>
- <span data-ttu-id="2103a-108">PUT</span><span class="sxs-lookup"><span data-stu-id="2103a-108">PUT</span></span>
- <span data-ttu-id="2103a-109">DELETE</span><span class="sxs-lookup"><span data-stu-id="2103a-109">DELETE</span></span> 

<span data-ttu-id="2103a-110">Microsoft Graph API のすべての要求は、次の基本的な URL パターンを使用します。</span><span class="sxs-lookup"><span data-stu-id="2103a-110">All Microsoft Graph API requests use the following basic URL pattern:</span></span>

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

<span data-ttu-id="2103a-111">この URL で、</span><span class="sxs-lookup"><span data-stu-id="2103a-111">For this URL:</span></span>

- <span data-ttu-id="2103a-112">`https://graph.microsoft.com` は、Microsoft Graph API エンドポイントです。</span><span class="sxs-lookup"><span data-stu-id="2103a-112">`https://graph.microsoft.com` is the Microsoft Graph API endpoint.</span></span>
- <span data-ttu-id="2103a-113">`{version}` は、ターゲットのサービス バージョンです。たとえば、`v1.0` または `beta` です。</span><span class="sxs-lookup"><span data-stu-id="2103a-113">`{version}` is the target service version, for example, `v1.0` or `beta`.</span></span>
- <span data-ttu-id="2103a-114">`{resource}` は、以下のようなリソースのセグメントまたはパスです。</span><span class="sxs-lookup"><span data-stu-id="2103a-114">`{resource}` is resource segment or path, such as:</span></span>
  - <span data-ttu-id="2103a-115">`users`, `groups`, `devices`, `organization`</span><span class="sxs-lookup"><span data-stu-id="2103a-115"></span></span>
  - <span data-ttu-id="2103a-116">別名 `me`、サインインしているユーザーに解決されます</span><span class="sxs-lookup"><span data-stu-id="2103a-116">The alias `me`, which resolves to the signed-in user</span></span>
   - <span data-ttu-id="2103a-117">ユーザーに属するリソース (`me/events`、`me/drive`、`me/messages` など)</span><span class="sxs-lookup"><span data-stu-id="2103a-117">The resources belonging to a user, such as `me/events`, `me/drive` or `me/messages`</span></span>
  - <span data-ttu-id="2103a-118">別名 `myOrganization`、サインインしているユーザーの組織のテナントに解決されます</span><span class="sxs-lookup"><span data-stu-id="2103a-118">The alias `myOrganization`, which resolves to the tenant of the organization signed-in user</span></span>
- <span data-ttu-id="2103a-119">`[query_parameters]` は、追加のクエリ パラメーター (`$filter` や `$select` など) を表します。</span><span class="sxs-lookup"><span data-stu-id="2103a-119">`[query_parameters]` represents additional query parameters such as `$filter` and `$select`.</span></span>

<span data-ttu-id="2103a-p101">必要に応じて、テナントを要求の一部としても指定できます。`me` を使用する場合は、テナントを指定しません。一般的な要求の一覧については、「[Microsoft Graph の概要](overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2103a-p101">Optionally, you can also specify the tenant as part of your request. When using `me`, do not specify the tenant. For a list of common requests, see [Overview of Microsoft Graph](overview.md).</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="2103a-123">Microsoft Graph API メタデータ</span><span class="sxs-lookup"><span data-stu-id="2103a-123">Microsoft Graph API metadata</span></span>
<span data-ttu-id="2103a-p102">メタデータ ドキュメント ($metadata) が、サービス ルートに公開されます。たとえば、v1.0 およびベータ版のサービス ドキュメントは、次の URL で表示できます。</span><span class="sxs-lookup"><span data-stu-id="2103a-p102">The metadata document ($metadata) is published at the service root. For example, you can view the service document for the v1.0 and beta versions via the following URLs.</span></span>

<span data-ttu-id="2103a-126">Microsoft Graph API `v1.0` メタデータ。</span><span class="sxs-lookup"><span data-stu-id="2103a-126">Microsoft Graph API `v1.0` metadata.</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```
<span data-ttu-id="2103a-127">Microsoft Graph API `beta` メタデータ。</span><span class="sxs-lookup"><span data-stu-id="2103a-127">Microsoft Graph API `beta` metadata.</span></span>
```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="2103a-128">メタデータにより、Microsoft Graph が送受信する要求および応答パケットを構成するエンティティの種類およびセット、複合型、列挙型などの、Microsoft Graph のデータ モデルを参照し、理解することができます。</span><span class="sxs-lookup"><span data-stu-id="2103a-128">The metadata allows you to see and understand the data model of Microsoft Graph, including the entity types and sets, complex types, and enums that make up the request and response packets sent to and from Microsoft Graph.</span></span>
<span data-ttu-id="2103a-129">メタデータを使用して、Microsoft Graph のエンティティ間のリレーションシップを理解することができ、また、エンティティ間を移動する URL を確立することができます。</span><span class="sxs-lookup"><span data-stu-id="2103a-129">You can use the metadata to understand the realtionships between entities in Microsoft Graph and establish URLs that navigate between entities.</span></span>
<span data-ttu-id="2103a-130">このナビゲーション ベースの相互関連性は、Microsoft Graph 固有の特徴となっています。</span><span class="sxs-lookup"><span data-stu-id="2103a-130">This navigation-based interconnectedness gives Microsoft Graph its unique character.</span></span>

<span data-ttu-id="2103a-131">パス URL リソース名、クエリ パラメーター、アクション パラメーターと値は、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="2103a-131">Path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span> <span data-ttu-id="2103a-132">ただし、割り当てる値、エンティティ ID、その他の base64 でエンコードされた値では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="2103a-132">However, values you assign, entity IDs, and other base64-encoded values are case-sensitive.</span></span>

<span data-ttu-id="2103a-133">次のセクションでは、Microsoft Graph API を呼び出す基本的なプログラミング パターンをいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="2103a-133">The following sections show a few basic programming pattern calls to the Microsoft Graph API.</span></span>

## <a name="navigate-from-a-set-to-a-member"></a><span data-ttu-id="2103a-134">セットからメンバーへの移動</span><span class="sxs-lookup"><span data-stu-id="2103a-134">Navigate from a set to a member</span></span>

<span data-ttu-id="2103a-p105">ユーザーに関する情報を表示するには、HTTPS GET 要求を使用して、`users` コレクションから識別子によって識別される特定ユーザーの `User` エンティティを取得します。`User` エンティティでは、`id` プロパティと `userPrincipalName` プロパティのいずれかを識別子として使用できます。次の要求の例では、ユーザーの ID として `userPrincipalName` の値が使用されています。</span><span class="sxs-lookup"><span data-stu-id="2103a-p105">To view the information about a user, you get the `User` entity from the `users` collection to the specific user identified by its identifier, using an HTTPS GET request. For a `User` entity, either the `id` or `userPrincipalName` property can be used as the identifier. The following example request uses the `userPrincipalName` value as the user's id.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="2103a-138">成功した場合は、次のように、ペイロードにユーザー リソース表現を含む 200 OK 応答が返されるはずです。</span><span class="sxs-lookup"><span data-stu-id="2103a-138">If successful, you should get a 200 OK response containing the user resource representation in the payload, as shown as follows:</span></span>

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


## <a name="project-from-an-entity-to-properties"></a><span data-ttu-id="2103a-139">1 つのエンティティから複数のプロパティへのプロジェクション</span><span class="sxs-lookup"><span data-stu-id="2103a-139">Project from an entity to properties</span></span>
<span data-ttu-id="2103a-p106">ユーザーから提供された _About me_ の記述やスキル セットなどのユーザーの個人データのみを取得するには、以前の要求に _select_ クエリ パラメーターを追加することができます。たとえば、</span><span class="sxs-lookup"><span data-stu-id="2103a-p106">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the _select_ query parameter to the previous request. For example:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="2103a-142">成功した場合の応答は、200 OK 状態と次の形式のペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2103a-142">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="2103a-143">ここでは、`user` エンティティ上のプロパティ セット全体ではなく、`aboutMe` プロパティと `displayName` プロパティと `skills` プロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="2103a-143">Here, instead of the entire property sets on the `user` entity, only the `aboutMe`, `displayName`, and `skills` properties are returned.</span></span>

## <a name="traverse-to-another-resource-via-relationship"></a><span data-ttu-id="2103a-144">リレーションシップ経由の別のリソースへの走査</span><span class="sxs-lookup"><span data-stu-id="2103a-144">Traverse to another resource via relationship</span></span>
<span data-ttu-id="2103a-p107">上司は、直属の部下である他のユーザーとの `directReports` リレーションシップを保持します。ユーザーの直属の部下の一覧を問い合わせるために、次の HTTPS GET 要求を使用して、リレーションシップ走査経由で指定されたターゲットに移動できます。</span><span class="sxs-lookup"><span data-stu-id="2103a-p107">A manager holds a `directReports` relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="2103a-147">成功した場合の応答は、200 OK 状態と次の形式のペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2103a-147">The successful response returns the 200 OK status and a payload of the following format:</span></span>

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

<span data-ttu-id="2103a-p108">同様に、リレーションシップをフォローすると関連リソースに移動できます。たとえば、`user => messages` リレーションシップは、Azure AD ユーザーから Outlook メール メッセージのセットへのグラフ走査を可能にします。次の例は、REST API 呼び出しでこれを行う方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2103a-p108">Similarly, you can follow a relationship to navigate to related resources. For example, the `user => messages` relationship enables traversal from an Azure AD User to a set of Outlook mail messages. The following example shows how to do this in a REST API call:</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
<span data-ttu-id="2103a-151">成功した場合の応答は、200 OK 状態と次の形式のペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2103a-151">The successful response returns the 200 OK status and a payload of the following format:</span></span>


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

## <a name="project-from-entities-to-properties"></a><span data-ttu-id="2103a-152">複数のエンティティから複数のプロパティへのプロジェクション</span><span class="sxs-lookup"><span data-stu-id="2103a-152">Project from entities to properties</span></span>
<span data-ttu-id="2103a-p109">単一のエンティティからそのプロパティへのプロジェクションに加えて、同様の `select` クエリ オプションをエンティティ コレクションに適用して、それらのプロパティのいずれかのコレクションにプロジェクションさせることもできます。たとえば、サインインしているユーザーのドライブにある項目を問い合わせるには、次の HTTPS GET 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="2103a-p109">In addition to projection from a single entity to its properties, you can also apply the similar `select` query option to an entity collection to project them to a collection of some of their properties. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="2103a-155">成功した場合の応答は、次の例に示すように、200 OK 状態コードと、共有ファイルの名前と種類を含むペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2103a-155">The successful response returns a 200 OK status code and a payload containing the names and types of the shared files, as shown in the following example:</span></span>

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

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a><span data-ttu-id="2103a-156">フィルター処理クエリ オプションを使用してユーザーのサブセットを問い合わせる</span><span class="sxs-lookup"><span data-stu-id="2103a-156">Query a subset of users with the filtering query option</span></span>
<span data-ttu-id="2103a-p110">組織内の特定の役職の従業員を検索するには、ユーザー コレクションから移動してから、_filter_ クエリ オプションを指定することができます。次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="2103a-p110">To find the employees of a specific job title within an organization, you can navigate from the users collection and then specify a _filter_ query option. An example is shown as follows:</span></span>

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="2103a-159">成功した場合の応答は、次の例に示すように、200 OK 状態コードと指定された役職 (`'Helper'`) を持つユーザーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="2103a-159">The successful response returns the 200 OK status code and a list of users with the specified job title (`'Helper'`), as shown in the following example:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a><span data-ttu-id="2103a-160">アクションまたは関数を呼び出す</span><span class="sxs-lookup"><span data-stu-id="2103a-160">Call actions or functions</span></span>
<span data-ttu-id="2103a-161">Microsoft Graph は、_アクション_および_関数_もサポートし、標準の HTTP メソッドとは単純に一致しない方法でリソースを操作します。</span><span class="sxs-lookup"><span data-stu-id="2103a-161">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not a simple fit with standard HTTP methods.</span></span> <span data-ttu-id="2103a-162">たとえば、次の HTTPS POST 要求は、サインインしているユーザー (`me`) に電子メール メッセージを送信させます。</span><span class="sxs-lookup"><span data-stu-id="2103a-162">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>
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
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

<span data-ttu-id="2103a-163">要求ペイロードには、`sendMail` アクションへの入力が含まれています。これは、$metadata でも定義されています。</span><span class="sxs-lookup"><span data-stu-id="2103a-163">The request payload contains the input to the `sendMail` action, which is also defined in the $metadata.</span></span>

## <a name="use-microsoft-graph-client-libraries"></a><span data-ttu-id="2103a-164">Microsoft Graph クライアント ライブラリを使う</span><span class="sxs-lookup"><span data-stu-id="2103a-164">Use Microsoft Graph client libraries</span></span>
<span data-ttu-id="2103a-p112">SDK のパワーと使いやすさは気に入っていただけましたか?REST API を使用していつでも Microsoft Graph を呼び出すことができますが、多数の一般的なプラットフォームのための SDK も用意されています。</span><span class="sxs-lookup"><span data-stu-id="2103a-p112">Like the power and ease of SDKs? While you can always call Microsoft Graph using the REST API, we also provide SDKs for many popular platforms.</span></span>

<span data-ttu-id="2103a-167">当社の[サンプル コード、および Sdk](https://developer.microsoft.com/graph/code-samples-and-sdks)について説明します。</span><span class="sxs-lookup"><span data-stu-id="2103a-167">Explore our [code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>