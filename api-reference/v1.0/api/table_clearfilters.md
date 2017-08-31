# <a name="table-clearfilters"></a><span data-ttu-id="ac320-101">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="ac320-101">Table: clearFilters</span></span>

<span data-ttu-id="ac320-102">現在テーブルに適用されているすべてのフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="ac320-102">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac320-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac320-103">Permissions</span></span>
<span data-ttu-id="ac320-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac320-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac320-106">Permission type</span></span>      | <span data-ttu-id="ac320-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac320-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac320-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac320-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac320-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac320-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ac320-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac320-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac320-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac320-111">Not supported.</span></span>    |
|<span data-ttu-id="ac320-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac320-112">Application</span></span> | <span data-ttu-id="ac320-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac320-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac320-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac320-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="ac320-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac320-115">Request headers</span></span>
| <span data-ttu-id="ac320-116">名前</span><span class="sxs-lookup"><span data-stu-id="ac320-116">Name</span></span>       | <span data-ttu-id="ac320-117">説明</span><span class="sxs-lookup"><span data-stu-id="ac320-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ac320-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac320-118">Authorization</span></span>  | <span data-ttu-id="ac320-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac320-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac320-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac320-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ac320-122">応答</span><span class="sxs-lookup"><span data-stu-id="ac320-122">Response</span></span>

<span data-ttu-id="ac320-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ac320-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac320-125">例</span><span class="sxs-lookup"><span data-stu-id="ac320-125">Example</span></span>
<span data-ttu-id="ac320-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ac320-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac320-127">要求</span><span class="sxs-lookup"><span data-stu-id="ac320-127">Request</span></span>
<span data-ttu-id="ac320-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac320-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="ac320-129">応答</span><span class="sxs-lookup"><span data-stu-id="ac320-129">Response</span></span>
<span data-ttu-id="ac320-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ac320-130">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->