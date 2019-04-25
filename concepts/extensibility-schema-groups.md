---
title: 'スキーマ拡張機能を使用したグループへのカスタム データの追加 '
description: '*スキーマ拡張機能*の使用方法について、具体例を使って説明します。 '
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: c1241133dff25769d7dc140fc086ab286093ab04
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526102"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a><span data-ttu-id="daa64-103">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="daa64-103">Add custom data to groups using schema extensions</span></span> 

<span data-ttu-id="daa64-104">*スキーマ拡張機能*の使用方法について、具体例を使って説明します。</span><span class="sxs-lookup"><span data-stu-id="daa64-104">We're going to walk you through an example to demonstrate how to use *schema extensions*.</span></span> 

<span data-ttu-id="daa64-p101">ここでは、企業向けトレーニングのコースや教材を製作する “Graph Learn” という名前の学習管理ソフトウェア会社で開発者として働いているとしましょう。充実した共同エクスペリエンスを備えた Office 365 グループは、オンライン コースの参加者および講師が指導するコースの参加者どちらに対しても、コース コンテンツを配信したりエクササイズの記録をとったりするのに最適なツールです。トレーニング コースのために使う Office 365 グループを、トレーニング コースとしてすぐに見分けがつくようにしておくと、他の開発者がグループを見つけやすくなり、学習コースに基づいて豊富なエクスペリエンスを構築するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="daa64-p101">Imagine you're a developer in a Learning Management Software company called “Graph Learn” that builds training courses and materials for businesses.  Office 365 groups, with their rich collaborative experiences, is a fantastic way to deliver course content and record exercises among participants for both online courses and instructor-led courses.  You may want to make those Office 365 groups used for training courses easily identifiable as training courses, which will allow other developers to discover your groups and build rich experiences on top of your learning courses.</span></span>

<span data-ttu-id="daa64-108">このシナリオでは、以下の操作を行う方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="daa64-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="daa64-109">利用可能なスキーマ拡張機能の定義を確認する</span><span class="sxs-lookup"><span data-stu-id="daa64-109">View available schema extension definitions that you could use.</span></span>
2. <span data-ttu-id="daa64-110">トレーニング コースの対象グループに適用されるスキーマ拡張機能の定義を登録する</span><span class="sxs-lookup"><span data-stu-id="daa64-110">Register a schema extension definition that targets groups for training courses.</span></span>
3. <span data-ttu-id="daa64-111">登録したスキーマ拡張機能の定義に基づいた拡張データで新しいグループを作成する</span><span class="sxs-lookup"><span data-stu-id="daa64-111">Create a new group with extended data based on the schema extension definition that you just registered.</span></span>
4. <span data-ttu-id="daa64-112">スキーマ拡張機能の定義に基づいて既存のグループのカスタム データを追加、更新または削除する</span><span class="sxs-lookup"><span data-stu-id="daa64-112">Add, update, or remove custom data in an existing group based on a schema extension definition.</span></span>
5. <span data-ttu-id="daa64-113">グループと拡張機能データを読み取る</span><span class="sxs-lookup"><span data-stu-id="daa64-113">Read back a group and the extension data.</span></span>

><span data-ttu-id="daa64-p102">**注:** このトピックでは、**グループ** リソースでスキーマ拡張機能の値を作成し、読み取る方法について説明します (手順 3 から 5)。同じメソッドは、\*\* administrativeUnit**、**デバイス**、**イベント**、**メッセージ**、**組織**、**投稿\*\*、および **ユーザー** リソースの種類でもサポートされています。このため、これらのリソースのいずれかで、下にある要求例と同様の操作を実行できます。注: **administrativeUnit** はベータ版エンドポイントでのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="daa64-p102">**Note:** This topic shows you how to create and read schema extension values on a **group** resource (steps 3-5).  The same methods are supported for the **administrativeUnit**, **device**, **event**, **message**, **organization**, **post**, and **user** resource types as well.  So you can carry out similar operations as the example requests below on any of those resources. Note that **administrativeUnit** is available only in the beta endpoint.</span></span>

