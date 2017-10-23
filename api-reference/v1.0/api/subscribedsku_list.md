# <a name="list-subscribedskus"></a><span data-ttu-id="65d57-101">subscribedSkus を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="65d57-101">List subscribedSkus</span></span>
<span data-ttu-id="65d57-102">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="65d57-102">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="65d57-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65d57-103">Permissions</span></span>
<span data-ttu-id="65d57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="65d57-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65d57-106">Permission type</span></span>      | <span data-ttu-id="65d57-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65d57-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65d57-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65d57-108">Delegated (work or school account)</span></span> | <span data-ttu-id="65d57-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65d57-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65d57-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65d57-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d57-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d57-111">Not supported.</span></span>    |
|<span data-ttu-id="65d57-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65d57-112">Application</span></span> | <span data-ttu-id="65d57-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d57-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65d57-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65d57-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65d57-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65d57-115">Optional query parameters</span></span>
<span data-ttu-id="65d57-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="65d57-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="65d57-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65d57-117">Request headers</span></span>
| <span data-ttu-id="65d57-118">名前</span><span class="sxs-lookup"><span data-stu-id="65d57-118">Name</span></span>       | <span data-ttu-id="65d57-119">型</span><span class="sxs-lookup"><span data-stu-id="65d57-119">Type</span></span> | <span data-ttu-id="65d57-120">説明</span><span class="sxs-lookup"><span data-stu-id="65d57-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65d57-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d57-121">Authorization</span></span>  | <span data-ttu-id="65d57-122">string</span><span class="sxs-lookup"><span data-stu-id="65d57-122">string</span></span>  | <span data-ttu-id="65d57-p102">Bearer &lt;token&gt;。*必須*</span><span class="sxs-lookup"><span data-stu-id="65d57-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="65d57-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="65d57-125">Request body</span></span>
<span data-ttu-id="65d57-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65d57-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d57-127">応答</span><span class="sxs-lookup"><span data-stu-id="65d57-127">Response</span></span>

<span data-ttu-id="65d57-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscribedSku](../resources/subscribedsku.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="65d57-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65d57-129">例</span><span class="sxs-lookup"><span data-stu-id="65d57-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65d57-130">要求</span><span class="sxs-lookup"><span data-stu-id="65d57-130">Request</span></span>
<span data-ttu-id="65d57-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65d57-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="65d57-132">応答</span><span class="sxs-lookup"><span data-stu-id="65d57-132">Response</span></span>
<span data-ttu-id="65d57-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65d57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
            "capabilityStatus": "Enabled",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
            "prepaidUnits": {
                "enabled": 25,
                "suspended": 0,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
                    "servicePlanName": "ADALLOM_S_O365",
                    "provisioningStatus": "Success",
                    "appliesTo": "User"
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
