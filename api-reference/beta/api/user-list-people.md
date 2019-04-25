---
title: ユーザーを一覧表示する
description: ユーザーのコミュニケーションとコラボレーションパターン、およびビジネス上の関係によって決定される、ユーザーに対して関連性のある人物が注文した人物オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: deb9fd929a2b0b8ce4da9392cb465497c2236b0c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544296"
---
# <a name="list-people"></a><span data-ttu-id="2f1ae-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2f1ae-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f1ae-104">ユーザーのコミュニケーションとコラボレーションパターン、およびビジネス上の関係によって決定される、[ユーザー](../resources/user.md)に対して関連性のある人物が注文した[人物](../resources/person.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f1ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f1ae-105">Permissions</span></span>

<span data-ttu-id="2f1ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f1ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f1ae-108">Permission type</span></span>      | <span data-ttu-id="2f1ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f1ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f1ae-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="2f1ae-111">People.Read</span></span>    |
|<span data-ttu-id="2f1ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f1ae-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="2f1ae-113">People.Read</span></span>    |
|<span data-ttu-id="2f1ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f1ae-114">Application</span></span> | <span data-ttu-id="2f1ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f1ae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f1ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f1ae-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f1ae-117">Optional query parameters</span></span>

<span data-ttu-id="2f1ae-118">このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="2f1ae-119">名前</span><span class="sxs-lookup"><span data-stu-id="2f1ae-119">Name</span></span>|<span data-ttu-id="2f1ae-120">値</span><span class="sxs-lookup"><span data-stu-id="2f1ae-120">Value</span></span>|<span data-ttu-id="2f1ae-121">説明</span><span class="sxs-lookup"><span data-stu-id="2f1ae-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="2f1ae-122">$filter</span><span class="sxs-lookup"><span data-stu-id="2f1ae-122">$filter</span></span>|<span data-ttu-id="2f1ae-123">string</span><span class="sxs-lookup"><span data-stu-id="2f1ae-123">string</span></span>|<span data-ttu-id="2f1ae-124">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="2f1ae-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="2f1ae-125">$orderby</span></span>|<span data-ttu-id="2f1ae-126">string</span><span class="sxs-lookup"><span data-stu-id="2f1ae-126">string</span></span>|<span data-ttu-id="2f1ae-127">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="2f1ae-128">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="2f1ae-129">$search</span><span class="sxs-lookup"><span data-stu-id="2f1ae-129">$search</span></span>|<span data-ttu-id="2f1ae-130">string</span><span class="sxs-lookup"><span data-stu-id="2f1ae-130">string</span></span>|<span data-ttu-id="2f1ae-131">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-131">Search for people by name or alias.</span></span> <span data-ttu-id="2f1ae-132">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="2f1ae-133">パラメーターは、サインインしているユーザーの関連する人物を検索する場合にのみ機能し、他のユーザーに関連する人物を検索する目的では使用できません。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="2f1ae-134">また、 `topic`その人物との電子メールによる会話から抜粋したトピックに基づいてユーザーを検索するキーワードもサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="2f1ae-135">情報と例については、「[ユーザーに関する情報を取得](/graph/people-example#perform-a-fuzzy-search)する」の「*あいまい検索を実行*する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="2f1ae-136">$select</span><span class="sxs-lookup"><span data-stu-id="2f1ae-136">$select</span></span>|<span data-ttu-id="2f1ae-137">string</span><span class="sxs-lookup"><span data-stu-id="2f1ae-137">string</span></span>|<span data-ttu-id="2f1ae-p104">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="2f1ae-140">$skip</span><span class="sxs-lookup"><span data-stu-id="2f1ae-140">$skip</span></span>|<span data-ttu-id="2f1ae-141">int</span><span class="sxs-lookup"><span data-stu-id="2f1ae-141">int</span></span>|<span data-ttu-id="2f1ae-p105">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="2f1ae-144">$top</span><span class="sxs-lookup"><span data-stu-id="2f1ae-144">$top</span></span>|<span data-ttu-id="2f1ae-145">int</span><span class="sxs-lookup"><span data-stu-id="2f1ae-145">int</span></span>|<span data-ttu-id="2f1ae-146">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2f1ae-147">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f1ae-147">Request headers</span></span>

| <span data-ttu-id="2f1ae-148">名前</span><span class="sxs-lookup"><span data-stu-id="2f1ae-148">Name</span></span>      |<span data-ttu-id="2f1ae-149">説明</span><span class="sxs-lookup"><span data-stu-id="2f1ae-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f1ae-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f1ae-150">Authorization</span></span>  | <span data-ttu-id="2f1ae-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f1ae-153">承諾</span><span class="sxs-lookup"><span data-stu-id="2f1ae-153">Accept</span></span> | <span data-ttu-id="2f1ae-154">application/json</span><span class="sxs-lookup"><span data-stu-id="2f1ae-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f1ae-155">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f1ae-155">Request body</span></span>

<span data-ttu-id="2f1ae-156">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f1ae-157">応答</span><span class="sxs-lookup"><span data-stu-id="2f1ae-157">Response</span></span>

<span data-ttu-id="2f1ae-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[person](../resources/person.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f1ae-159">例</span><span class="sxs-lookup"><span data-stu-id="2f1ae-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="2f1ae-160">参照</span><span class="sxs-lookup"><span data-stu-id="2f1ae-160">Browse</span></span>

