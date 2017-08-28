# <a name="get-person"></a><span data-ttu-id="016aa-101">人物を取得する</span><span class="sxs-lookup"><span data-stu-id="016aa-101">Get person</span></span>

<span data-ttu-id="016aa-102">[person](../resources/person.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="016aa-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="016aa-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="016aa-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="016aa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="016aa-105">Permissions</span></span>
<span data-ttu-id="016aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="016aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="016aa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="016aa-108">Permission type</span></span>      | <span data-ttu-id="016aa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="016aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="016aa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="016aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="016aa-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="016aa-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="016aa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="016aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="016aa-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="016aa-113">People.Read</span></span>    |
|<span data-ttu-id="016aa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="016aa-114">Application</span></span> | <span data-ttu-id="016aa-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="016aa-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="016aa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="016aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="016aa-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="016aa-117">Optional query parameters</span></span>
|<span data-ttu-id="016aa-118">名前</span><span class="sxs-lookup"><span data-stu-id="016aa-118">Name</span></span>|<span data-ttu-id="016aa-119">値</span><span class="sxs-lookup"><span data-stu-id="016aa-119">Value</span></span>|<span data-ttu-id="016aa-120">説明</span><span class="sxs-lookup"><span data-stu-id="016aa-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="016aa-121">$filter</span><span class="sxs-lookup"><span data-stu-id="016aa-121">$filter</span></span>|<span data-ttu-id="016aa-122">string</span><span class="sxs-lookup"><span data-stu-id="016aa-122">string</span></span>|<span data-ttu-id="016aa-123">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="016aa-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="016aa-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="016aa-124">$orderby</span></span>|<span data-ttu-id="016aa-125">string</span><span class="sxs-lookup"><span data-stu-id="016aa-125">string</span></span>|<span data-ttu-id="016aa-p103">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="016aa-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="016aa-128">$search</span><span class="sxs-lookup"><span data-stu-id="016aa-128">$search</span></span>|<span data-ttu-id="016aa-129">string</span><span class="sxs-lookup"><span data-stu-id="016aa-129">string</span></span>|<span data-ttu-id="016aa-p104">名またはエイリアスで人物を検索します。ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="016aa-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="016aa-132">$select</span><span class="sxs-lookup"><span data-stu-id="016aa-132">$select</span></span>|<span data-ttu-id="016aa-133">string</span><span class="sxs-lookup"><span data-stu-id="016aa-133">string</span></span>|<span data-ttu-id="016aa-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="016aa-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="016aa-136">$skip</span><span class="sxs-lookup"><span data-stu-id="016aa-136">$skip</span></span>|<span data-ttu-id="016aa-137">int</span><span class="sxs-lookup"><span data-stu-id="016aa-137">int</span></span>|<span data-ttu-id="016aa-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="016aa-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="016aa-140">$top</span><span class="sxs-lookup"><span data-stu-id="016aa-140">$top</span></span>|<span data-ttu-id="016aa-141">int</span><span class="sxs-lookup"><span data-stu-id="016aa-141">int</span></span>|<span data-ttu-id="016aa-142">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="016aa-142">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="016aa-143">パラメーター</span><span class="sxs-lookup"><span data-stu-id="016aa-143">Parameters</span></span>
| <span data-ttu-id="016aa-144">パラメーター</span><span class="sxs-lookup"><span data-stu-id="016aa-144">Parameter</span></span> |<span data-ttu-id="016aa-145">型</span><span class="sxs-lookup"><span data-stu-id="016aa-145">Type</span></span>       |<span data-ttu-id="016aa-146">説明</span><span class="sxs-lookup"><span data-stu-id="016aa-146">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="016aa-147">property_value</span><span class="sxs-lookup"><span data-stu-id="016aa-147">property_value</span></span>|<span data-ttu-id="016aa-148">String</span><span class="sxs-lookup"><span data-stu-id="016aa-148">String</span></span>     |<span data-ttu-id="016aa-p107">照合する拡張プロパティの値。「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="016aa-p107">The value of the extended property to match. Required where listed in the **HTTP request** section.</span></span>|
|<span data-ttu-id="016aa-151">person_property</span><span class="sxs-lookup"><span data-stu-id="016aa-151">person_property</span></span>|<span data-ttu-id="016aa-152">String</span><span class="sxs-lookup"><span data-stu-id="016aa-152">String</span></span>    |<span data-ttu-id="016aa-p108">一致させるユーザーのプロパティ。「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="016aa-p108">The person property to match. Required where listed in the **HTTP request** section.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="016aa-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="016aa-155">Request headers</span></span>
| <span data-ttu-id="016aa-156">名前</span><span class="sxs-lookup"><span data-stu-id="016aa-156">Name</span></span>      |<span data-ttu-id="016aa-157">説明</span><span class="sxs-lookup"><span data-stu-id="016aa-157">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="016aa-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="016aa-158">Authorization</span></span>  | <span data-ttu-id="016aa-p109">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="016aa-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="016aa-161">要求本文</span><span class="sxs-lookup"><span data-stu-id="016aa-161">Request body</span></span>
<span data-ttu-id="016aa-162">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="016aa-162">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="016aa-163">応答</span><span class="sxs-lookup"><span data-stu-id="016aa-163">Response</span></span>
<span data-ttu-id="016aa-p110">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトを返します。応答には、1 つの人物インスタンスまたは人物インスタンスのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="016aa-p110">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="016aa-166">例</span><span class="sxs-lookup"><span data-stu-id="016aa-166">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="016aa-167">検索を実行する</span><span class="sxs-lookup"><span data-stu-id="016aa-167">Perform a search</span></span> 
<span data-ttu-id="016aa-168">次に示す要求では、「Irene McGowan」という名前の人物について検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="016aa-168">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="016aa-169">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="016aa-169">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="016aa-170">フィルター処理された応答で返されるフィールドを選択する</span><span class="sxs-lookup"><span data-stu-id="016aa-170">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="016aa-171">*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="016aa-171">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="016aa-p111">次の例では、指定した名前と等しい表示名を持つ人物の **displayName** と **scoredEmailAddresses** を取得します。この例では、表示名が "Lorrie Frye" と等しい人物のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="016aa-p111">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="016aa-174">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="016aa-174">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
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
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