## <a name="1-view-available-schema-extensions"></a><span data-ttu-id="daa64-118">1.利用可能なスキーマ拡張機能を確認する</span><span class="sxs-lookup"><span data-stu-id="daa64-118">1. View available schema extensions</span></span>
<span data-ttu-id="daa64-p103">開発者は、まずアプリで再利用できるスキーマ拡張機能の定義が他にないか調べる必要があります。これは **schemaExtension** リソースをクエリすることによって可能です。</span><span class="sxs-lookup"><span data-stu-id="daa64-p103">First, as a developer, you might want to find any other schema extension definitions that our app could reuse.  This can be done by querying the **schemaExtension** resource.</span></span>  
<span data-ttu-id="daa64-121">次の例では、特定のスキーマ拡張機能を **id** でクエリします。</span><span class="sxs-lookup"><span data-stu-id="daa64-121">In the example below, you're going to query for a specific schema extension by **id**.</span></span>

<span data-ttu-id="daa64-p104">応答で返される拡張機能の**状態**値は **Available** であることに注意してください。これは、**targetTypes** プロパティのリソースへのアクセス許可を持つ任意のアプリが、拡張機能を使用でき、付加的な変更で拡張機能を更新できることを示しています。通常、この操作では、**状態**にかかわらず、指定されたフィルターに一致するすべてのスキーマ拡張機能が返されるため、使用する前に拡張機能の状態を必ず確認してください。</span><span class="sxs-lookup"><span data-stu-id="daa64-p104">Notice that the extension returned in the response has **Available** as the **status** value, which indicates that any app which has permission to the resources in the **targetTypes** property can use and update the extension with additive changes. In general, this operation returns any schema extensions that satisfy the specified filter regardless of **status**, so do check the extension status before using it.</span></span>


##### <a name="request"></a><span data-ttu-id="daa64-124">要求</span><span class="sxs-lookup"><span data-stu-id="daa64-124">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="daa64-125">応答</span><span class="sxs-lookup"><span data-stu-id="daa64-125">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a><span data-ttu-id="daa64-126">2.トレーニング コースについて説明するスキーマ拡張機能の定義を登録する</span><span class="sxs-lookup"><span data-stu-id="daa64-126">2. Register a schema extension definition that describes a training course</span></span>
<span data-ttu-id="daa64-127">ニーズに*適した*スキーマ拡張機能が見つからない場合は、**グループ** リソースでトレーニング コースの新しい拡張機能の定義を作成し登録します。</span><span class="sxs-lookup"><span data-stu-id="daa64-127">If you can't find a schema extension that *is* appropriate for your needs, you can create and register a new extension definition for training courses on the **group** resource.</span></span>  

<span data-ttu-id="daa64-p105">スキーマ拡張機能定義を作成する場合、**id** プロパティに文字列を指定する必要があります。これを実行するには、次の 2 つの方法があります。次の例は優先される方法を示しています。この方法では、ご使用のテナントで検証済みのバニティ ドメイン名 (`graphlearn.com`) を使用します。検証済みドメイン名 (`graphlearn`) とスキーマ拡張機能名 (`courses`) を連結し、連結後の文字列 `graphlearn_courses` を使用して **ID** を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="daa64-p105">When creating a schema extension definition, you should provide a string for the **id** property. There are two ways to do this. The following example shows the preferred way, which uses a vanity domain name (`graphlearn.com`) that has been verified with your tenant. Concatenate the verified domain name (`graphlearn`) with a name for the schema extension (`courses`), and assign **id** with the resultant string, `graphlearn_courses`.</span></span>  

<span data-ttu-id="daa64-p106">説明 (見つけやすくするため)、(この拡張機能が適用されるリソースを定義する) 対象の種類、およびスキーマを構成するカスタム プロパティも指定します。この例の場合、`courseId`、`courseName`、`courseType` のカスタム プロパティとその種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="daa64-p106">Then, specify a description (to enable discoverability), target types (defining which resources this extension applies to), and the custom properties that make up the schema.  In this example, specify the `courseId`, `courseName` and `courseType` custom properties and their types.</span></span>

