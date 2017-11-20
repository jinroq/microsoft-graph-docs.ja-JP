# <a name="worksheet-range"></a><span data-ttu-id="88bc7-101">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="88bc7-101">Worksheet: Range</span></span>

<span data-ttu-id="88bc7-102">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="88bc7-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="88bc7-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88bc7-103">Permissions</span></span>
<span data-ttu-id="88bc7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88bc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88bc7-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88bc7-106">Permission type</span></span>      | <span data-ttu-id="88bc7-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88bc7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88bc7-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88bc7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="88bc7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88bc7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88bc7-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88bc7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88bc7-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88bc7-111">Not supported.</span></span>    |
|<span data-ttu-id="88bc7-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88bc7-112">Application</span></span> | <span data-ttu-id="88bc7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88bc7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88bc7-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88bc7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="88bc7-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88bc7-115">Request headers</span></span>
| <span data-ttu-id="88bc7-116">名前</span><span class="sxs-lookup"><span data-stu-id="88bc7-116">Name</span></span>       | <span data-ttu-id="88bc7-117">説明</span><span class="sxs-lookup"><span data-stu-id="88bc7-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88bc7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="88bc7-118">Authorization</span></span>  | <span data-ttu-id="88bc7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88bc7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88bc7-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="88bc7-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="88bc7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="88bc7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88bc7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="88bc7-124">Request body</span></span>
<span data-ttu-id="88bc7-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="88bc7-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="88bc7-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="88bc7-126">Parameter</span></span>    | <span data-ttu-id="88bc7-127">型</span><span class="sxs-lookup"><span data-stu-id="88bc7-127">Type</span></span>   |<span data-ttu-id="88bc7-128">説明</span><span class="sxs-lookup"><span data-stu-id="88bc7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88bc7-129">address</span><span class="sxs-lookup"><span data-stu-id="88bc7-129">address</span></span>|<span data-ttu-id="88bc7-130">string</span><span class="sxs-lookup"><span data-stu-id="88bc7-130">string</span></span>|<span data-ttu-id="88bc7-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="88bc7-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="88bc7-134">応答</span><span class="sxs-lookup"><span data-stu-id="88bc7-134">Response</span></span>

<span data-ttu-id="88bc7-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88bc7-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88bc7-136">例</span><span class="sxs-lookup"><span data-stu-id="88bc7-136">Example</span></span>
<span data-ttu-id="88bc7-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="88bc7-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88bc7-138">要求</span><span class="sxs-lookup"><span data-stu-id="88bc7-138">Request</span></span>
<span data-ttu-id="88bc7-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88bc7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="88bc7-140">応答</span><span class="sxs-lookup"><span data-stu-id="88bc7-140">Response</span></span>
<span data-ttu-id="88bc7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88bc7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->