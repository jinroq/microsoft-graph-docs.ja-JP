# <a name="list-people"></a><span data-ttu-id="99e8c-101">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="99e8c-101">List people</span></span>

<span data-ttu-id="99e8c-102">[ユーザー](../resources/user.md)との関連 (ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決まる) によって配列された[人物](../resources/person.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="99e8c-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="99e8c-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99e8c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99e8c-105">Permissions</span></span>
<span data-ttu-id="99e8c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="99e8c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99e8c-108">Permission type</span></span>      | <span data-ttu-id="99e8c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99e8c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e8c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99e8c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99e8c-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="99e8c-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="99e8c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99e8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e8c-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="99e8c-113">People.Read</span></span>    |
|<span data-ttu-id="99e8c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99e8c-114">Application</span></span> | <span data-ttu-id="99e8c-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="99e8c-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99e8c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99e8c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99e8c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="99e8c-117">Optional query parameters</span></span>
|<span data-ttu-id="99e8c-118">名前</span><span class="sxs-lookup"><span data-stu-id="99e8c-118">Name</span></span>|<span data-ttu-id="99e8c-119">値</span><span class="sxs-lookup"><span data-stu-id="99e8c-119">Value</span></span>|<span data-ttu-id="99e8c-120">説明</span><span class="sxs-lookup"><span data-stu-id="99e8c-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="99e8c-121">$filter</span><span class="sxs-lookup"><span data-stu-id="99e8c-121">$filter</span></span>|<span data-ttu-id="99e8c-122">string</span><span class="sxs-lookup"><span data-stu-id="99e8c-122">string</span></span>|<span data-ttu-id="99e8c-123">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="99e8c-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="99e8c-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="99e8c-124">$orderby</span></span>|<span data-ttu-id="99e8c-125">string</span><span class="sxs-lookup"><span data-stu-id="99e8c-125">string</span></span>|<span data-ttu-id="99e8c-p103">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="99e8c-128">$search</span><span class="sxs-lookup"><span data-stu-id="99e8c-128">$search</span></span>|<span data-ttu-id="99e8c-129">string</span><span class="sxs-lookup"><span data-stu-id="99e8c-129">string</span></span>|<span data-ttu-id="99e8c-p104">名またはエイリアスで人物を検索します。ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="99e8c-132">$select</span><span class="sxs-lookup"><span data-stu-id="99e8c-132">$select</span></span>|<span data-ttu-id="99e8c-133">string</span><span class="sxs-lookup"><span data-stu-id="99e8c-133">string</span></span>|<span data-ttu-id="99e8c-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="99e8c-136">$skip</span><span class="sxs-lookup"><span data-stu-id="99e8c-136">$skip</span></span>|<span data-ttu-id="99e8c-137">int</span><span class="sxs-lookup"><span data-stu-id="99e8c-137">int</span></span>|<span data-ttu-id="99e8c-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="99e8c-140">$top</span><span class="sxs-lookup"><span data-stu-id="99e8c-140">$top</span></span>|<span data-ttu-id="99e8c-141">int</span><span class="sxs-lookup"><span data-stu-id="99e8c-141">int</span></span>|<span data-ttu-id="99e8c-142">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="99e8c-142">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="99e8c-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99e8c-143">Request headers</span></span>
| <span data-ttu-id="99e8c-144">名前</span><span class="sxs-lookup"><span data-stu-id="99e8c-144">Name</span></span>      |<span data-ttu-id="99e8c-145">説明</span><span class="sxs-lookup"><span data-stu-id="99e8c-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99e8c-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e8c-146">Authorization</span></span>  | <span data-ttu-id="99e8c-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99e8c-149">承諾</span><span class="sxs-lookup"><span data-stu-id="99e8c-149">Accept</span></span> | <span data-ttu-id="99e8c-150">application/json</span><span class="sxs-lookup"><span data-stu-id="99e8c-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="99e8c-151">要求本文</span><span class="sxs-lookup"><span data-stu-id="99e8c-151">Request body</span></span>
<span data-ttu-id="99e8c-152">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99e8c-152">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99e8c-153">応答</span><span class="sxs-lookup"><span data-stu-id="99e8c-153">Response</span></span>
<span data-ttu-id="99e8c-p108">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトのコレクションを返します。応答には、1 つの person オブジェクトまたは person オブジェクトのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="99e8c-156">例</span><span class="sxs-lookup"><span data-stu-id="99e8c-156">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="99e8c-157">関連する人物のコレクションの取得</span><span class="sxs-lookup"><span data-stu-id="99e8c-157">Get a collection of relevant people</span></span> 

<span data-ttu-id="99e8c-158">次に示す要求では、コミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップに基づいて、サインインしているユーザーに最も関連のある人物を取得します (`/me`)。</span><span class="sxs-lookup"><span data-stu-id="99e8c-158">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="99e8c-p109">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* クエリ パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
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

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        }
    ]
}
```
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="99e8c-163">他のユーザーの関連する人物の検索</span><span class="sxs-lookup"><span data-stu-id="99e8c-163">Search other user’s relevant people</span></span>

<span data-ttu-id="99e8c-p110">次の要求は、サインインしているユーザーの組織内の他の人物と最も関連のある人物を取得します。この要求には People.Read.All アクセス許可が必要です。この例では、Roscoe Seidel の関連する人物が表示されます。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p110">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_other_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="99e8c-p111">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="99e8c-p111">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_other_person",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        }
    ]
}
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
