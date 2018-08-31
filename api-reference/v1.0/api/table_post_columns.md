# <a name="create-tablecolumn"></a><span data-ttu-id="ef55a-101">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="ef55a-101">Create TableColumn</span></span>

<span data-ttu-id="ef55a-102">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="ef55a-102">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef55a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ef55a-103">Permissions</span></span>
<span data-ttu-id="ef55a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef55a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef55a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef55a-106">Permission type</span></span>      | <span data-ttu-id="ef55a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef55a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef55a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef55a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ef55a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef55a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ef55a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef55a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef55a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef55a-111">Not supported.</span></span>    |
|<span data-ttu-id="ef55a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef55a-112">Application</span></span> | <span data-ttu-id="ef55a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef55a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef55a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef55a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="ef55a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef55a-115">Request headers</span></span>
| <span data-ttu-id="ef55a-116">名前</span><span class="sxs-lookup"><span data-stu-id="ef55a-116">Name</span></span>       | <span data-ttu-id="ef55a-117">説明</span><span class="sxs-lookup"><span data-stu-id="ef55a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ef55a-118">承認</span><span class="sxs-lookup"><span data-stu-id="ef55a-118">Authorization</span></span>  | <span data-ttu-id="ef55a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ef55a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef55a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ef55a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ef55a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ef55a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef55a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef55a-124">Request body</span></span>
<span data-ttu-id="ef55a-125">要求本文で、[WorkbookTableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef55a-125">In the request body, supply a JSON representation of [directoryObject](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef55a-126">応答</span><span class="sxs-lookup"><span data-stu-id="ef55a-126">Response</span></span>

<span data-ttu-id="ef55a-127">成功した場合、このメソッドは`201 Created` 応答コードと、応答本文で [WorkbookTableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ef55a-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef55a-128">例</span><span class="sxs-lookup"><span data-stu-id="ef55a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef55a-129">要求</span><span class="sxs-lookup"><span data-stu-id="ef55a-129">Request</span></span>
<span data-ttu-id="ef55a-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef55a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="ef55a-131">要求本文で、[WorkbookTableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef55a-131">In the request body, supply a JSON representation of [plannerPlan](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ef55a-132">応答</span><span class="sxs-lookup"><span data-stu-id="ef55a-132">Response</span></span>
<span data-ttu-id="ef55a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef55a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->