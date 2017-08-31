# <a name="range-lastrow"></a><span data-ttu-id="5b3a4-101">範囲:LastRow</span><span class="sxs-lookup"><span data-stu-id="5b3a4-101">Range: LastRow</span></span>

<span data-ttu-id="5b3a4-p101">範囲内の最後の行を取得します。たとえば、"B2:D5" の最後の行は "B5:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="5b3a4-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b3a4-104">Permissions</span></span>
<span data-ttu-id="5b3a4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b3a4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b3a4-107">Permission type</span></span>      | <span data-ttu-id="5b3a4-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b3a4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b3a4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b3a4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5b3a4-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b3a4-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5b3a4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b3a4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b3a4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-112">Not supported.</span></span>    |
|<span data-ttu-id="5b3a4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b3a4-113">Application</span></span> | <span data-ttu-id="5b3a4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b3a4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b3a4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(<address>)/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="5b3a4-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b3a4-116">Request headers</span></span>
| <span data-ttu-id="5b3a4-117">名前</span><span class="sxs-lookup"><span data-stu-id="5b3a4-117">Name</span></span>       | <span data-ttu-id="5b3a4-118">説明</span><span class="sxs-lookup"><span data-stu-id="5b3a4-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5b3a4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b3a4-119">Authorization</span></span>  | <span data-ttu-id="5b3a4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b3a4-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b3a4-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5b3a4-123">応答</span><span class="sxs-lookup"><span data-stu-id="5b3a4-123">Response</span></span>

<span data-ttu-id="5b3a4-124">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b3a4-125">例</span><span class="sxs-lookup"><span data-stu-id="5b3a4-125">Example</span></span>
<span data-ttu-id="5b3a4-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5b3a4-127">要求</span><span class="sxs-lookup"><span data-stu-id="5b3a4-127">Request</span></span>
<span data-ttu-id="5b3a4-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="5b3a4-129">応答</span><span class="sxs-lookup"><span data-stu-id="5b3a4-129">Response</span></span>
<span data-ttu-id="5b3a4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b3a4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->