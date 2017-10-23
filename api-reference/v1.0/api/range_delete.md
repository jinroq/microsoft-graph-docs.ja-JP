# <a name="range-delete"></a><span data-ttu-id="ae516-101">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="ae516-101">Range: delete</span></span>

<span data-ttu-id="ae516-102">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="ae516-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae516-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae516-103">Permissions</span></span>
<span data-ttu-id="ae516-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae516-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae516-106">Permission type</span></span>      | <span data-ttu-id="ae516-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae516-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae516-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae516-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae516-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae516-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae516-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae516-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae516-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae516-111">Not supported.</span></span>    |
|<span data-ttu-id="ae516-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae516-112">Application</span></span> | <span data-ttu-id="ae516-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae516-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae516-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae516-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="ae516-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae516-115">Request headers</span></span>
| <span data-ttu-id="ae516-116">名前</span><span class="sxs-lookup"><span data-stu-id="ae516-116">Name</span></span>       | <span data-ttu-id="ae516-117">説明</span><span class="sxs-lookup"><span data-stu-id="ae516-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae516-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae516-118">Authorization</span></span>  | <span data-ttu-id="ae516-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae516-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae516-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae516-121">Request body</span></span>
<span data-ttu-id="ae516-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae516-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae516-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae516-123">Parameter</span></span>    | <span data-ttu-id="ae516-124">型</span><span class="sxs-lookup"><span data-stu-id="ae516-124">Type</span></span>   |<span data-ttu-id="ae516-125">説明</span><span class="sxs-lookup"><span data-stu-id="ae516-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae516-126"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="ae516-126">shift</span></span>|<span data-ttu-id="ae516-127">string</span><span class="sxs-lookup"><span data-stu-id="ae516-127">string</span></span>|<span data-ttu-id="ae516-p103">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="ae516-p103">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="ae516-130">応答</span><span class="sxs-lookup"><span data-stu-id="ae516-130">Response</span></span>

<span data-ttu-id="ae516-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ae516-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae516-133">例</span><span class="sxs-lookup"><span data-stu-id="ae516-133">Example</span></span>
<span data-ttu-id="ae516-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ae516-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae516-135">要求</span><span class="sxs-lookup"><span data-stu-id="ae516-135">Request</span></span>
<span data-ttu-id="ae516-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae516-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="ae516-137">応答</span><span class="sxs-lookup"><span data-stu-id="ae516-137">Response</span></span>
<span data-ttu-id="ae516-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ae516-138">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->