# <a name="list-domains"></a><span data-ttu-id="0b3ec-101">ドメインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0b3ec-101">List domains</span></span>

<span data-ttu-id="0b3ec-102">ドメイン オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-102">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b3ec-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b3ec-103">Permissions</span></span>
<span data-ttu-id="0b3ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b3ec-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b3ec-106">Permission type</span></span>      | <span data-ttu-id="0b3ec-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b3ec-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b3ec-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b3ec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0b3ec-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b3ec-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="0b3ec-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b3ec-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b3ec-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-111">Not supported.</span></span>    |
|<span data-ttu-id="0b3ec-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b3ec-112">Application</span></span> | <span data-ttu-id="0b3ec-113">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3ec-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b3ec-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b3ec-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b3ec-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b3ec-115">Optional query parameters</span></span>
<span data-ttu-id="0b3ec-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b3ec-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b3ec-117">Request headers</span></span>
| <span data-ttu-id="0b3ec-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b3ec-118">Name</span></span>      |<span data-ttu-id="0b3ec-119">説明</span><span class="sxs-lookup"><span data-stu-id="0b3ec-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b3ec-120">承認</span><span class="sxs-lookup"><span data-stu-id="0b3ec-120">Authorization</span></span>  | <span data-ttu-id="0b3ec-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0b3ec-123">承諾</span><span class="sxs-lookup"><span data-stu-id="0b3ec-123">Accept</span></span>         | <span data-ttu-id="0b3ec-124">application/json;</span><span class="sxs-lookup"><span data-stu-id="0b3ec-124">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b3ec-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b3ec-125">Request body</span></span>
<span data-ttu-id="0b3ec-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b3ec-127">応答</span><span class="sxs-lookup"><span data-stu-id="0b3ec-127">Response</span></span>

<span data-ttu-id="0b3ec-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domain](../resources/domain.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-128">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b3ec-129">例</span><span class="sxs-lookup"><span data-stu-id="0b3ec-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b3ec-130">要求</span><span class="sxs-lookup"><span data-stu-id="0b3ec-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="0b3ec-131">応答</span><span class="sxs-lookup"><span data-stu-id="0b3ec-131">Response</span></span>
<span data-ttu-id="0b3ec-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b3ec-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->