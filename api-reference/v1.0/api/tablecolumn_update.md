# <a name="update-tablecolumn"></a><span data-ttu-id="390cd-101">tablecolumn を更新する</span><span class="sxs-lookup"><span data-stu-id="390cd-101">Update tablecolumn</span></span>

<span data-ttu-id="390cd-102">tablecolumn オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="390cd-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="390cd-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="390cd-103">Permissions</span></span>
<span data-ttu-id="390cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="390cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="390cd-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="390cd-106">Permission type</span></span>      | <span data-ttu-id="390cd-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="390cd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="390cd-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="390cd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="390cd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="390cd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="390cd-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="390cd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="390cd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="390cd-111">Not supported.</span></span>    |
|<span data-ttu-id="390cd-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="390cd-112">Application</span></span> | <span data-ttu-id="390cd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="390cd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="390cd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="390cd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="390cd-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="390cd-115">Optional request headers</span></span>
| <span data-ttu-id="390cd-116">名前</span><span class="sxs-lookup"><span data-stu-id="390cd-116">Name</span></span>       | <span data-ttu-id="390cd-117">説明</span><span class="sxs-lookup"><span data-stu-id="390cd-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="390cd-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="390cd-118">Authorization</span></span>  | <span data-ttu-id="390cd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="390cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="390cd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="390cd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="390cd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="390cd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="390cd-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="390cd-124">Request body</span></span>
<span data-ttu-id="390cd-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="390cd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="390cd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="390cd-128">Property</span></span>     | <span data-ttu-id="390cd-129">型</span><span class="sxs-lookup"><span data-stu-id="390cd-129">Type</span></span>   |<span data-ttu-id="390cd-130">説明</span><span class="sxs-lookup"><span data-stu-id="390cd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="390cd-131">values</span><span class="sxs-lookup"><span data-stu-id="390cd-131">values</span></span>|<span data-ttu-id="390cd-132">json</span><span class="sxs-lookup"><span data-stu-id="390cd-132">json</span></span>|<span data-ttu-id="390cd-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="390cd-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="390cd-136">応答</span><span class="sxs-lookup"><span data-stu-id="390cd-136">Response</span></span>

<span data-ttu-id="390cd-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="390cd-137">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="390cd-138">例</span><span class="sxs-lookup"><span data-stu-id="390cd-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="390cd-139">要求</span><span class="sxs-lookup"><span data-stu-id="390cd-139">Request</span></span>
<span data-ttu-id="390cd-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="390cd-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="390cd-141">応答</span><span class="sxs-lookup"><span data-stu-id="390cd-141">Response</span></span>
<span data-ttu-id="390cd-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="390cd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->