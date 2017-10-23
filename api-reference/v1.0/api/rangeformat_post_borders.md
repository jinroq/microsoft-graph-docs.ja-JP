# <a name="create-rangeborder"></a><span data-ttu-id="89e6d-101">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="89e6d-101">Create RangeBorder</span></span>

<span data-ttu-id="89e6d-102">この API を使用して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="89e6d-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="89e6d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89e6d-103">Permissions</span></span>
<span data-ttu-id="89e6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89e6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89e6d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89e6d-106">Permission type</span></span>      | <span data-ttu-id="89e6d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89e6d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89e6d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89e6d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="89e6d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89e6d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89e6d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89e6d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e6d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89e6d-111">Not supported.</span></span>    |
|<span data-ttu-id="89e6d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89e6d-112">Application</span></span> | <span data-ttu-id="89e6d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89e6d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e6d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89e6d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="89e6d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89e6d-115">Request headers</span></span>
| <span data-ttu-id="89e6d-116">名前</span><span class="sxs-lookup"><span data-stu-id="89e6d-116">Name</span></span>       | <span data-ttu-id="89e6d-117">説明</span><span class="sxs-lookup"><span data-stu-id="89e6d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89e6d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e6d-118">Authorization</span></span>  | <span data-ttu-id="89e6d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="89e6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89e6d-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="89e6d-121">Request body</span></span>
<span data-ttu-id="89e6d-122">要求本文で、[RangeBorder](../resources/rangeborder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89e6d-122">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89e6d-123">応答</span><span class="sxs-lookup"><span data-stu-id="89e6d-123">Response</span></span>

<span data-ttu-id="89e6d-124">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [RangeBorder](../resources/rangeborder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89e6d-124">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e6d-125">例</span><span class="sxs-lookup"><span data-stu-id="89e6d-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89e6d-126">要求</span><span class="sxs-lookup"><span data-stu-id="89e6d-126">Request</span></span>
<span data-ttu-id="89e6d-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89e6d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="89e6d-128">要求本文で、[RangeBorder](../resources/rangeborder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89e6d-128">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="89e6d-129">応答</span><span class="sxs-lookup"><span data-stu-id="89e6d-129">Response</span></span>
<span data-ttu-id="89e6d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89e6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->