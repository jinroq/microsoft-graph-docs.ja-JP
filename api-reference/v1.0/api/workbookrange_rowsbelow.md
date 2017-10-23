# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="3a2db-101">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="3a2db-101">workbookRange: rowsBelow</span></span>

<span data-ttu-id="3a2db-102">指定した範囲の下にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a2db-102">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a2db-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a2db-103">Permissions</span></span>
<span data-ttu-id="3a2db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a2db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a2db-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a2db-106">Permission type</span></span>      | <span data-ttu-id="3a2db-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a2db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a2db-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a2db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3a2db-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2db-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a2db-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a2db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a2db-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a2db-111">Not supported.</span></span>    |
|<span data-ttu-id="3a2db-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a2db-112">Application</span></span> | <span data-ttu-id="3a2db-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a2db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a2db-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a2db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="3a2db-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a2db-115">Request headers</span></span>
| <span data-ttu-id="3a2db-116">名前</span><span class="sxs-lookup"><span data-stu-id="3a2db-116">Name</span></span>       | <span data-ttu-id="3a2db-117">説明</span><span class="sxs-lookup"><span data-stu-id="3a2db-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a2db-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a2db-118">Authorization</span></span>  | <span data-ttu-id="3a2db-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a2db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a2db-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a2db-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a2db-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3a2db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="3a2db-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a2db-124">Parameters</span></span>

| <span data-ttu-id="3a2db-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a2db-125">Parameter</span></span>    | <span data-ttu-id="3a2db-126">型</span><span class="sxs-lookup"><span data-stu-id="3a2db-126">Type</span></span>   |<span data-ttu-id="3a2db-127">説明</span><span class="sxs-lookup"><span data-stu-id="3a2db-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a2db-128">count</span><span class="sxs-lookup"><span data-stu-id="3a2db-128">count</span></span>|<span data-ttu-id="3a2db-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3a2db-129">Int32</span></span>|<span data-ttu-id="3a2db-p104">結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です</span><span class="sxs-lookup"><span data-stu-id="3a2db-p104">The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a2db-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a2db-134">Request body</span></span>

### <a name="response"></a><span data-ttu-id="3a2db-135">応答</span><span class="sxs-lookup"><span data-stu-id="3a2db-135">Response</span></span>
<span data-ttu-id="3a2db-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a2db-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a2db-137">例</span><span class="sxs-lookup"><span data-stu-id="3a2db-137">Example</span></span>
<span data-ttu-id="3a2db-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3a2db-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a2db-139">要求</span><span class="sxs-lookup"><span data-stu-id="3a2db-139">Request</span></span>
<span data-ttu-id="3a2db-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a2db-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="3a2db-141">応答</span><span class="sxs-lookup"><span data-stu-id="3a2db-141">Response</span></span>
<span data-ttu-id="3a2db-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a2db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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