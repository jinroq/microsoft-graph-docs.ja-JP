# <a name="get-person"></a><span data-ttu-id="c860e-101">人物を取得する</span><span class="sxs-lookup"><span data-stu-id="c860e-101">Get person</span></span>

<span data-ttu-id="c860e-102">[person](../resources/person.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c860e-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="c860e-p101">この情報は、People API 経由で取得できます。例については、「[例](#examples)」セクションと記事「[人の関連情報を取得する](../../../concepts/people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c860e-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c860e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c860e-105">Permissions</span></span>
<span data-ttu-id="c860e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c860e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c860e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c860e-108">Permission type</span></span>      | <span data-ttu-id="c860e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c860e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c860e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c860e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c860e-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="c860e-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="c860e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c860e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c860e-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="c860e-113">People.Read</span></span>    |
|<span data-ttu-id="c860e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c860e-114">Application</span></span> | <span data-ttu-id="c860e-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="c860e-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c860e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c860e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/{id}
GET /users/{id | userPrincipalName}/people/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c860e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c860e-117">Optional query parameters</span></span>
<span data-ttu-id="c860e-118">このメソッドでは、「[ユーザーの関連情報を取得する](../../../concepts/people_example.md)」の記事に示す例のように、[OData クエリ パラメーター](../../../concepts/query_parameters.md)を使用して応答をカスタマイズすることができます。</span><span class="sxs-lookup"><span data-stu-id="c860e-118">This method supports the following [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, with examples shown in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="c860e-119">名前</span><span class="sxs-lookup"><span data-stu-id="c860e-119">Name</span></span>|<span data-ttu-id="c860e-120">値</span><span class="sxs-lookup"><span data-stu-id="c860e-120">Value</span></span>|<span data-ttu-id="c860e-121">説明</span><span class="sxs-lookup"><span data-stu-id="c860e-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="c860e-122">$filter</span><span class="sxs-lookup"><span data-stu-id="c860e-122">$filter</span></span>|<span data-ttu-id="c860e-123">string</span><span class="sxs-lookup"><span data-stu-id="c860e-123">string</span></span>|<span data-ttu-id="c860e-124">応答を、指定した条件に等しいレコードを持つ人物のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="c860e-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="c860e-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="c860e-125">$orderby</span></span>|<span data-ttu-id="c860e-126">string</span><span class="sxs-lookup"><span data-stu-id="c860e-126">string</span></span>|<span data-ttu-id="c860e-127">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="c860e-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="c860e-128">応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="c860e-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="c860e-129">$search</span><span class="sxs-lookup"><span data-stu-id="c860e-129">$search</span></span>|<span data-ttu-id="c860e-130">string</span><span class="sxs-lookup"><span data-stu-id="c860e-130">string</span></span>|<span data-ttu-id="c860e-131">名またはエイリアスで人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="c860e-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="c860e-132">ファジー マッチをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c860e-132">Supports Fuzzy matching.</span></span>| 
|<span data-ttu-id="c860e-133">$select</span><span class="sxs-lookup"><span data-stu-id="c860e-133">$select</span></span>|<span data-ttu-id="c860e-134">string</span><span class="sxs-lookup"><span data-stu-id="c860e-134">string</span></span>|<span data-ttu-id="c860e-p105">応答に含めるプロパティを示すコンマ区切りのリスト。最適なパフォーマンスを得るには、必要なプロパティのサブセットのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="c860e-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="c860e-137">$skip</span><span class="sxs-lookup"><span data-stu-id="c860e-137">$skip</span></span>|<span data-ttu-id="c860e-138">int</span><span class="sxs-lookup"><span data-stu-id="c860e-138">int</span></span>|<span data-ttu-id="c860e-p106">最初の n 個の結果をスキップします。これはページングに役立ちます。これは *$search* の使用時にはサポートされません。</span><span class="sxs-lookup"><span data-stu-id="c860e-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="c860e-141">$top</span><span class="sxs-lookup"><span data-stu-id="c860e-141">$top</span></span>|<span data-ttu-id="c860e-142">int</span><span class="sxs-lookup"><span data-stu-id="c860e-142">int</span></span>|<span data-ttu-id="c860e-143">返される結果の数。</span><span class="sxs-lookup"><span data-stu-id="c860e-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="c860e-144">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c860e-144">Request headers</span></span>
| <span data-ttu-id="c860e-145">名前</span><span class="sxs-lookup"><span data-stu-id="c860e-145">Name</span></span>      |<span data-ttu-id="c860e-146">説明</span><span class="sxs-lookup"><span data-stu-id="c860e-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c860e-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="c860e-147">Authorization</span></span>  | <span data-ttu-id="c860e-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c860e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c860e-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="c860e-150">Request body</span></span>
<span data-ttu-id="c860e-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c860e-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c860e-152">応答</span><span class="sxs-lookup"><span data-stu-id="c860e-152">Response</span></span>
<span data-ttu-id="c860e-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [person](../resources/person.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c860e-153">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/person.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c860e-154">例</span><span class="sxs-lookup"><span data-stu-id="c860e-154">Examples</span></span>
#### <a name="request-1"></a><span data-ttu-id="c860e-155">要求 1</span><span class="sxs-lookup"><span data-stu-id="c860e-155">Request 1</span></span>
<span data-ttu-id="c860e-156">次に、ユーザーの組織内で対象 ID を持つ人物を取得する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="c860e-156">The following is an example of the request that gets the person who has this ID in the user's organization.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person_by_id"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85
```

#### <a name="response-1"></a><span data-ttu-id="c860e-157">応答 1</span><span class="sxs-lookup"><span data-stu-id="c860e-157">Response 1</span></span>
<span data-ttu-id="c860e-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c860e-158">The following is an example of a response.</span></span>

><span data-ttu-id="c860e-159">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c860e-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c860e-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c860e-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 629

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
```

#### <a name="request-2"></a><span data-ttu-id="c860e-161">要求 2</span><span class="sxs-lookup"><span data-stu-id="c860e-161">Request 2</span></span>
<span data-ttu-id="c860e-162">次に、ユーザーの組織内で対象 ID を持つ人物を取得し、選択したプロパティに応答を限定する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="c860e-162">The following is an example of the request that gets the person who has this ID in the user's organization and restricts the response to the selected properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_by_id_with_select"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85?$select=displayName
```
#### <a name="response-2"></a><span data-ttu-id="c860e-163">応答 2</span><span class="sxs-lookup"><span data-stu-id="c860e-163">Response 2</span></span>
<span data-ttu-id="c860e-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c860e-164">The following is an example of a response.</span></span>

><span data-ttu-id="c860e-165">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c860e-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c860e-166">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c860e-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id_with_select",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer"
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
