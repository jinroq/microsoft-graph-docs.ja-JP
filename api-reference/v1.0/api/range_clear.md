# <a name="range-clear"></a><span data-ttu-id="1289a-101">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="1289a-101">Range: clear</span></span>

<span data-ttu-id="1289a-102">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="1289a-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="1289a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1289a-103">Permissions</span></span>
<span data-ttu-id="1289a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1289a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1289a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1289a-106">Permission type</span></span>      | <span data-ttu-id="1289a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1289a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1289a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1289a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1289a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1289a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1289a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1289a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1289a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1289a-111">Not supported.</span></span>    |
|<span data-ttu-id="1289a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1289a-112">Application</span></span> | <span data-ttu-id="1289a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1289a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1289a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1289a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="1289a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1289a-115">Request headers</span></span>
| <span data-ttu-id="1289a-116">名前</span><span class="sxs-lookup"><span data-stu-id="1289a-116">Name</span></span>       | <span data-ttu-id="1289a-117">説明</span><span class="sxs-lookup"><span data-stu-id="1289a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1289a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="1289a-118">Authorization</span></span>  | <span data-ttu-id="1289a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1289a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1289a-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="1289a-121">Request body</span></span>
<span data-ttu-id="1289a-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1289a-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1289a-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1289a-123">Parameter</span></span>    | <span data-ttu-id="1289a-124">型</span><span class="sxs-lookup"><span data-stu-id="1289a-124">Type</span></span>   |<span data-ttu-id="1289a-125">説明</span><span class="sxs-lookup"><span data-stu-id="1289a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1289a-126">applyTo</span><span class="sxs-lookup"><span data-stu-id="1289a-126">applyTo</span></span>|<span data-ttu-id="1289a-127">string</span><span class="sxs-lookup"><span data-stu-id="1289a-127">string</span></span>|<span data-ttu-id="1289a-p103">省略可能。クリア操作の種類を決定します。可能な値は、`All`、`Formats`、`Contents` です。</span><span class="sxs-lookup"><span data-stu-id="1289a-p103">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="1289a-131">応答</span><span class="sxs-lookup"><span data-stu-id="1289a-131">Response</span></span>

<span data-ttu-id="1289a-p104">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1289a-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1289a-134">例</span><span class="sxs-lookup"><span data-stu-id="1289a-134">Example</span></span>
<span data-ttu-id="1289a-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1289a-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1289a-136">要求</span><span class="sxs-lookup"><span data-stu-id="1289a-136">Request</span></span>
<span data-ttu-id="1289a-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1289a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="1289a-138">応答</span><span class="sxs-lookup"><span data-stu-id="1289a-138">Response</span></span>
<span data-ttu-id="1289a-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1289a-139">Here is an example of the response.</span></span> 
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
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->