---
title: Microsoft Graph 内を移動してデータとメソッドにアクセスする
description: Microsoft Graph API を使用してデータの読み取りと書き込みを行うだけでなく、多数の要求パターンを使用して Microsoft Graph のリソースをスキャンすることができます。また、メタデータ ドキュメントによって、リソースのデータ モデル、および Microsoft Graph 内のリレーションシップを理解することができます。
localization_priority: Priority
ms.openlocfilehash: 2b02ca0ed623fa17d9b640ff0bb1c17c3b3e022e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840650"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a><span data-ttu-id="2c3e9-104">Microsoft Graph 内を移動してデータとメソッドにアクセスする</span><span class="sxs-lookup"><span data-stu-id="2c3e9-104">Access data and methods by navigating Microsoft Graph</span></span>

<span data-ttu-id="2c3e9-p102">Microsoft Graph API を使用してデータの読み取りと書き込みを行うだけでなく、多数の要求パターンを使用して Microsoft Graph のリソースをスキャンすることができます。また、メタデータ ドキュメントによって、リソースのデータ モデル、および Microsoft Graph 内のリレーションシップを理解することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p102">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="2c3e9-107">Microsoft Graph API メタデータ</span><span class="sxs-lookup"><span data-stu-id="2c3e9-107">Microsoft Graph API metadata</span></span>

<span data-ttu-id="2c3e9-p103">メタデータ ドキュメント ($metadata) が、サービス ルートに公開されます。Microsoft Graph API の v1.0 およびベータ版のサービス ドキュメントは、次の URL で表示できます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p103">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="2c3e9-110">**Microsoft Graph API v1.0 メタデータ**</span><span class="sxs-lookup"><span data-stu-id="2c3e9-110">**Microsoft Graph API v1.0 metadata**</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="2c3e9-111">**Microsoft Graph API beta メタデータ**</span><span class="sxs-lookup"><span data-stu-id="2c3e9-111">**Microsoft Graph API beta metadata**</span></span>

```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="2c3e9-112">メタデータにより、要求および応答パケットが表すリソースを構成するエンティティの種類、複合型、列挙型を含む、Microsoft Graph のデータ モデルを参照し、理解することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-112">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span>

<span data-ttu-id="2c3e9-113">メタデータを使用して、Microsoft Graph のエンティティ間のリレーションシップを学ぶことができ、また、それらのエンティティ間を移動する URL を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-113">You can use the metadata to learn the realtionships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

> [!NOTE]
> - <span data-ttu-id="2c3e9-114">リソース ID の大文字と小文字の区別 は、Microsoft Graph API から返されたものと同じものを使用します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-114">Use resource IDs in the same case as they are returned from Microsoft Graph APIs.</span></span>
> - <span data-ttu-id="2c3e9-115">リソース ID、ユーザーが割り当てる値、およびその他の base-64 でエンコードされた値は、_大文字と小文字が区別される_ものと考えてください。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-115">Assume resource IDs, values you assign, and other base-64-encoded values are _case-sensitive_.</span></span>
> - <span data-ttu-id="2c3e9-116">パス URL リソース名、クエリ パラメーター、アクション パラメーターと値は、_大文字と小文字は区別されない_ものと考えてください。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-116">The path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="2c3e9-117">リソースのコレクションを表示する</span><span class="sxs-lookup"><span data-stu-id="2c3e9-117">View a collection of resources</span></span>

<span data-ttu-id="2c3e9-118">Microsoft Graph では、HTTP `GET` クエリを使用してテナント内のリソースを表示することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-118">Microsoft Graph lets you view resources in a tenant using HTTP `GET` queries.</span></span> <span data-ttu-id="2c3e9-119">クエリの応答には、各リソースのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-119">The query response includes properties of each resource.</span></span> <span data-ttu-id="2c3e9-120">各エンティティ リソースはそれぞれの ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-120">Entity resources are each identified by its ID.</span></span> <span data-ttu-id="2c3e9-121">リソース ID の形式は GUID にすることができ、一般に、リソースの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-121">The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span>

<span data-ttu-id="2c3e9-122">たとえば、テナント内で定義されている [user](/graph/api/resources/user?view=graph-rest-1.0) リソースのコレクションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-122">For example, you can get the collection of users defined in a tenant:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-p105">成功した場合は、200 OK 応答が返され、そのペイロードに **user** リソースのコレクションが含まれています。各ユーザーは **id** プロパティによって識別され、既定のプロパティが返されます。簡潔にするため、以下に示すペイロードは切り捨てられています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p105">If successful, you'll get a 200 OK response that contains the collection of **user** resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

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

<span data-ttu-id="2c3e9-p106">Microsoft Graph を使用すると、1 つのリソースと別のリソース間のリレーションシップをナビゲートすることにより、コレクションを表示することもできます。たとえば、ユーザーの **mailFolders** ナビゲーション プロパティを通して、そのユーザーのメールボックス内の [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) リソースのコレクションに対してクエリを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p106">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resources in the user's mailbox:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-p107">成功した場合は、200 OK 応答が返され、そのペイロードに [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) リソースのコレクションが含まれています。各 **mailFolder** は **id** プロパティによって識別され、いくつかのプロパティも返されます。簡潔にするため、以下に示すペイロードは切り捨てられています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p107">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

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




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="2c3e9-131">ID ごとにコレクションから特定のリソースを表示する</span><span class="sxs-lookup"><span data-stu-id="2c3e9-131">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="2c3e9-132">引き続き例として **user** を使用します。ユーザーに関する情報を表示するには、HTTPS GET 要求を使用してユーザーの ID から特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-132">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a user entity, you can use either the id or userPrincipalName property as the identifier. The following request example uses the userPrincipalName value as the user's ID.</span></span> <span data-ttu-id="2c3e9-133">**user** エンティティでは、**id** プロパティまたは **userPrincipalName** プロパティのいずれかを識別子として使用できます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-133">For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier.</span></span>

<span data-ttu-id="2c3e9-134">次の要求の例では、ユーザーの ID として **userPrincipalName** の値を使用しています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-134">The following example request uses the \*\*\*\* value as the user's id.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-135">成功した場合は、200 OK 応答が返され、そのペイロードに、次に示すようなユーザー リソースの表現が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-135">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

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

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="2c3e9-136">リソースの特定のプロパティの読み取り</span><span class="sxs-lookup"><span data-stu-id="2c3e9-136">Read specific properties of a resource</span></span>
<span data-ttu-id="2c3e9-137">ユーザーから提供された_自己紹介_の記述やスキル セットなどのユーザーの個人データのみを取得するには、次の例に示したように、以前の要求に [$select](query-parameters.md) クエリ パラメーターを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-137">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query-parameters.md) query parameter to the previous request, as shown in the following example.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-138">成功した場合の応答は、200 OK 状態と、次に示すペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-138">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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
<span data-ttu-id="2c3e9-139">ここでは、**user** エンティティのプロパティ セット全体ではなく、**aboutMe**、**displayName**、**skills** という基本的なプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-139">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="2c3e9-140">コレクション内リソースの特定のプロパティの読み取り</span><span class="sxs-lookup"><span data-stu-id="2c3e9-140">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="2c3e9-141">1 つのリソースの特定のプロパティを読み取ることに加え、類似の [$select](query-parameters.md) クエリ パラメーターをコレクションに適用し、それぞれに返される特定のプロパティだけを使用してコレクション内のすべてのリソースを戻すことができます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-141">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query-parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

<span data-ttu-id="2c3e9-142">たとえば、サインインしているユーザーのドライブにある項目の名前を問い合わせるには、次の HTTPS GET 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-142">For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-143">成功した場合の応答は、次の例に示すように、200 OK 状態コードと、共有ファイルの名前のみを含むペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-143">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="2c3e9-144">リレーションシップ経由で 1 つのリソースから別のリソースへとスキャンする</span><span class="sxs-lookup"><span data-stu-id="2c3e9-144">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="2c3e9-p109">上司は、直属の部下である他のユーザーとの **directReports** リレーションシップを保持します。ユーザーの直属の部下の一覧を問い合わせるために、次の HTTPS GET 要求を使用して、リレーションシップ走査経由で指定されたターゲットに移動できます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p109">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="2c3e9-147">表示のように、成功した場合の応答は 200 OK 状態とペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-147">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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

<span data-ttu-id="2c3e9-p110">同様に、リレーションシップをたどると、関連リソースに移動できます。たとえば、ユーザーとメッセージ間のリレーションシップにより、Azure Active Directory (Azure AD) ユーザーから Outlook メール メッセージのセットにスキャンできます。次の例は、REST API 呼び出しでこれを行う方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p110">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```no-highlight
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