<span data-ttu-id="daa64-134">[要求で **ID** を割り当てる他の方法の例](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2)を参照してください。この例で必要となるのは、スキーマ名の指定のみです。</span><span class="sxs-lookup"><span data-stu-id="daa64-134">See an [example of the other way to assign **id** in the request](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2), that requires you to provide only a schema name.</span></span>

<span data-ttu-id="daa64-p107">スキーマ拡張機能を最初に作成するとき、その状態は **InDevelopment** であることに注意してください。拡張機能の開発中は、この状態を保持できます。その間、拡張機能を付加的な変更で更新したり、削除したりできるのは拡張機能を作成したアプリだけです。他のアプリで使用するために拡張機能を共有する準備ができたら、**status** を **Available** に設定します。</span><span class="sxs-lookup"><span data-stu-id="daa64-p107">Notice that when you initially create a schema extension, its status is **InDevelopment**. While you're developing the extension, you can keep it in this status, during which only your app that created it can update it with additive changes or delete it. When you are ready to share the extension for use by other apps, set **status** to **Available**.</span></span>

##### <a name="request"></a><span data-ttu-id="daa64-138">要求</span><span class="sxs-lookup"><span data-stu-id="daa64-138">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json
{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="daa64-139">応答</span><span class="sxs-lookup"><span data-stu-id="daa64-139">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="3-create-a-new-group-with-extended-data"></a><span data-ttu-id="daa64-140">3.拡張データを含む新しいグループを作成する</span><span class="sxs-lookup"><span data-stu-id="daa64-140">3. Create a new group with extended data</span></span> 
<span data-ttu-id="daa64-p108">_新しい_グループを作成し、登録したばかりの `graphlearn_courses` スキーマ拡張機能定義を使って、追加のデータでグループを拡張します。これは、**グループ** リソースへの標準的な ```POST``` と、要求本文で定義された追加の `graphlearn_courses` の複合型の拡張機能です。応答では、データ拡張機能を返しません。```GET``` 操作を使用して、名前により拡張機能を明示的に ```$select``` する必要があります。</span><span class="sxs-lookup"><span data-stu-id="daa64-p108">Create a _new_ group and extend it with extra data using the `graphlearn_courses` schema extension definition that we just registered.  This is a standard ```POST``` to the **group** resource, with the additional `graphlearn_courses` complex type extension defined in the request body.  The response will not mirror back any data extensions. We need to explicitly ```$select``` the extension by name using a ```GET``` operation.</span></span>

##### <a name="request"></a><span data-ttu-id="daa64-145">要求</span><span class="sxs-lookup"><span data-stu-id="daa64-145">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a><span data-ttu-id="daa64-146">応答</span><span class="sxs-lookup"><span data-stu-id="daa64-146">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a><span data-ttu-id="daa64-147">4.既存のグループのカスタム データを追加、更新、または削除します。</span><span class="sxs-lookup"><span data-stu-id="daa64-147">4. Add, update, or remove custom data in an existing group</span></span>
<span data-ttu-id="daa64-148">```PATCH``` 要求の本文で定義した追加の `graphlearn_courses` の複合型の拡張機能を使って、カスタム データを拡張し、_既存_のグループ インスタンスに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="daa64-148">You can extend and add custom data to an _existing_ group instance with the additional `graphlearn_courses` complex type extension defined in the body of a ```PATCH``` request.</span></span>  

##### <a name="request"></a><span data-ttu-id="daa64-149">要求</span><span class="sxs-lookup"><span data-stu-id="daa64-149">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a><span data-ttu-id="daa64-150">応答</span><span class="sxs-lookup"><span data-stu-id="daa64-150">Response</span></span>
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="daa64-151">拡張機能データの値を更新する場合は、複合型拡張機能の全体を ```PATCH``` 要求の本文に置きます (既存のリソースにカスタム データを追加するのと同様)。</span><span class="sxs-lookup"><span data-stu-id="daa64-151">If you want to update the values of the extension data, put the entire extension complex type in the body of a ```PATCH``` request (similar to adding custom data to an existing resource).</span></span>

<span data-ttu-id="daa64-152">対応する拡張機能のプロパティを Null に設定することで、リソース インスタンスに追加されたカスタム データを削除できます。</span><span class="sxs-lookup"><span data-stu-id="daa64-152">You can also remove custom data added to a resource instance by setting the corresponding extension property to null.</span></span> 

<span data-ttu-id="daa64-153">リソース インスタンスからスキーマ拡張機能を削除する場合、当該インスタンスの複合型拡張機能を Null に設定します。</span><span class="sxs-lookup"><span data-stu-id="daa64-153">To remove a schema extension from a resource instance, set the extension complex type in that instance to null.</span></span>


## <a name="5-get-a-group-and-its-extension-data"></a><span data-ttu-id="daa64-154">5.グループとその拡張機能データを取得する</span><span class="sxs-lookup"><span data-stu-id="daa64-154">5. Get a group and its extension data</span></span>
<span data-ttu-id="daa64-155">拡張機能の名前や ID など特定の拡張機能のプロパティ値に一致する `$filter` を使用すると簡単にグループ (または複数のグループ) を検索できます。</span><span class="sxs-lookup"><span data-stu-id="daa64-155">A handy way to look for a group (or groups) is to use `$filter` to match for specific extension property values, such as an extension name or ID.</span></span> 

<span data-ttu-id="daa64-156">次に、`$select` を使って、拡張機能の名前を指定し (この場合は `graphlearn_courses`)、グループのカスタムデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="daa64-156">Then, to get the custom data in a group, use `$select` to include the extension by name (in this case by `graphlearn_courses`).</span></span>

<span data-ttu-id="daa64-p109">次の例では、`graphlearn_courses` の拡張機能と `123` に一致する `courseId` のプロパティ値を有するグループを検索し、`graphlearn_courses` 拡張機能のグループのプロパティ、**displayName**、**ID**、**説明**、カスタム データを取得します。(実際のクエリでは、必要に応じて URL エンコードを行ってください。)</span><span class="sxs-lookup"><span data-stu-id="daa64-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

#### <a name="request"></a><span data-ttu-id="daa64-159">要求</span><span class="sxs-lookup"><span data-stu-id="daa64-159">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a><span data-ttu-id="daa64-160">応答</span><span class="sxs-lookup"><span data-stu-id="daa64-160">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="daa64-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="daa64-161">See also</span></span>

- [<span data-ttu-id="daa64-162">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="daa64-162">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="daa64-163">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="daa64-163">Add custom data to users using open extensions (preview)</span></span>](extensibility-open-users.md)
- [<span data-ttu-id="daa64-164">Office 365 のドメイン</span><span class="sxs-lookup"><span data-stu-id="daa64-164">Office 365 domains</span></span>](https://technet.microsoft.com/ja-JP/library/office-365-domains.aspx)
- [<span data-ttu-id="daa64-165">新しい Office 365 のドメインの追加および検証</span><span class="sxs-lookup"><span data-stu-id="daa64-165">Adding and Verifying a Domain for the NEW Office 365</span></span>](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="daa64-166">schemaExtension リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="daa64-166">schemaExtension resource type</span></span>](/graph/api/resources/schemaextension?view=graph-rest-1.0)
- [<span data-ttu-id="daa64-167">schemaExtensions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="daa64-167">List schemaExtensions</span></span>](/graph/api/schemaextension-list?view=graph-rest-1.0)
- [<span data-ttu-id="daa64-168">schemaExtension を作成する</span><span class="sxs-lookup"><span data-stu-id="daa64-168">Create schemaExtension</span></span>](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0)
- [<span data-ttu-id="daa64-169">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="daa64-169">Get schemaExtension</span></span>](/graph/api/schemaextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="daa64-170">schemaExtension を更新する</span><span class="sxs-lookup"><span data-stu-id="daa64-170">Update schemaExtension</span></span>](/graph/api/schemaextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="daa64-171">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="daa64-171">Delete schemaExtension</span></span>](/graph/api/schemaextension-delete?view=graph-rest-1.0)
