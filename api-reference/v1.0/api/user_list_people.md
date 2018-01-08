# <a name="list-people"></a><span data-ttu-id="3f8a0-101">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3f8a0-101">List people</span></span>

<span data-ttu-id="3f8a0-102">[ユーザー](../resources/user.md)との関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された[人物](../resources/person.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="3f8a0-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f8a0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f8a0-105">Permissions</span></span>
<span data-ttu-id="3f8a0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3f8a0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f8a0-108">Permission type</span></span>      | <span data-ttu-id="3f8a0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f8a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f8a0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f8a0-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f8a0-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="3f8a0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f8a0-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="3f8a0-113">People.Read</span></span>    |
|<span data-ttu-id="3f8a0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f8a0-114">Application</span></span> | <span data-ttu-id="3f8a0-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f8a0-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f8a0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f8a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f8a0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3f8a0-117">Optional query parameters</span></span>
<span data-ttu-id="3f8a0-118">このメソッドでは、「[ユーザーの関連情報を取得する](../../../concepts/people_example.md)」の記事に示す例のように、[OData クエリ パラメーター](../../../concepts/query_parameters.md)を使用して応答をカスタマイズすることができます。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-118">This method supports the [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, as shown in the examples in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="3f8a0-119">名前</span><span class="sxs-lookup"><span data-stu-id="3f8a0-119">Name</span></span>|<span data-ttu-id="3f8a0-120">値</span><span class="sxs-lookup"><span data-stu-id="3f8a0-120">Value</span></span>|<span data-ttu-id="3f8a0-121">説明</span><span class="sxs-lookup"><span data-stu-id="3f8a0-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="3f8a0-122">$filter</span><span class="sxs-lookup"><span data-stu-id="3f8a0-122">$filter</span></span>|<span data-ttu-id="3f8a0-123">string</span><span class="sxs-lookup"><span data-stu-id="3f8a0-123">string</span></span>|<span data-ttu-id="3f8a0-124">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="3f8a0-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="3f8a0-125">$orderby</span></span>|<span data-ttu-id="3f8a0-126">string</span><span class="sxs-lookup"><span data-stu-id="3f8a0-126">string</span></span>|<span data-ttu-id="3f8a0-127">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="3f8a0-128">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="3f8a0-129">$search</span><span class="sxs-lookup"><span data-stu-id="3f8a0-129">$search</span></span>|<span data-ttu-id="3f8a0-130">string</span><span class="sxs-lookup"><span data-stu-id="3f8a0-130">string</span></span>|<span data-ttu-id="3f8a0-131">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="3f8a0-132">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-132">Supports Fuzzy matching.</span></span>| 
|<span data-ttu-id="3f8a0-133">$select</span><span class="sxs-lookup"><span data-stu-id="3f8a0-133">$select</span></span>|<span data-ttu-id="3f8a0-134">string</span><span class="sxs-lookup"><span data-stu-id="3f8a0-134">string</span></span>|<span data-ttu-id="3f8a0-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="3f8a0-137">$skip</span><span class="sxs-lookup"><span data-stu-id="3f8a0-137">$skip</span></span>|<span data-ttu-id="3f8a0-138">int</span><span class="sxs-lookup"><span data-stu-id="3f8a0-138">int</span></span>|<span data-ttu-id="3f8a0-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="3f8a0-141">$top</span><span class="sxs-lookup"><span data-stu-id="3f8a0-141">$top</span></span>|<span data-ttu-id="3f8a0-142">int</span><span class="sxs-lookup"><span data-stu-id="3f8a0-142">int</span></span>|<span data-ttu-id="3f8a0-143">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="3f8a0-144">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f8a0-144">Request headers</span></span>
| <span data-ttu-id="3f8a0-145">名前</span><span class="sxs-lookup"><span data-stu-id="3f8a0-145">Name</span></span>      |<span data-ttu-id="3f8a0-146">説明</span><span class="sxs-lookup"><span data-stu-id="3f8a0-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f8a0-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f8a0-147">Authorization</span></span>  | <span data-ttu-id="3f8a0-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f8a0-150">承諾</span><span class="sxs-lookup"><span data-stu-id="3f8a0-150">Accept</span></span> | <span data-ttu-id="3f8a0-151">application/json</span><span class="sxs-lookup"><span data-stu-id="3f8a0-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f8a0-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f8a0-152">Request body</span></span>
<span data-ttu-id="3f8a0-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f8a0-154">応答</span><span class="sxs-lookup"><span data-stu-id="3f8a0-154">Response</span></span>
<span data-ttu-id="3f8a0-p108">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトのコレクションを返します。応答には、1 つの person オブジェクトまたは person オブジェクトのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="3f8a0-157">例</span><span class="sxs-lookup"><span data-stu-id="3f8a0-157">Examples</span></span>
#### <a name="request"></a><span data-ttu-id="3f8a0-158">要求</span><span class="sxs-lookup"><span data-stu-id="3f8a0-158">Request</span></span>
<span data-ttu-id="3f8a0-159">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-159">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="3f8a0-160">応答</span><span class="sxs-lookup"><span data-stu-id="3f8a0-160">Response</span></span>
<span data-ttu-id="3f8a0-161">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-161">The following is an example of a response.</span></span>

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

<span data-ttu-id="3f8a0-162">他の例については、「[関係する人の情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f8a0-162">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
