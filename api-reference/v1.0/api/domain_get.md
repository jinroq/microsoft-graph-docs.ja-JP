# <a name="get-domain"></a><span data-ttu-id="4c1e2-101">ドメインを取得する</span><span class="sxs-lookup"><span data-stu-id="4c1e2-101">Get domain</span></span>

<span data-ttu-id="4c1e2-102">ドメイン オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c1e2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c1e2-103">Permissions</span></span>

<span data-ttu-id="4c1e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4c1e2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c1e2-106">Permission type</span></span>      | <span data-ttu-id="4c1e2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c1e2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c1e2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c1e2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4c1e2-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c1e2-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="4c1e2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c1e2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c1e2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-111">Not supported.</span></span>    |
|<span data-ttu-id="4c1e2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c1e2-112">Application</span></span> | <span data-ttu-id="4c1e2-113">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1e2-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c1e2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c1e2-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="4c1e2-115">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-115">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4c1e2-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c1e2-116">Optional query parameters</span></span>

<span data-ttu-id="4c1e2-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c1e2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c1e2-118">Request headers</span></span>

| <span data-ttu-id="4c1e2-119">名前</span><span class="sxs-lookup"><span data-stu-id="4c1e2-119">Name</span></span>      |<span data-ttu-id="4c1e2-120">説明</span><span class="sxs-lookup"><span data-stu-id="4c1e2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c1e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c1e2-121">Authorization</span></span>  | <span data-ttu-id="4c1e2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c1e2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c1e2-124">Content-Type</span></span>  | <span data-ttu-id="4c1e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c1e2-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c1e2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c1e2-126">Request body</span></span>
<span data-ttu-id="4c1e2-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c1e2-128">応答</span><span class="sxs-lookup"><span data-stu-id="4c1e2-128">Response</span></span>

<span data-ttu-id="4c1e2-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-129">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c1e2-130">例</span><span class="sxs-lookup"><span data-stu-id="4c1e2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c1e2-131">要求</span><span class="sxs-lookup"><span data-stu-id="4c1e2-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="4c1e2-132">応答</span><span class="sxs-lookup"><span data-stu-id="4c1e2-132">Response</span></span>
<span data-ttu-id="4c1e2-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c1e2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->