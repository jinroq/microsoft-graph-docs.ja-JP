# <a name="get-workbookpivottable"></a><span data-ttu-id="998fd-101">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="998fd-101">Get workbookPivotTable</span></span>

<span data-ttu-id="998fd-102">workbookPivotTable オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="998fd-102">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="998fd-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="998fd-103">Permissions</span></span>
<span data-ttu-id="998fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="998fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="998fd-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="998fd-106">Permission type</span></span>      | <span data-ttu-id="998fd-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="998fd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="998fd-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="998fd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="998fd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="998fd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="998fd-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="998fd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="998fd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="998fd-111">Not supported.</span></span>    |
|<span data-ttu-id="998fd-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="998fd-112">Application</span></span> | <span data-ttu-id="998fd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="998fd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="998fd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="998fd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="998fd-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="998fd-115">Optional query parameters</span></span>
<span data-ttu-id="998fd-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="998fd-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="998fd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="998fd-117">Request headers</span></span>
| <span data-ttu-id="998fd-118">名前</span><span class="sxs-lookup"><span data-stu-id="998fd-118">Name</span></span>      |<span data-ttu-id="998fd-119">説明</span><span class="sxs-lookup"><span data-stu-id="998fd-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="998fd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="998fd-120">Authorization</span></span>  | <span data-ttu-id="998fd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="998fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="998fd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="998fd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="998fd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="998fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="998fd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="998fd-126">Request body</span></span>
<span data-ttu-id="998fd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="998fd-127">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="998fd-128">応答</span><span class="sxs-lookup"><span data-stu-id="998fd-128">Response</span></span>
<span data-ttu-id="998fd-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookPivotTable](../resources/workbookpivottable.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="998fd-129">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="998fd-130">例</span><span class="sxs-lookup"><span data-stu-id="998fd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="998fd-131">要求</span><span class="sxs-lookup"><span data-stu-id="998fd-131">Request</span></span>
<span data-ttu-id="998fd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="998fd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="998fd-133">応答</span><span class="sxs-lookup"><span data-stu-id="998fd-133">Response</span></span>
<span data-ttu-id="998fd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="998fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
