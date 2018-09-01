# <a name="workbookrange-resizedrange"></a><span data-ttu-id="cc3e7-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="cc3e7-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="cc3e7-102">現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc3e7-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc3e7-103">Permissions</span></span>
<span data-ttu-id="cc3e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc3e7-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc3e7-106">Permission type</span></span>      | <span data-ttu-id="cc3e7-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc3e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc3e7-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cc3e7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc3e7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cc3e7-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc3e7-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-111">Not supported.</span></span>    |
|<span data-ttu-id="cc3e7-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc3e7-112">Application</span></span> | <span data-ttu-id="cc3e7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc3e7-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc3e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="cc3e7-115">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc3e7-115">Function parameters</span></span>

| <span data-ttu-id="cc3e7-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc3e7-116">Parameter</span></span>    | <span data-ttu-id="cc3e7-117">型</span><span class="sxs-lookup"><span data-stu-id="cc3e7-117">Type</span></span>   |<span data-ttu-id="cc3e7-118">説明</span><span class="sxs-lookup"><span data-stu-id="cc3e7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc3e7-119">deltaRows</span><span class="sxs-lookup"><span data-stu-id="cc3e7-119">deltaRows</span></span>|<span data-ttu-id="cc3e7-120">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3e7-120">Int32</span></span>|<span data-ttu-id="cc3e7-p102">現在の範囲を基準にして、右下隅を拡張する行の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します</span><span class="sxs-lookup"><span data-stu-id="cc3e7-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="cc3e7-123">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="cc3e7-123">deltaColumns</span></span>|<span data-ttu-id="cc3e7-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3e7-124">Int32</span></span>|<span data-ttu-id="cc3e7-125">現在の範囲を基準にして、右下隅を拡張する列の数です。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-125">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span> <span data-ttu-id="cc3e7-126">範囲を拡張するには正の数値を、縮小するには負の数値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-126">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="cc3e7-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc3e7-127">Request headers</span></span>
| <span data-ttu-id="cc3e7-128">名前</span><span class="sxs-lookup"><span data-stu-id="cc3e7-128">Name</span></span>       | <span data-ttu-id="cc3e7-129">説明</span><span class="sxs-lookup"><span data-stu-id="cc3e7-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc3e7-130">承認</span><span class="sxs-lookup"><span data-stu-id="cc3e7-130">Authorization</span></span>  | <span data-ttu-id="cc3e7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc3e7-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cc3e7-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="cc3e7-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc3e7-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc3e7-136">Request body</span></span>
<span data-ttu-id="cc3e7-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-137">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="cc3e7-138">応答</span><span class="sxs-lookup"><span data-stu-id="cc3e7-138">Response</span></span>
<span data-ttu-id="cc3e7-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3e7-140">例</span><span class="sxs-lookup"><span data-stu-id="cc3e7-140">Example</span></span>
<span data-ttu-id="cc3e7-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc3e7-142">要求</span><span class="sxs-lookup"><span data-stu-id="cc3e7-142">Request</span></span>
<span data-ttu-id="cc3e7-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-143">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="cc3e7-144">応答</span><span class="sxs-lookup"><span data-stu-id="cc3e7-144">Response</span></span>
<span data-ttu-id="cc3e7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc3e7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
