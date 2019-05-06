---
title: ユーザーを一覧表示する
description: ユーザーとの関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された人物オブジェクトのコレクションを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: e7dd5c2ffefe57ffebf5e8d2fe3e9dca3101a488
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571227"
---
# <a name="list-people"></a><span data-ttu-id="9c7e1-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9c7e1-103">List people</span></span>

<span data-ttu-id="9c7e1-104">[ユーザー](../resources/user.md)との関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された[人物](../resources/person.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="9c7e1-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](/graph/people-example)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c7e1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9c7e1-107">Permissions</span></span>

<span data-ttu-id="9c7e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c7e1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c7e1-110">Permission type</span></span>      | <span data-ttu-id="9c7e1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c7e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c7e1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c7e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c7e1-113">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c7e1-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="9c7e1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c7e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c7e1-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="9c7e1-115">People.Read</span></span>    |
|<span data-ttu-id="9c7e1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c7e1-116">Application</span></span> | <span data-ttu-id="9c7e1-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c7e1-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c7e1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c7e1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c7e1-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9c7e1-119">Optional query parameters</span></span>

<span data-ttu-id="9c7e1-120">このメソッドでは、「[ユーザーの関連情報を取得する](/graph/people-example)」の記事に示す例のように、[OData クエリ パラメーター](/graph/query-parameters)を使用して応答をカスタマイズすることができます。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="9c7e1-121">名前</span><span class="sxs-lookup"><span data-stu-id="9c7e1-121">Name</span></span>|<span data-ttu-id="9c7e1-122">値</span><span class="sxs-lookup"><span data-stu-id="9c7e1-122">Value</span></span>|<span data-ttu-id="9c7e1-123">説明</span><span class="sxs-lookup"><span data-stu-id="9c7e1-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="9c7e1-124">$filter</span><span class="sxs-lookup"><span data-stu-id="9c7e1-124">$filter</span></span>|<span data-ttu-id="9c7e1-125">string</span><span class="sxs-lookup"><span data-stu-id="9c7e1-125">string</span></span>|<span data-ttu-id="9c7e1-126">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="9c7e1-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="9c7e1-127">$orderby</span></span>|<span data-ttu-id="9c7e1-128">string</span><span class="sxs-lookup"><span data-stu-id="9c7e1-128">string</span></span>|<span data-ttu-id="9c7e1-129">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="9c7e1-130">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="9c7e1-131">$search</span><span class="sxs-lookup"><span data-stu-id="9c7e1-131">$search</span></span>|<span data-ttu-id="9c7e1-132">string</span><span class="sxs-lookup"><span data-stu-id="9c7e1-132">string</span></span>|<span data-ttu-id="9c7e1-133">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-133">Search for people by name or alias.</span></span> <span data-ttu-id="9c7e1-134">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="9c7e1-135">パラメーターは、サインインしたユーザーの関連人物を検索するためにのみ機能し、他のユーザーに関連する人物を検索するためには機能しません。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="9c7e1-136">その人とのメール会話から抽出されたトピックに基づいて人を見つける `topic` キーワードもサポートします。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="9c7e1-137">情報と例については、[関係者の情報を取得する](/graph/people-example#perform-a-fuzzy-search)の*あいまい検索の実行*セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="9c7e1-138">$select</span><span class="sxs-lookup"><span data-stu-id="9c7e1-138">$select</span></span>|<span data-ttu-id="9c7e1-139">string</span><span class="sxs-lookup"><span data-stu-id="9c7e1-139">string</span></span>|<span data-ttu-id="9c7e1-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="9c7e1-142">$skip</span><span class="sxs-lookup"><span data-stu-id="9c7e1-142">$skip</span></span>|<span data-ttu-id="9c7e1-143">int</span><span class="sxs-lookup"><span data-stu-id="9c7e1-143">int</span></span>|<span data-ttu-id="9c7e1-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="9c7e1-146">$top</span><span class="sxs-lookup"><span data-stu-id="9c7e1-146">$top</span></span>|<span data-ttu-id="9c7e1-147">int</span><span class="sxs-lookup"><span data-stu-id="9c7e1-147">int</span></span>|<span data-ttu-id="9c7e1-148">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9c7e1-149">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c7e1-149">Request headers</span></span>

| <span data-ttu-id="9c7e1-150">名前</span><span class="sxs-lookup"><span data-stu-id="9c7e1-150">Name</span></span>      |<span data-ttu-id="9c7e1-151">説明</span><span class="sxs-lookup"><span data-stu-id="9c7e1-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c7e1-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7e1-152">Authorization</span></span>  | <span data-ttu-id="9c7e1-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c7e1-155">承諾</span><span class="sxs-lookup"><span data-stu-id="9c7e1-155">Accept</span></span> | <span data-ttu-id="9c7e1-156">application/json</span><span class="sxs-lookup"><span data-stu-id="9c7e1-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c7e1-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c7e1-157">Request body</span></span>

<span data-ttu-id="9c7e1-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c7e1-159">応答</span><span class="sxs-lookup"><span data-stu-id="9c7e1-159">Response</span></span>

<span data-ttu-id="9c7e1-p108">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトのコレクションを返します。応答には、1 つの person オブジェクトまたは person オブジェクトのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="9c7e1-162">例</span><span class="sxs-lookup"><span data-stu-id="9c7e1-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="9c7e1-163">要求</span><span class="sxs-lookup"><span data-stu-id="9c7e1-163">Request</span></span>

<span data-ttu-id="9c7e1-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="9c7e1-165">応答</span><span class="sxs-lookup"><span data-stu-id="9c7e1-165">Response</span></span>

<span data-ttu-id="9c7e1-166">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="9c7e1-167">他の例については、「[関係する人の情報を取得する](/graph/people-example)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c7e1-167">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