<span data-ttu-id="2f1ae-161">このセクションの要求は、コミュニケーション、コラボレーション、およびビジネスのリレーションシップに基づいて`/me`、サインインしているユーザーに最も関連のある人物を取得します ()。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="2f1ae-162">既定では、応答ごとに 10 件のレコードが返されます。ただし、$top パラメーターを使用することで、*これを変更*できます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="2f1ae-163">これらの要求には、ユーザーの読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="2f1ae-164">要求</span><span class="sxs-lookup"><span data-stu-id="2f1ae-164">Request</span></span>

<span data-ttu-id="2f1ae-165">既定の要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="2f1ae-166">応答</span><span class="sxs-lookup"><span data-stu-id="2f1ae-166">Response</span></span>

<span data-ttu-id="2f1ae-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-167">The following is an example of the response.</span></span>
><span data-ttu-id="2f1ae-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="2f1ae-170">人物の続きのページの要求</span><span class="sxs-lookup"><span data-stu-id="2f1ae-170">Requesting a subsequent page of people</span></span>

<span data-ttu-id="2f1ae-p109">最初の応答に関連のある人物のリストを完全に含められない場合は、追加の情報ページを要求するために、*$top* と *$skip* を使用して 2 番目の要求を行うことができます。前の要求に追加情報が含まれている場合は、次の要求でサーバーから人物についての後続ページを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="2f1ae-173">応答の並べ替え</span><span class="sxs-lookup"><span data-stu-id="2f1ae-173">Sort the response</span></span>

<span data-ttu-id="2f1ae-p110">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。 応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。 このクエリでは、自分に最も関連のある人物を選択し、その人物を表示名で並べ替えてから、最初の 10 人の人物を並べ替え済みのリストで返します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p110">By default the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="2f1ae-177">返される人物の数と返されるフィールドの変更</span><span class="sxs-lookup"><span data-stu-id="2f1ae-177">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="2f1ae-178">応答で返される人物の数は、*$top* パラメーターを設定することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-178">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="2f1ae-179">次の例では、最も関連のある`/me`1000 ユーザーを要求します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-179">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="2f1ae-180">また、この要求では、人物の表示名のみを要求することで、サーバーから返されるデータの量も制限しています。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-180">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="2f1ae-181">返されるフィールドの選択</span><span class="sxs-lookup"><span data-stu-id="2f1ae-181">Selecting the fields to return</span></span>

<span data-ttu-id="2f1ae-p112">サーバーから返されるデータの量は、1 つ以上のフィールドを選択する *$select* パラメーターを使用することで制限できます。*@odata.id* フィールドは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p112">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="2f1ae-184">次に示す例では、最も関連のある 10 人の人物の *DisplayName* と *EmailAddress* に応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-184">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="2f1ae-185">フィルターを使用した応答の制限</span><span class="sxs-lookup"><span data-stu-id="2f1ae-185">Using a filter to limit the response</span></span>

<span data-ttu-id="2f1ae-186">*$filter* パラメーターを使用すると、指定した条件に等しいレコードを持つ人物のみに応答を制限できます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-186">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="2f1ae-187">次のクエリは、ソース "Directory" を持つユーザーに対する応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-187">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="2f1ae-188">フィルター処理された応答で返されるフィールドを選択する</span><span class="sxs-lookup"><span data-stu-id="2f1ae-188">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="2f1ae-189">*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-189">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="2f1ae-p113">次に示す例では、指定した名前と等しい表示名を持つ人物の *DisplayName* と *EmailAddress* を取得します。 この例では、表示名が "Nestor Kellum" と等しい人物のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p113">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name. In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="2f1ae-192">人物の検索</span><span class="sxs-lookup"><span data-stu-id="2f1ae-192">Search people</span></span>

<span data-ttu-id="2f1ae-193">このセクションの要求は、サインインしているユーザーに最も関連のある人物を`/me`取得することもできます ()。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-193">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="2f1ae-194">検索要求には、ユーザーの読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-194">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="2f1ae-195">検索による人物の選択</span><span class="sxs-lookup"><span data-stu-id="2f1ae-195">Using search to select people</span></span>

<span data-ttu-id="2f1ae-196">*$search* パラメーターを使用して、特定の条件セットを満たす人物を選びます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-196">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="2f1ae-197">次の検索クエリは、GivenName また`/me`は姓が "j" という文字で始まる人物を返します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-197">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="2f1ae-198">検索による関連するトピックの指定</span><span class="sxs-lookup"><span data-stu-id="2f1ae-198">Using search to specify a relevant topic</span></span>

<span data-ttu-id="2f1ae-199">次の要求では、名前`/me`に "ma" が含まれていて、"機能の計画" と関連付けられている人物を返します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-199">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="2f1ae-200">あいまい検索の実行</span><span class="sxs-lookup"><span data-stu-id="2f1ae-200">Performing a fuzzy search</span></span>

<span data-ttu-id="2f1ae-201">次に示す要求では、"Hermaini Hall" という名前の人物について検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-201">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="2f1ae-202">サインインしているユーザーに関連する "Herminia Hull" という名前の人物が存在するため、"Herminia Hull" の情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-202">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="2f1ae-203">関連する人</span><span class="sxs-lookup"><span data-stu-id="2f1ae-203">Related people</span></span>

<span data-ttu-id="2f1ae-204">次の要求は、ユーザーの組織内の他のユーザーに最も関連のある人物を取得します。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-204">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="2f1ae-205">この要求には、ユーザーに対してすべてのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-205">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="2f1ae-206">この例では、nestor Kellum の関連する人物が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2f1ae-206">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