<span data-ttu-id="2c3e9-151">表示のように、成功した場合の応答は 200 OK 状態とペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-151">The successful response returns the 200 OK status and a payload, as shown.</span></span>


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
<span data-ttu-id="2c3e9-152">メタデータを参照し、`EntityType` を検索し、その `NavigationProperty` のすべての `EntityType` を確認することにより、特定のリソースのすべてのリレーションシップを確認できます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-152">You can see all the relationships on a given resource by going to the metadata, finding the EntityType, and looking at all NavigationProperties for that EntityType.</span></span>

## <a name="call-actions-and-functions"></a><span data-ttu-id="2c3e9-153">呼び出しのアクションと関数</span><span class="sxs-lookup"><span data-stu-id="2c3e9-153">Call actions or functions</span></span>
<span data-ttu-id="2c3e9-154">Microsoft Graph は、単なる作成、読み取り、更新、削除 (CRUD) 操作ではない方法でリソースを操作するための_アクション_と_関数_もサポートしています。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-154">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations.</span></span> <span data-ttu-id="2c3e9-155">アクションまたは関数の引数を入力するために HTTPS POST 要求の形を取ることがよくあります。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-155">They are often in the shape of HTTPS POST requests in order to intake arguments for the action or function.</span></span> <span data-ttu-id="2c3e9-156">たとえば、次のアクションはサインインしているユーザー (`me`) に電子メール メッセージを送信させます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-156">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>

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
          "address": "garthf@contoso.onmicrosoft.com"
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

<span data-ttu-id="2c3e9-p112">メタデータで使用可能な、すべての関数を表示できます。それらは関数または操作として表示されます。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p112">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="2c3e9-159">Microsoft Graph SDK を使用する</span><span class="sxs-lookup"><span data-stu-id="2c3e9-159">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="2c3e9-p113">SDK のパワーと使いやすさは気に入っていただけましたか?常に REST API を使用して Microsoft Graph を呼び出すことができますが、多数の一般的なプラットフォームのための SDK も用意されています。利用可能な SDK を検索するには、「[コード サンプルと SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c3e9-p113">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="2c3e9-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c3e9-163">See also</span></span>

- [<span data-ttu-id="2c3e9-164">Microsoft Graph API を使用する</span><span class="sxs-lookup"><span data-stu-id="2c3e9-164">Use the Microsoft Graph API</span></span>](use-the-api.md)
- [<span data-ttu-id="2c3e9-165">認証トークンの取得</span><span class="sxs-lookup"><span data-stu-id="2c3e9-165">Get auth tokens</span></span>](/graph/auth)
