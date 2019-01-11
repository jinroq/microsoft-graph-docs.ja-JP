---
title: ユーザーを一覧表示する
description: Person オブジェクトのユーザーの通信とコラボレーションのパターンとビジネスの関係によって決定されると、ユーザーに関連性の順のリストを取得します。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 3bd9c8cdd3737cbd8d96fd4f9b24f5382ce04793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872780"
---
# <a name="list-people"></a><span data-ttu-id="f89f8-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f89f8-103">List people</span></span>

> <span data-ttu-id="f89f8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f89f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f89f8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f89f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f89f8-106">[Person](../resources/person.md)オブジェクトの順に、[ユーザー](../resources/user.md)ユーザーの通信とコラボレーションのパターンとビジネスの関係によって決定される関連性についての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-106">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="f89f8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f89f8-107">Permissions</span></span>

<span data-ttu-id="f89f8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f89f8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f89f8-110">Permission type</span></span>      | <span data-ttu-id="f89f8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f89f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f89f8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f89f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f89f8-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="f89f8-113">People.Read</span></span>    |
|<span data-ttu-id="f89f8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f89f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f89f8-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="f89f8-115">People.Read</span></span>    |
|<span data-ttu-id="f89f8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f89f8-116">Application</span></span> | <span data-ttu-id="f89f8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f89f8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f89f8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f89f8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f89f8-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f89f8-119">Optional query parameters</span></span>

