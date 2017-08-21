# <a name="get-person"></a><span data-ttu-id="fceaa-101">人物を取得する</span><span class="sxs-lookup"><span data-stu-id="fceaa-101">Get person</span></span>

<span data-ttu-id="fceaa-102">[person](../resources/person.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fceaa-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/person.md) object.</span></span>

<span data-ttu-id="fceaa-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[関係する人の情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fceaa-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="fceaa-105">Prerequisites</span></span>
<span data-ttu-id="fceaa-106">この API の一部を実行するには、次の**アクセス許可**が必要です。*People.Read*、*People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="fceaa-106">The following **permissions** are required to execute portions of this API: *People.Read*; *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="fceaa-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fceaa-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fceaa-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fceaa-108">Optional query parameters</span></span>
|<span data-ttu-id="fceaa-109">名前</span><span class="sxs-lookup"><span data-stu-id="fceaa-109">Name</span></span>|<span data-ttu-id="fceaa-110">値</span><span class="sxs-lookup"><span data-stu-id="fceaa-110">Value</span></span>|<span data-ttu-id="fceaa-111">説明</span><span class="sxs-lookup"><span data-stu-id="fceaa-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="fceaa-112">$filter</span><span class="sxs-lookup"><span data-stu-id="fceaa-112">$filter</span></span>|<span data-ttu-id="fceaa-113">string</span><span class="sxs-lookup"><span data-stu-id="fceaa-113">string</span></span>|<span data-ttu-id="fceaa-114">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="fceaa-114">You can use the $filter parameter to limit the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="fceaa-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="fceaa-115">$orderby</span></span>|<span data-ttu-id="fceaa-116">string</span><span class="sxs-lookup"><span data-stu-id="fceaa-116">string</span></span>|<span data-ttu-id="fceaa-p102">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p102">By default the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>|
|<span data-ttu-id="fceaa-119">$search</span><span class="sxs-lookup"><span data-stu-id="fceaa-119">$search</span></span>|<span data-ttu-id="fceaa-120">string</span><span class="sxs-lookup"><span data-stu-id="fceaa-120">string</span></span>|<span data-ttu-id="fceaa-p103">名またはエイリアスで人物を検索します。ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="fceaa-123">$select</span><span class="sxs-lookup"><span data-stu-id="fceaa-123">$select</span></span>|<span data-ttu-id="fceaa-124">string</span><span class="sxs-lookup"><span data-stu-id="fceaa-124">string</span></span>|<span data-ttu-id="fceaa-p104">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="fceaa-127">$skip</span><span class="sxs-lookup"><span data-stu-id="fceaa-127">$skip</span></span>|<span data-ttu-id="fceaa-128">int</span><span class="sxs-lookup"><span data-stu-id="fceaa-128">int</span></span>|<span data-ttu-id="fceaa-p105">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="fceaa-131">$top</span><span class="sxs-lookup"><span data-stu-id="fceaa-131">$top</span></span>|<span data-ttu-id="fceaa-132">int</span><span class="sxs-lookup"><span data-stu-id="fceaa-132">int</span></span>|<span data-ttu-id="fceaa-133">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="fceaa-133">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="fceaa-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fceaa-134">Parameters</span></span>
| <span data-ttu-id="fceaa-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fceaa-135">Parameter</span></span> |<span data-ttu-id="fceaa-136">型</span><span class="sxs-lookup"><span data-stu-id="fceaa-136">Type</span></span>       |<span data-ttu-id="fceaa-137">説明</span><span class="sxs-lookup"><span data-stu-id="fceaa-137">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="fceaa-138">property_value</span><span class="sxs-lookup"><span data-stu-id="fceaa-138">property_value</span></span>|<span data-ttu-id="fceaa-139">文字列</span><span class="sxs-lookup"><span data-stu-id="fceaa-139">String</span></span>     |<span data-ttu-id="fceaa-p106">照合する拡張プロパティの値。「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p106">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|
|<span data-ttu-id="fceaa-142">person_property</span><span class="sxs-lookup"><span data-stu-id="fceaa-142">person_property</span></span>|<span data-ttu-id="fceaa-143">String</span><span class="sxs-lookup"><span data-stu-id="fceaa-143">String</span></span>    |<span data-ttu-id="fceaa-p107">一致させるユーザーのプロパティ。「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p107">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fceaa-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fceaa-146">Request headers</span></span>
| <span data-ttu-id="fceaa-147">名前</span><span class="sxs-lookup"><span data-stu-id="fceaa-147">Name</span></span>      |<span data-ttu-id="fceaa-148">説明</span><span class="sxs-lookup"><span data-stu-id="fceaa-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fceaa-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="fceaa-149">Authorization</span></span>  | <span data-ttu-id="fceaa-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fceaa-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="fceaa-152">Request body</span></span>
<span data-ttu-id="fceaa-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fceaa-153">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fceaa-154">応答</span><span class="sxs-lookup"><span data-stu-id="fceaa-154">Response</span></span>
<span data-ttu-id="fceaa-p109">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトを返します。応答には、1 つの人物インスタンスまたは人物インスタンスのコレクションを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p109">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="fceaa-157">例</span><span class="sxs-lookup"><span data-stu-id="fceaa-157">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="fceaa-158">検索を実行する</span><span class="sxs-lookup"><span data-stu-id="fceaa-158">Perform a search</span></span> 
<span data-ttu-id="fceaa-159">次に示す要求では、「Irene McGowan」という名前の人物について検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fceaa-159">The following request does a search for a person named "Hermaini Hall."</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="fceaa-160">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fceaa-160">The following example shows the response from the server with the search results.</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="fceaa-161">フィルター処理された応答で返されるフィールドを選択する</span><span class="sxs-lookup"><span data-stu-id="fceaa-161">Selecting the fields to return in a filtered response</span></span> 
<span data-ttu-id="fceaa-162">*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="fceaa-162">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="fceaa-p110">次の例では、指定した名前と等しい表示名を持つ人物の **displayName** と **scoredEmailAddresses** を取得します。この例では、表示名が "Lorrie Frye" と等しい人物のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="fceaa-p110">The following example gets the **DisplayName** and **EmailAddress** of people whose display name equals the specified name. In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="fceaa-165">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fceaa-165">The following example shows the response from the server with the search results.</span></span> 

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
