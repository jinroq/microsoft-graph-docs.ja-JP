# <a name="chart-setposition"></a><span data-ttu-id="24185-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="24185-101">Chart: setPosition</span></span>

<span data-ttu-id="24185-102">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="24185-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="24185-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24185-103">Permissions</span></span>
<span data-ttu-id="24185-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24185-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24185-106">Permission type</span></span>      | <span data-ttu-id="24185-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24185-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24185-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24185-108">Delegated (work or school account)</span></span> | <span data-ttu-id="24185-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24185-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24185-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24185-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24185-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24185-111">Not supported.</span></span>    |
|<span data-ttu-id="24185-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24185-112">Application</span></span> | <span data-ttu-id="24185-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24185-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24185-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24185-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="24185-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24185-115">Request headers</span></span>
| <span data-ttu-id="24185-116">名前</span><span class="sxs-lookup"><span data-stu-id="24185-116">Name</span></span>       | <span data-ttu-id="24185-117">説明</span><span class="sxs-lookup"><span data-stu-id="24185-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24185-118">承認</span><span class="sxs-lookup"><span data-stu-id="24185-118">Authorization</span></span>  | <span data-ttu-id="24185-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24185-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24185-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24185-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="24185-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="24185-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24185-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="24185-124">Request body</span></span>
<span data-ttu-id="24185-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="24185-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24185-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="24185-126">Parameter</span></span>    | <span data-ttu-id="24185-127">型</span><span class="sxs-lookup"><span data-stu-id="24185-127">Type</span></span>   |<span data-ttu-id="24185-128">説明</span><span class="sxs-lookup"><span data-stu-id="24185-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24185-129">startCell</span><span class="sxs-lookup"><span data-stu-id="24185-129">startCell</span></span>|<span data-ttu-id="24185-130">Json</span><span class="sxs-lookup"><span data-stu-id="24185-130">Json</span></span>|<span data-ttu-id="24185-p104">開始セル。これは、グラフの移動先です。開始セルは、ユーザーの右から左への表示の設定に応じて、左上のセルか、右上のセルとなります。</span><span class="sxs-lookup"><span data-stu-id="24185-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="24185-134">endCell</span><span class="sxs-lookup"><span data-stu-id="24185-134">endCell</span></span>|<span data-ttu-id="24185-135">Json</span><span class="sxs-lookup"><span data-stu-id="24185-135">Json</span></span>|<span data-ttu-id="24185-p105">オプション。終了セル。指定されている場合、グラフの幅と高さは、このセルまたは範囲を完全にカバーするように設定されます。</span><span class="sxs-lookup"><span data-stu-id="24185-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="24185-139">応答</span><span class="sxs-lookup"><span data-stu-id="24185-139">Response</span></span>

<span data-ttu-id="24185-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="24185-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24185-142">例</span><span class="sxs-lookup"><span data-stu-id="24185-142">Example</span></span>
<span data-ttu-id="24185-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="24185-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24185-144">要求</span><span class="sxs-lookup"><span data-stu-id="24185-144">Request</span></span>
<span data-ttu-id="24185-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24185-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="24185-146">応答</span><span class="sxs-lookup"><span data-stu-id="24185-146">Response</span></span>
<span data-ttu-id="24185-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="24185-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->