# <a name="nameditem-range"></a><span data-ttu-id="ab24e-101">NamedItem:Range</span><span class="sxs-lookup"><span data-stu-id="ab24e-101">NamedItem: Range</span></span>

<span data-ttu-id="ab24e-p101">名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。</span><span class="sxs-lookup"><span data-stu-id="ab24e-p101">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab24e-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab24e-104">Permissions</span></span>
<span data-ttu-id="ab24e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab24e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab24e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab24e-107">Permission type</span></span>      | <span data-ttu-id="ab24e-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab24e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab24e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab24e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ab24e-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab24e-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab24e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab24e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab24e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab24e-112">Not supported.</span></span>    |
|<span data-ttu-id="ab24e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab24e-113">Application</span></span> | <span data-ttu-id="ab24e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab24e-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab24e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab24e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="ab24e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab24e-116">Request headers</span></span>
| <span data-ttu-id="ab24e-117">名前</span><span class="sxs-lookup"><span data-stu-id="ab24e-117">Name</span></span>       | <span data-ttu-id="ab24e-118">説明</span><span class="sxs-lookup"><span data-stu-id="ab24e-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab24e-119">承認</span><span class="sxs-lookup"><span data-stu-id="ab24e-119">Authorization</span></span>  | <span data-ttu-id="ab24e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab24e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab24e-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ab24e-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="ab24e-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ab24e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab24e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab24e-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ab24e-126">応答</span><span class="sxs-lookup"><span data-stu-id="ab24e-126">Response</span></span>

<span data-ttu-id="ab24e-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab24e-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab24e-128">例</span><span class="sxs-lookup"><span data-stu-id="ab24e-128">Example</span></span>
<span data-ttu-id="ab24e-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ab24e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab24e-130">要求</span><span class="sxs-lookup"><span data-stu-id="ab24e-130">Request</span></span>
<span data-ttu-id="ab24e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab24e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="ab24e-132">応答</span><span class="sxs-lookup"><span data-stu-id="ab24e-132">Response</span></span>
<span data-ttu-id="ab24e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab24e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->