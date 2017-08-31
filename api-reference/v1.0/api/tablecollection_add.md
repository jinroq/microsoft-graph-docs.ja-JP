# <a name="tablecollection-add"></a><span data-ttu-id="f8f81-101">TableCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="f8f81-101">TableCollection: add</span></span>

<span data-ttu-id="f8f81-p101">新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8f81-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8f81-105">Permissions</span></span>
<span data-ttu-id="f8f81-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8f81-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8f81-108">Permission type</span></span>      | <span data-ttu-id="f8f81-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8f81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8f81-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8f81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8f81-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8f81-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8f81-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8f81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8f81-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8f81-113">Not supported.</span></span>    |
|<span data-ttu-id="f8f81-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8f81-114">Application</span></span> | <span data-ttu-id="f8f81-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8f81-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8f81-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8f81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="f8f81-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8f81-117">Request headers</span></span>
| <span data-ttu-id="f8f81-118">名前</span><span class="sxs-lookup"><span data-stu-id="f8f81-118">Name</span></span>       | <span data-ttu-id="f8f81-119">説明</span><span class="sxs-lookup"><span data-stu-id="f8f81-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8f81-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f81-120">Authorization</span></span>  | <span data-ttu-id="f8f81-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8f81-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8f81-123">Request body</span></span>
<span data-ttu-id="f8f81-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8f81-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8f81-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f8f81-125">Parameter</span></span>    | <span data-ttu-id="f8f81-126">型</span><span class="sxs-lookup"><span data-stu-id="f8f81-126">Type</span></span>   |<span data-ttu-id="f8f81-127">説明</span><span class="sxs-lookup"><span data-stu-id="f8f81-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8f81-128">address</span><span class="sxs-lookup"><span data-stu-id="f8f81-128">address</span></span>|<span data-ttu-id="f8f81-129">string</span><span class="sxs-lookup"><span data-stu-id="f8f81-129">string</span></span>|<span data-ttu-id="f8f81-p104">データ ソースを表す Range オブジェクトのアドレスまたは名前。アドレスにシート名が含まれていない場合は、現在作業中のシートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p104">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="f8f81-132">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f8f81-132">hasHeaders</span></span>|<span data-ttu-id="f8f81-133">boolean</span><span class="sxs-lookup"><span data-stu-id="f8f81-133">boolean</span></span>|<span data-ttu-id="f8f81-p105">インポートされたデータに列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p105">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="f8f81-137">応答</span><span class="sxs-lookup"><span data-stu-id="f8f81-137">Response</span></span>

<span data-ttu-id="f8f81-138">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f8f81-138">If successful, this method returns `200, OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f81-139">例</span><span class="sxs-lookup"><span data-stu-id="f8f81-139">Example</span></span>
<span data-ttu-id="f8f81-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f8f81-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8f81-141">要求</span><span class="sxs-lookup"><span data-stu-id="f8f81-141">Request</span></span>
<span data-ttu-id="f8f81-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8f81-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f8f81-143">応答</span><span class="sxs-lookup"><span data-stu-id="f8f81-143">Response</span></span>
<span data-ttu-id="f8f81-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8f81-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
