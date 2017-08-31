# <a name="chart-delete"></a><span data-ttu-id="b0680-101">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="b0680-101">Chart: delete</span></span>

<span data-ttu-id="b0680-102">グラフ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b0680-102">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0680-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0680-103">Permissions</span></span>
<span data-ttu-id="b0680-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0680-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0680-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0680-106">Permission type</span></span>      | <span data-ttu-id="b0680-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0680-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0680-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0680-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b0680-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0680-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0680-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0680-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0680-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0680-111">Not supported.</span></span>    |
|<span data-ttu-id="b0680-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0680-112">Application</span></span> | <span data-ttu-id="b0680-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0680-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0680-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0680-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="b0680-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0680-115">Request headers</span></span>
| <span data-ttu-id="b0680-116">名前</span><span class="sxs-lookup"><span data-stu-id="b0680-116">Name</span></span>       | <span data-ttu-id="b0680-117">説明</span><span class="sxs-lookup"><span data-stu-id="b0680-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0680-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0680-118">Authorization</span></span>  | <span data-ttu-id="b0680-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0680-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0680-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0680-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b0680-122">応答</span><span class="sxs-lookup"><span data-stu-id="b0680-122">Response</span></span>

<span data-ttu-id="b0680-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b0680-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0680-125">例</span><span class="sxs-lookup"><span data-stu-id="b0680-125">Example</span></span>
<span data-ttu-id="b0680-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b0680-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0680-127">要求</span><span class="sxs-lookup"><span data-stu-id="b0680-127">Request</span></span>
<span data-ttu-id="b0680-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0680-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/delete
```

##### <a name="response"></a><span data-ttu-id="b0680-129">応答</span><span class="sxs-lookup"><span data-stu-id="b0680-129">Response</span></span>
<span data-ttu-id="b0680-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b0680-130">Here is an example of the response.</span></span> 
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
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->