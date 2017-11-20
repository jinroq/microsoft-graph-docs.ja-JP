# <a name="tablecollection-add"></a><span data-ttu-id="da68d-101">TableCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="da68d-101">TableCollection: add</span></span>

<span data-ttu-id="da68d-p101">新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="da68d-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="da68d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da68d-105">Permissions</span></span>
<span data-ttu-id="da68d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da68d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da68d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da68d-108">Permission type</span></span>      | <span data-ttu-id="da68d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da68d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da68d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da68d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da68d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da68d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da68d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da68d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da68d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da68d-113">Not supported.</span></span>    |
|<span data-ttu-id="da68d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da68d-114">Application</span></span> | <span data-ttu-id="da68d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da68d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da68d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da68d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="da68d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da68d-117">Request headers</span></span>
| <span data-ttu-id="da68d-118">名前</span><span class="sxs-lookup"><span data-stu-id="da68d-118">Name</span></span>       | <span data-ttu-id="da68d-119">説明</span><span class="sxs-lookup"><span data-stu-id="da68d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da68d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="da68d-120">Authorization</span></span>  | <span data-ttu-id="da68d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da68d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da68d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da68d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="da68d-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="da68d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da68d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="da68d-126">Request body</span></span>
<span data-ttu-id="da68d-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="da68d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da68d-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="da68d-128">Parameter</span></span>    | <span data-ttu-id="da68d-129">Type</span><span class="sxs-lookup"><span data-stu-id="da68d-129">Type</span></span>   |<span data-ttu-id="da68d-130">説明</span><span class="sxs-lookup"><span data-stu-id="da68d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da68d-131">address</span><span class="sxs-lookup"><span data-stu-id="da68d-131">address</span></span>|<span data-ttu-id="da68d-132">string</span><span class="sxs-lookup"><span data-stu-id="da68d-132">string</span></span>|<span data-ttu-id="da68d-p105">データ ソースを表す Range オブジェクトのアドレスまたは名前。アドレスにシート名が含まれていない場合は、現在作業中のシートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="da68d-p105">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="da68d-135">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="da68d-135">hasHeaders</span></span>|<span data-ttu-id="da68d-136">boolean</span><span class="sxs-lookup"><span data-stu-id="da68d-136">boolean</span></span>|<span data-ttu-id="da68d-p106">インポートされたデータに列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="da68d-p106">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="da68d-140">応答</span><span class="sxs-lookup"><span data-stu-id="da68d-140">Response</span></span>

<span data-ttu-id="da68d-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da68d-141">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da68d-142">例</span><span class="sxs-lookup"><span data-stu-id="da68d-142">Example</span></span>
<span data-ttu-id="da68d-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="da68d-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da68d-144">要求</span><span class="sxs-lookup"><span data-stu-id="da68d-144">Request</span></span>
<span data-ttu-id="da68d-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da68d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="da68d-146">応答</span><span class="sxs-lookup"><span data-stu-id="da68d-146">Response</span></span>
<span data-ttu-id="da68d-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da68d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
