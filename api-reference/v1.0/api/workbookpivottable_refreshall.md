# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="da994-101">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="da994-101">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="da994-102">指定されたワークシート内のピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="da994-102">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="da994-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da994-103">Permissions</span></span>
<span data-ttu-id="da994-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da994-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da994-106">Permission type</span></span>      | <span data-ttu-id="da994-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da994-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da994-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da994-108">Delegated (work or school account)</span></span> | <span data-ttu-id="da994-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da994-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da994-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da994-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da994-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da994-111">Not supported.</span></span>    |
|<span data-ttu-id="da994-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da994-112">Application</span></span> | <span data-ttu-id="da994-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da994-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da994-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da994-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="da994-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da994-115">Request headers</span></span>
| <span data-ttu-id="da994-116">名前</span><span class="sxs-lookup"><span data-stu-id="da994-116">Name</span></span>       | <span data-ttu-id="da994-117">説明</span><span class="sxs-lookup"><span data-stu-id="da994-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da994-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="da994-118">Authorization</span></span>  | <span data-ttu-id="da994-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da994-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da994-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da994-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="da994-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="da994-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da994-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="da994-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="da994-125">応答</span><span class="sxs-lookup"><span data-stu-id="da994-125">Response</span></span>
<span data-ttu-id="da994-p104">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="da994-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da994-128">例</span><span class="sxs-lookup"><span data-stu-id="da994-128">Example</span></span>
<span data-ttu-id="da994-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="da994-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da994-130">要求</span><span class="sxs-lookup"><span data-stu-id="da994-130">Request</span></span>
<span data-ttu-id="da994-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da994-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="da994-132">応答</span><span class="sxs-lookup"><span data-stu-id="da994-132">Response</span></span>
<span data-ttu-id="da994-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="da994-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
