# <a name="range-merge"></a><span data-ttu-id="ded90-101">範囲: マージ</span><span class="sxs-lookup"><span data-stu-id="ded90-101">Range: merge</span></span>

<span data-ttu-id="ded90-102">範囲内のセルをワークシートの 1 つの領域にマージします。</span><span class="sxs-lookup"><span data-stu-id="ded90-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="ded90-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ded90-103">Permissions</span></span>
<span data-ttu-id="ded90-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ded90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ded90-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ded90-106">Permission type</span></span>      | <span data-ttu-id="ded90-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ded90-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ded90-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ded90-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ded90-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ded90-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ded90-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ded90-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ded90-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ded90-111">Not supported.</span></span>    |
|<span data-ttu-id="ded90-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ded90-112">Application</span></span> | <span data-ttu-id="ded90-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ded90-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ded90-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ded90-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="ded90-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ded90-115">Request headers</span></span>
| <span data-ttu-id="ded90-116">名前</span><span class="sxs-lookup"><span data-stu-id="ded90-116">Name</span></span>       | <span data-ttu-id="ded90-117">説明</span><span class="sxs-lookup"><span data-stu-id="ded90-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ded90-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ded90-118">Authorization</span></span>  | <span data-ttu-id="ded90-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ded90-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ded90-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="ded90-121">Request body</span></span>
<span data-ttu-id="ded90-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ded90-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ded90-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ded90-123">Parameter</span></span>    | <span data-ttu-id="ded90-124">型</span><span class="sxs-lookup"><span data-stu-id="ded90-124">Type</span></span>   |<span data-ttu-id="ded90-125">説明</span><span class="sxs-lookup"><span data-stu-id="ded90-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ded90-126">across</span><span class="sxs-lookup"><span data-stu-id="ded90-126">across</span></span>|<span data-ttu-id="ded90-127">boolean</span><span class="sxs-lookup"><span data-stu-id="ded90-127">boolean</span></span>|<span data-ttu-id="ded90-p103">省略可能。指定した範囲のセルを行ごとに結合して、行ごとに別のセルを作成する場合は True に設定します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="ded90-p103">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ded90-131">応答</span><span class="sxs-lookup"><span data-stu-id="ded90-131">Response</span></span>

<span data-ttu-id="ded90-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ded90-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ded90-134">例</span><span class="sxs-lookup"><span data-stu-id="ded90-134">Example</span></span>
<span data-ttu-id="ded90-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ded90-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ded90-136">要求</span><span class="sxs-lookup"><span data-stu-id="ded90-136">Request</span></span>
<span data-ttu-id="ded90-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ded90-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="ded90-138">応答</span><span class="sxs-lookup"><span data-stu-id="ded90-138">Response</span></span>
<span data-ttu-id="ded90-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ded90-139">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->