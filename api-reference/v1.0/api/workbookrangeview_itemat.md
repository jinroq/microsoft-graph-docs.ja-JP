# <a name="workbookrangeview-itemat"></a><span data-ttu-id="48aa5-101">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="48aa5-101">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="48aa5-102">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48aa5-102">Permissions</span></span>
<span data-ttu-id="48aa5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48aa5-105">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48aa5-105">Permission type</span></span>      | <span data-ttu-id="48aa5-106">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48aa5-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48aa5-107">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48aa5-107">Delegated (work or school account)</span></span> | <span data-ttu-id="48aa5-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48aa5-108">Files.ReadWrite</span></span> |
|<span data-ttu-id="48aa5-109">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48aa5-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48aa5-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48aa5-110">Not supported.</span></span>    |
|<span data-ttu-id="48aa5-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48aa5-111">Application</span></span> | <span data-ttu-id="48aa5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48aa5-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48aa5-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48aa5-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="48aa5-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48aa5-114">Request headers</span></span>
| <span data-ttu-id="48aa5-115">名前</span><span class="sxs-lookup"><span data-stu-id="48aa5-115">Name</span></span>       | <span data-ttu-id="48aa5-116">説明</span><span class="sxs-lookup"><span data-stu-id="48aa5-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48aa5-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="48aa5-117">Authorization</span></span>  | <span data-ttu-id="48aa5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48aa5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48aa5-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="48aa5-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="48aa5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="48aa5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48aa5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="48aa5-123">Request body</span></span>
<span data-ttu-id="48aa5-124">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="48aa5-124">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="48aa5-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="48aa5-125">Parameter</span></span>    | <span data-ttu-id="48aa5-126">型</span><span class="sxs-lookup"><span data-stu-id="48aa5-126">Type</span></span>   |<span data-ttu-id="48aa5-127">説明</span><span class="sxs-lookup"><span data-stu-id="48aa5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48aa5-128">index</span><span class="sxs-lookup"><span data-stu-id="48aa5-128">index</span></span>|<span data-ttu-id="48aa5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="48aa5-129">Int32</span></span>|<span data-ttu-id="48aa5-130">返される項目のインデックス。</span><span class="sxs-lookup"><span data-stu-id="48aa5-130">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="48aa5-131">応答</span><span class="sxs-lookup"><span data-stu-id="48aa5-131">Response</span></span>

<span data-ttu-id="48aa5-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48aa5-132">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48aa5-133">例</span><span class="sxs-lookup"><span data-stu-id="48aa5-133">Example</span></span>
<span data-ttu-id="48aa5-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="48aa5-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48aa5-135">要求</span><span class="sxs-lookup"><span data-stu-id="48aa5-135">Request</span></span>
<span data-ttu-id="48aa5-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48aa5-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="48aa5-137">応答</span><span class="sxs-lookup"><span data-stu-id="48aa5-137">Response</span></span>
<span data-ttu-id="48aa5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48aa5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
