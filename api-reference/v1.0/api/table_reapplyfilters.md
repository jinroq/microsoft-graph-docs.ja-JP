# <a name="table-reapplyfilters"></a><span data-ttu-id="9181b-101">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="9181b-101">Table: reapplyFilters</span></span>

<span data-ttu-id="9181b-102">現在テーブルにあるすべてのフィルターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="9181b-102">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9181b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9181b-103">Permissions</span></span>
<span data-ttu-id="9181b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9181b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9181b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9181b-106">Permission type</span></span>      | <span data-ttu-id="9181b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9181b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9181b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9181b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9181b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9181b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9181b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9181b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9181b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9181b-111">Not supported.</span></span>    |
|<span data-ttu-id="9181b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9181b-112">Application</span></span> | <span data-ttu-id="9181b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9181b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9181b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9181b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="9181b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9181b-115">Request headers</span></span>
| <span data-ttu-id="9181b-116">名前</span><span class="sxs-lookup"><span data-stu-id="9181b-116">Name</span></span>       | <span data-ttu-id="9181b-117">説明</span><span class="sxs-lookup"><span data-stu-id="9181b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9181b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9181b-118">Authorization</span></span>  | <span data-ttu-id="9181b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9181b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9181b-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9181b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9181b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9181b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9181b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9181b-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9181b-125">応答</span><span class="sxs-lookup"><span data-stu-id="9181b-125">Response</span></span>

<span data-ttu-id="9181b-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9181b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9181b-128">例</span><span class="sxs-lookup"><span data-stu-id="9181b-128">Example</span></span>
<span data-ttu-id="9181b-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9181b-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9181b-130">要求</span><span class="sxs-lookup"><span data-stu-id="9181b-130">Request</span></span>
<span data-ttu-id="9181b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9181b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="9181b-132">応答</span><span class="sxs-lookup"><span data-stu-id="9181b-132">Response</span></span>
<span data-ttu-id="9181b-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9181b-133">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->