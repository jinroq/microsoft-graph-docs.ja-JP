---
title: ユーザーを一覧表示する
description: ユーザーとの関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された人物オブジェクトのコレクションを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: be4bb525cbc37781ad49312041da26cc84299459
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274012"
---
# <a name="list-people"></a><span data-ttu-id="e2c39-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e2c39-103">List people</span></span>

<span data-ttu-id="e2c39-104">[ユーザー](../resources/user.md)との関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された[人物](../resources/person.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="e2c39-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](/graph/people-example)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2c39-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2c39-107">Permissions</span></span>

<span data-ttu-id="e2c39-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2c39-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2c39-110">Permission type</span></span>      | <span data-ttu-id="e2c39-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2c39-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2c39-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2c39-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2c39-113">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2c39-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="e2c39-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2c39-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2c39-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="e2c39-115">People.Read</span></span>    |
|<span data-ttu-id="e2c39-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2c39-116">Application</span></span> | <span data-ttu-id="e2c39-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2c39-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2c39-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2c39-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2c39-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2c39-119">Optional query parameters</span></span>

<span data-ttu-id="e2c39-120">このメソッドでは、「[ユーザーの関連情報を取得する](/graph/people-example)」の記事に示す例のように、[OData クエリ パラメーター](/graph/query-parameters)を使用して応答をカスタマイズすることができます。</span><span class="sxs-lookup"><span data-stu-id="e2c39-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="e2c39-121">名前</span><span class="sxs-lookup"><span data-stu-id="e2c39-121">Name</span></span>|<span data-ttu-id="e2c39-122">値</span><span class="sxs-lookup"><span data-stu-id="e2c39-122">Value</span></span>|<span data-ttu-id="e2c39-123">説明</span><span class="sxs-lookup"><span data-stu-id="e2c39-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="e2c39-124">$filter</span><span class="sxs-lookup"><span data-stu-id="e2c39-124">$filter</span></span>|<span data-ttu-id="e2c39-125">string</span><span class="sxs-lookup"><span data-stu-id="e2c39-125">string</span></span>|<span data-ttu-id="e2c39-126">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="e2c39-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="e2c39-127">$orderby</span></span>|<span data-ttu-id="e2c39-128">string</span><span class="sxs-lookup"><span data-stu-id="e2c39-128">string</span></span>|<span data-ttu-id="e2c39-129">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="e2c39-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="e2c39-130">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="e2c39-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e2c39-131">$search</span><span class="sxs-lookup"><span data-stu-id="e2c39-131">$search</span></span>|<span data-ttu-id="e2c39-132">string</span><span class="sxs-lookup"><span data-stu-id="e2c39-132">string</span></span>|<span data-ttu-id="e2c39-133">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-133">Search for people by name or alias.</span></span> <span data-ttu-id="e2c39-134">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2c39-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="e2c39-135">パラメーターは、サインインしたユーザーの関連人物を検索するためにのみ機能し、他のユーザーに関連する人物を検索するためには機能しません。</span><span class="sxs-lookup"><span data-stu-id="e2c39-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="e2c39-136">その人とのメール会話から抽出されたトピックに基づいて人を見つける `topic` キーワードもサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2c39-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="e2c39-137">情報と例については、[関係者の情報を取得する](/graph/people-example#perform-a-fuzzy-search)の*あいまい検索の実行*セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2c39-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="e2c39-138">$select</span><span class="sxs-lookup"><span data-stu-id="e2c39-138">$select</span></span>|<span data-ttu-id="e2c39-139">string</span><span class="sxs-lookup"><span data-stu-id="e2c39-139">string</span></span>|<span data-ttu-id="e2c39-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="e2c39-142">$skip</span><span class="sxs-lookup"><span data-stu-id="e2c39-142">$skip</span></span>|<span data-ttu-id="e2c39-143">int</span><span class="sxs-lookup"><span data-stu-id="e2c39-143">int</span></span>|<span data-ttu-id="e2c39-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="e2c39-146">$top</span><span class="sxs-lookup"><span data-stu-id="e2c39-146">$top</span></span>|<span data-ttu-id="e2c39-147">int</span><span class="sxs-lookup"><span data-stu-id="e2c39-147">int</span></span>|<span data-ttu-id="e2c39-148">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="e2c39-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e2c39-149">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2c39-149">Request headers</span></span>

| <span data-ttu-id="e2c39-150">名前</span><span class="sxs-lookup"><span data-stu-id="e2c39-150">Name</span></span>      |<span data-ttu-id="e2c39-151">説明</span><span class="sxs-lookup"><span data-stu-id="e2c39-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2c39-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2c39-152">Authorization</span></span>  | <span data-ttu-id="e2c39-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2c39-155">承諾</span><span class="sxs-lookup"><span data-stu-id="e2c39-155">Accept</span></span> | <span data-ttu-id="e2c39-156">application/json</span><span class="sxs-lookup"><span data-stu-id="e2c39-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2c39-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2c39-157">Request body</span></span>

<span data-ttu-id="e2c39-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2c39-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2c39-159">応答</span><span class="sxs-lookup"><span data-stu-id="e2c39-159">Response</span></span>

<span data-ttu-id="e2c39-p108">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトのコレクションを返します。応答には、1 つの person オブジェクトまたは person オブジェクトのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e2c39-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="e2c39-162">例</span><span class="sxs-lookup"><span data-stu-id="e2c39-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="e2c39-163">要求</span><span class="sxs-lookup"><span data-stu-id="e2c39-163">Request</span></span>

<span data-ttu-id="e2c39-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="e2c39-165">応答</span><span class="sxs-lookup"><span data-stu-id="e2c39-165">Response</span></span>

<span data-ttu-id="e2c39-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2c39-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1370

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
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2c39-167">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e2c39-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2c39-168">C#</span><span class="sxs-lookup"><span data-stu-id="e2c39-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_person_collection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2c39-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2c39-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_person_collection-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e2c39-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2c39-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_person_collection-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e2c39-171">他の例については、「[関係する人の情報を取得する](/graph/people-example)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2c39-171">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
