# <a name="range-entirerow"></a><span data-ttu-id="dd40c-101">範囲:EntireRow</span><span class="sxs-lookup"><span data-stu-id="dd40c-101">Range: EntireRow</span></span>

<span data-ttu-id="dd40c-102">範囲に含まれるすべての行を表すオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="dd40c-102">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd40c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dd40c-103">Permissions</span></span>
<span data-ttu-id="dd40c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd40c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd40c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd40c-106">Permission type</span></span>      | <span data-ttu-id="dd40c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd40c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd40c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd40c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dd40c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd40c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd40c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd40c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd40c-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd40c-111">Not supported.</span></span>    |
|<span data-ttu-id="dd40c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd40c-112">Application</span></span> | <span data-ttu-id="dd40c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd40c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd40c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd40c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/EntireRow
GET /workbook/worksheets/{id|name}/range(<address>)/EntireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireRow

```
## <a name="request-headers"></a><span data-ttu-id="dd40c-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd40c-115">Request headers</span></span>
| <span data-ttu-id="dd40c-116">名前</span><span class="sxs-lookup"><span data-stu-id="dd40c-116">Name</span></span>       | <span data-ttu-id="dd40c-117">説明</span><span class="sxs-lookup"><span data-stu-id="dd40c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd40c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd40c-118">Authorization</span></span>  | <span data-ttu-id="dd40c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dd40c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd40c-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd40c-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dd40c-122">応答</span><span class="sxs-lookup"><span data-stu-id="dd40c-122">Response</span></span>

<span data-ttu-id="dd40c-123">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dd40c-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd40c-124">例</span><span class="sxs-lookup"><span data-stu-id="dd40c-124">Example</span></span>
<span data-ttu-id="dd40c-125">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dd40c-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd40c-126">要求</span><span class="sxs-lookup"><span data-stu-id="dd40c-126">Request</span></span>
<span data-ttu-id="dd40c-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dd40c-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/EntireRow
```

##### <a name="response"></a><span data-ttu-id="dd40c-128">応答</span><span class="sxs-lookup"><span data-stu-id="dd40c-128">Response</span></span>
<span data-ttu-id="dd40c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dd40c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->