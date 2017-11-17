# <a name="chart-setdata"></a><span data-ttu-id="9404b-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="9404b-101">Chart: setData</span></span>

<span data-ttu-id="9404b-102">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="9404b-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="9404b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9404b-103">Permissions</span></span>
<span data-ttu-id="9404b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9404b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9404b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9404b-106">Permission type</span></span>      | <span data-ttu-id="9404b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9404b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9404b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9404b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9404b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9404b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9404b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9404b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9404b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9404b-111">Not supported.</span></span>    |
|<span data-ttu-id="9404b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9404b-112">Application</span></span> | <span data-ttu-id="9404b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9404b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9404b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9404b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="9404b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9404b-115">Request headers</span></span>
| <span data-ttu-id="9404b-116">名前</span><span class="sxs-lookup"><span data-stu-id="9404b-116">Name</span></span>       | <span data-ttu-id="9404b-117">説明</span><span class="sxs-lookup"><span data-stu-id="9404b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9404b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9404b-118">Authorization</span></span>  | <span data-ttu-id="9404b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9404b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9404b-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="9404b-121">Request body</span></span>
<span data-ttu-id="9404b-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9404b-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9404b-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9404b-123">Parameter</span></span>    | <span data-ttu-id="9404b-124">型</span><span class="sxs-lookup"><span data-stu-id="9404b-124">Type</span></span>   |<span data-ttu-id="9404b-125">説明</span><span class="sxs-lookup"><span data-stu-id="9404b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9404b-126">sourceData</span><span class="sxs-lookup"><span data-stu-id="9404b-126">sourceData</span></span>|<span data-ttu-id="9404b-127">string</span><span class="sxs-lookup"><span data-stu-id="9404b-127">string</span></span>|<span data-ttu-id="9404b-128">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9404b-128">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="9404b-129">seriesBy</span><span class="sxs-lookup"><span data-stu-id="9404b-129">seriesBy</span></span>|<span data-ttu-id="9404b-130">string</span><span class="sxs-lookup"><span data-stu-id="9404b-130">string</span></span>|<span data-ttu-id="9404b-p103">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。次のいずれかを指定できます。自動 (既定)、行、列。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="9404b-p103">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="9404b-135">応答</span><span class="sxs-lookup"><span data-stu-id="9404b-135">Response</span></span>

<span data-ttu-id="9404b-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9404b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9404b-138">例</span><span class="sxs-lookup"><span data-stu-id="9404b-138">Example</span></span>
<span data-ttu-id="9404b-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9404b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9404b-140">要求</span><span class="sxs-lookup"><span data-stu-id="9404b-140">Request</span></span>
<span data-ttu-id="9404b-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9404b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="9404b-142">応答</span><span class="sxs-lookup"><span data-stu-id="9404b-142">Response</span></span>
<span data-ttu-id="9404b-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9404b-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->