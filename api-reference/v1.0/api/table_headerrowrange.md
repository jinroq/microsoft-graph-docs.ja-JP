# <a name="table-headerrowrange"></a><span data-ttu-id="7310c-101">Table:HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="7310c-101">Table: HeaderRowRange</span></span>

<span data-ttu-id="7310c-102">テーブルのヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="7310c-102">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7310c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7310c-103">Permissions</span></span>
<span data-ttu-id="7310c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7310c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7310c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7310c-106">Permission type</span></span>      | <span data-ttu-id="7310c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7310c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7310c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7310c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7310c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7310c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7310c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7310c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7310c-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7310c-111">Not supported.</span></span>    |
|<span data-ttu-id="7310c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7310c-112">Application</span></span> | <span data-ttu-id="7310c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7310c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7310c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7310c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="7310c-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7310c-115">Request headers</span></span>
| <span data-ttu-id="7310c-116">名前</span><span class="sxs-lookup"><span data-stu-id="7310c-116">Name</span></span>       | <span data-ttu-id="7310c-117">説明</span><span class="sxs-lookup"><span data-stu-id="7310c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7310c-118">承認</span><span class="sxs-lookup"><span data-stu-id="7310c-118">Authorization</span></span>  | <span data-ttu-id="7310c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7310c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7310c-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7310c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="7310c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7310c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7310c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7310c-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7310c-125">応答</span><span class="sxs-lookup"><span data-stu-id="7310c-125">Response</span></span>

<span data-ttu-id="7310c-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7310c-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7310c-127">例</span><span class="sxs-lookup"><span data-stu-id="7310c-127">Example</span></span>
<span data-ttu-id="7310c-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7310c-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7310c-129">要求</span><span class="sxs-lookup"><span data-stu-id="7310c-129">Request</span></span>
<span data-ttu-id="7310c-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7310c-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="7310c-131">応答</span><span class="sxs-lookup"><span data-stu-id="7310c-131">Response</span></span>
<span data-ttu-id="7310c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7310c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->