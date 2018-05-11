# <a name="list-organization"></a><span data-ttu-id="44957-101">組織を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="44957-101">List organization</span></span>

> <span data-ttu-id="44957-102">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44957-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44957-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44957-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44957-104">組織オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="44957-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="44957-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44957-105">Permissions</span></span>
<span data-ttu-id="44957-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44957-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44957-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44957-108">Permission type</span></span>      | <span data-ttu-id="44957-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44957-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44957-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="44957-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44957-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44957-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="44957-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44957-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44957-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44957-113">Not supported.</span></span>    |
|<span data-ttu-id="44957-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44957-114">Application</span></span> | <span data-ttu-id="44957-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44957-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="44957-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="44957-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="44957-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="44957-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="44957-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="44957-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="44957-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44957-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44957-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="44957-120">Optional query parameters</span></span>
<span data-ttu-id="44957-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="44957-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44957-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44957-122">Request headers</span></span>
| <span data-ttu-id="44957-123">名前</span><span class="sxs-lookup"><span data-stu-id="44957-123">Name</span></span>       | <span data-ttu-id="44957-124">型</span><span class="sxs-lookup"><span data-stu-id="44957-124">Type</span></span> | <span data-ttu-id="44957-125">説明</span><span class="sxs-lookup"><span data-stu-id="44957-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44957-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="44957-126">Authorization</span></span>  | <span data-ttu-id="44957-127">string</span><span class="sxs-lookup"><span data-stu-id="44957-127">string</span></span>  | <span data-ttu-id="44957-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44957-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44957-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="44957-130">Request body</span></span>
<span data-ttu-id="44957-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44957-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44957-132">応答</span><span class="sxs-lookup"><span data-stu-id="44957-132">Response</span></span>

<span data-ttu-id="44957-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="44957-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44957-134">例</span><span class="sxs-lookup"><span data-stu-id="44957-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44957-135">要求</span><span class="sxs-lookup"><span data-stu-id="44957-135">Request</span></span>
<span data-ttu-id="44957-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44957-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="44957-137">応答</span><span class="sxs-lookup"><span data-stu-id="44957-137">Response</span></span>
<span data-ttu-id="44957-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44957-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->