<span data-ttu-id="f89f8-120">このメソッドは、応答をカスタマイズするためには、次の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f89f8-120">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="f89f8-121">名前</span><span class="sxs-lookup"><span data-stu-id="f89f8-121">Name</span></span>|<span data-ttu-id="f89f8-122">値</span><span class="sxs-lookup"><span data-stu-id="f89f8-122">Value</span></span>|<span data-ttu-id="f89f8-123">説明</span><span class="sxs-lookup"><span data-stu-id="f89f8-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="f89f8-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f89f8-124">$filter</span></span>|<span data-ttu-id="f89f8-125">文字列</span><span class="sxs-lookup"><span data-stu-id="f89f8-125">string</span></span>|<span data-ttu-id="f89f8-126">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="f89f8-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="f89f8-127">$orderby</span></span>|<span data-ttu-id="f89f8-128">文字列</span><span class="sxs-lookup"><span data-stu-id="f89f8-128">string</span></span>|<span data-ttu-id="f89f8-129">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="f89f8-130">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f89f8-131">$search</span><span class="sxs-lookup"><span data-stu-id="f89f8-131">$search</span></span>|<span data-ttu-id="f89f8-132">文字列</span><span class="sxs-lookup"><span data-stu-id="f89f8-132">string</span></span>|<span data-ttu-id="f89f8-133">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-133">Search for people by name or alias.</span></span> <span data-ttu-id="f89f8-134">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f89f8-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="f89f8-135">パラメーターだけが、他のユーザーに関連する人の検索ではなく、サインインしているユーザーの関連するユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="f89f8-136">サポートしており、`topic`その人と電子メールのやり取りなどから抽出された項目に基づいて、ユーザーを検索するキーワードです。</span><span class="sxs-lookup"><span data-stu-id="f89f8-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="f89f8-137">例については、[人の関連情報を取得](/graph/people-example#perform-a-fuzzy-search)することで*あいまい検索を実行する*セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="f89f8-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="f89f8-138">$select</span><span class="sxs-lookup"><span data-stu-id="f89f8-138">$select</span></span>|<span data-ttu-id="f89f8-139">文字列</span><span class="sxs-lookup"><span data-stu-id="f89f8-139">string</span></span>|<span data-ttu-id="f89f8-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="f89f8-142">$skip</span><span class="sxs-lookup"><span data-stu-id="f89f8-142">$skip</span></span>|<span data-ttu-id="f89f8-143">int</span><span class="sxs-lookup"><span data-stu-id="f89f8-143">int</span></span>|<span data-ttu-id="f89f8-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="f89f8-146">$top</span><span class="sxs-lookup"><span data-stu-id="f89f8-146">$top</span></span>|<span data-ttu-id="f89f8-147">int</span><span class="sxs-lookup"><span data-stu-id="f89f8-147">int</span></span>|<span data-ttu-id="f89f8-148">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="f89f8-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f89f8-149">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f89f8-149">Request headers</span></span>

| <span data-ttu-id="f89f8-150">名前</span><span class="sxs-lookup"><span data-stu-id="f89f8-150">Name</span></span>      |<span data-ttu-id="f89f8-151">説明</span><span class="sxs-lookup"><span data-stu-id="f89f8-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f89f8-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="f89f8-152">Authorization</span></span>  | <span data-ttu-id="f89f8-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f89f8-155">承諾</span><span class="sxs-lookup"><span data-stu-id="f89f8-155">Accept</span></span> | <span data-ttu-id="f89f8-156">application/json</span><span class="sxs-lookup"><span data-stu-id="f89f8-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f89f8-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="f89f8-157">Request body</span></span>

<span data-ttu-id="f89f8-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f89f8-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f89f8-159">応答</span><span class="sxs-lookup"><span data-stu-id="f89f8-159">Response</span></span>

<span data-ttu-id="f89f8-160">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[ユーザー](../resources/person.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f89f8-160">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f89f8-161">例</span><span class="sxs-lookup"><span data-stu-id="f89f8-161">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="f89f8-162">参照</span><span class="sxs-lookup"><span data-stu-id="f89f8-162">Browse</span></span>

<span data-ttu-id="f89f8-163">このセクションで要求がサインインしているユーザーに最も関連する人を取得 (`/me`)、通信、コラボレーション、および取引関係に基づく。</span><span class="sxs-lookup"><span data-stu-id="f89f8-163">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="f89f8-164">既定では、応答ごとに 10 件のレコードが返されます。ただし、$top パラメーターを使用することで、*これを変更*できます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-164">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="f89f8-165">これらの要求には、People.Read アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f89f8-165">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="f89f8-166">要求</span><span class="sxs-lookup"><span data-stu-id="f89f8-166">Request</span></span>

<span data-ttu-id="f89f8-167">次に、既定の要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-167">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="f89f8-168">応答</span><span class="sxs-lookup"><span data-stu-id="f89f8-168">Response</span></span>

<span data-ttu-id="f89f8-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-169">The following is an example of the response.</span></span>
><span data-ttu-id="f89f8-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="f89f8-172">人物の続きのページの要求</span><span class="sxs-lookup"><span data-stu-id="f89f8-172">Requesting a subsequent page of people</span></span>

<span data-ttu-id="f89f8-p110">最初の応答に関連のある人物のリストを完全に含められない場合は、追加の情報ページを要求するために、*$top* と *$skip* を使用して 2 番目の要求を行うことができます。前の要求に追加情報が含まれている場合は、次の要求でサーバーから人物についての後続ページを取得します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p110">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="f89f8-175">応答の並べ替え</span><span class="sxs-lookup"><span data-stu-id="f89f8-175">Sort the response</span></span>

<span data-ttu-id="f89f8-p111">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。このクエリでは、自分に最も関連のある人物を選択し、その人物を表示名で並べ替えてから、最初の 10 人の人物を並べ替え済みのリストで返します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p111">By default the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="f89f8-179">返される人物の数と返されるフィールドの変更</span><span class="sxs-lookup"><span data-stu-id="f89f8-179">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="f89f8-180">応答で返される人物の数は、*$top* パラメーターを設定することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-180">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="f89f8-181">次の例の要求に最も関連する 1,000 人`/me`。</span><span class="sxs-lookup"><span data-stu-id="f89f8-181">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="f89f8-182">また、この要求では、人物の表示名のみを要求することで、サーバーから返されるデータの量も制限しています。</span><span class="sxs-lookup"><span data-stu-id="f89f8-182">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="f89f8-183">返されるフィールドの選択</span><span class="sxs-lookup"><span data-stu-id="f89f8-183">Selecting the fields to return</span></span>

<span data-ttu-id="f89f8-p113">サーバーから返されるデータの量は、1 つ以上のフィールドを選択する *$select* パラメーターを使用することで制限できます。*@odata.id* フィールドは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p113">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="f89f8-186">次に示す例では、最も関連のある 10 人の人物の *DisplayName* と *EmailAddress* に応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-186">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="f89f8-187">フィルターを使用した応答の制限</span><span class="sxs-lookup"><span data-stu-id="f89f8-187">Using a filter to limit the response</span></span>

<span data-ttu-id="f89f8-188">*$filter* パラメーターを使用すると、指定した条件に等しいレコードを持つ人物のみに応答を制限できます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-188">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="f89f8-189">次のクエリは、ソースの [ディレクトリ] にしますユーザーへの応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-189">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="f89f8-190">フィルター処理された応答で返されるフィールドを選ぶ</span><span class="sxs-lookup"><span data-stu-id="f89f8-190">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="f89f8-191">*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-191">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="f89f8-p114">次に示す例では、指定した名前と等しい表示名を持つ人物の *DisplayName* と *EmailAddress* を取得します。この例では、表示名が "Nestor Kellum" と等しい人物のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-p114">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name. In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="f89f8-194">人物の検索</span><span class="sxs-lookup"><span data-stu-id="f89f8-194">Search people</span></span>

<span data-ttu-id="f89f8-195">このセクション内の要求も取得ユーザー サインイン中のユーザーに最も関連する (`/me`)。</span><span class="sxs-lookup"><span data-stu-id="f89f8-195">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="f89f8-196">検索要求には、People.Read アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f89f8-196">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="f89f8-197">検索による人物の選択</span><span class="sxs-lookup"><span data-stu-id="f89f8-197">Using search to select people</span></span>

<span data-ttu-id="f89f8-198">*$search* パラメーターを使用して、特定の条件セットを満たす人物を選びます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-198">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="f89f8-199">人を返すに関連する次の検索クエリ`/me`名または姓を持つが、文字"j"で始まります。</span><span class="sxs-lookup"><span data-stu-id="f89f8-199">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="f89f8-200">検索による関連するトピックの指定</span><span class="sxs-lookup"><span data-stu-id="f89f8-200">Using search to specify a relevant topic</span></span>

<span data-ttu-id="f89f8-201">人を返すに関連する次のような要求`/me`名前持つにはには、"ma"と「機能は計画」との関連付けがある人が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f89f8-201">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="f89f8-202">あいまい検索の実行</span><span class="sxs-lookup"><span data-stu-id="f89f8-202">Performing a fuzzy search</span></span>

<span data-ttu-id="f89f8-203">次に示す要求では、"Hermaini Hall" という名前の人物について検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-203">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="f89f8-204">サインイン中のユーザーに関連の「Herminia の船体」という名前の人があるため、「Herminia 船体」の情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-204">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="f89f8-205">関連する人</span><span class="sxs-lookup"><span data-stu-id="f89f8-205">Related people</span></span>

<span data-ttu-id="f89f8-206">次のような要求では、ユーザーの組織で他のユーザーに最も関連するユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="f89f8-206">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="f89f8-207">この要求には、People.Read.All のアクセス許可を User.ReadBasic.All が必要です。</span><span class="sxs-lookup"><span data-stu-id="f89f8-207">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="f89f8-208">この例では、Nestor Kellum の関連する人が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f89f8-208">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
