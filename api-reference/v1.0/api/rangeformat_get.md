# <a name="get-rangeformat"></a><span data-ttu-id="babd8-101">RangeFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="babd8-101">Get RangeFormat</span></span>

<span data-ttu-id="babd8-102">rangeformat オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="babd8-102">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="babd8-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="babd8-103">Permissions</span></span>
<span data-ttu-id="babd8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="babd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="babd8-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="babd8-106">Permission type</span></span>      | <span data-ttu-id="babd8-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="babd8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="babd8-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="babd8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="babd8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="babd8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="babd8-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="babd8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="babd8-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="babd8-111">Not supported.</span></span>    |
|<span data-ttu-id="babd8-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="babd8-112">Application</span></span> | <span data-ttu-id="babd8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="babd8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="babd8-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="babd8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="babd8-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="babd8-115">Optional query parameters</span></span>
<span data-ttu-id="babd8-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="babd8-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="babd8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="babd8-117">Request headers</span></span>
| <span data-ttu-id="babd8-118">名前</span><span class="sxs-lookup"><span data-stu-id="babd8-118">Name</span></span>      |<span data-ttu-id="babd8-119">説明</span><span class="sxs-lookup"><span data-stu-id="babd8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="babd8-120">承認</span><span class="sxs-lookup"><span data-stu-id="babd8-120">Authorization</span></span>  | <span data-ttu-id="babd8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="babd8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="babd8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="babd8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="babd8-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="babd8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="babd8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="babd8-126">Request body</span></span>
<span data-ttu-id="babd8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="babd8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="babd8-128">応答</span><span class="sxs-lookup"><span data-stu-id="babd8-128">Response</span></span>

<span data-ttu-id="babd8-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[WorkbookRangeFormat](../resources/rangeformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="babd8-129">If successful, this method returns a `200 OK` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="babd8-130">例</span><span class="sxs-lookup"><span data-stu-id="babd8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="babd8-131">要求</span><span class="sxs-lookup"><span data-stu-id="babd8-131">Request</span></span>
<span data-ttu-id="babd8-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="babd8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format
```
##### <a name="response"></a><span data-ttu-id="babd8-133">応答</span><span class="sxs-lookup"><span data-stu-id="babd8-133">Response</span></span>
<span data-ttu-id="babd8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="babd8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->