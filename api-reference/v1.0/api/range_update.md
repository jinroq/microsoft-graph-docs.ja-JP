# <a name="update-range"></a><span data-ttu-id="8cc65-101">範囲を更新する</span><span class="sxs-lookup"><span data-stu-id="8cc65-101">Update range</span></span>

<span data-ttu-id="8cc65-102">範囲オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cc65-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cc65-103">Permissions</span></span>
<span data-ttu-id="8cc65-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8cc65-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cc65-106">Permission type</span></span>      | <span data-ttu-id="8cc65-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cc65-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc65-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc65-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc65-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cc65-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8cc65-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc65-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc65-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc65-111">Not supported.</span></span>    |
|<span data-ttu-id="8cc65-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cc65-112">Application</span></span> | <span data-ttu-id="8cc65-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc65-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc65-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cc65-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="8cc65-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cc65-115">Optional request headers</span></span>
| <span data-ttu-id="8cc65-116">名前</span><span class="sxs-lookup"><span data-stu-id="8cc65-116">Name</span></span>       | <span data-ttu-id="8cc65-117">説明</span><span class="sxs-lookup"><span data-stu-id="8cc65-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8cc65-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc65-118">Authorization</span></span>  | <span data-ttu-id="8cc65-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc65-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cc65-121">Request body</span></span>
<span data-ttu-id="8cc65-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8cc65-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc65-125">Property</span></span>     | <span data-ttu-id="8cc65-126">型</span><span class="sxs-lookup"><span data-stu-id="8cc65-126">Type</span></span>   |<span data-ttu-id="8cc65-127">説明</span><span class="sxs-lookup"><span data-stu-id="8cc65-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cc65-128">columnHidden</span><span class="sxs-lookup"><span data-stu-id="8cc65-128">columnHidden</span></span>|<span data-ttu-id="8cc65-129">boolean</span><span class="sxs-lookup"><span data-stu-id="8cc65-129">boolean</span></span>|<span data-ttu-id="8cc65-130">現在の範囲のすべての列が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-130">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="8cc65-131">formulas</span><span class="sxs-lookup"><span data-stu-id="8cc65-131">formulas</span></span>|<span data-ttu-id="8cc65-132">json</span><span class="sxs-lookup"><span data-stu-id="8cc65-132">json</span></span>|<span data-ttu-id="8cc65-133">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-133">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="8cc65-134">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="8cc65-134">formulasLocal</span></span>|<span data-ttu-id="8cc65-135">json</span><span class="sxs-lookup"><span data-stu-id="8cc65-135">json</span></span>|<span data-ttu-id="8cc65-p104">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p104">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="8cc65-138">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="8cc65-138">formulasR1C1</span></span>|<span data-ttu-id="8cc65-139">json</span><span class="sxs-lookup"><span data-stu-id="8cc65-139">json</span></span>|<span data-ttu-id="8cc65-140">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-140">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="8cc65-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="8cc65-141">numberFormat</span></span>|<span data-ttu-id="8cc65-142">json</span><span class="sxs-lookup"><span data-stu-id="8cc65-142">json</span></span>|<span data-ttu-id="8cc65-143">指定したセルの Excel の数値書式コードを表します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-143">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="8cc65-144">rowHidden</span><span class="sxs-lookup"><span data-stu-id="8cc65-144">rowHidden</span></span>|<span data-ttu-id="8cc65-145">boolean</span><span class="sxs-lookup"><span data-stu-id="8cc65-145">boolean</span></span>|<span data-ttu-id="8cc65-146">現在の範囲のすべての行が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-146">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="8cc65-147">values</span><span class="sxs-lookup"><span data-stu-id="8cc65-147">values</span></span>|<span data-ttu-id="8cc65-148">json</span><span class="sxs-lookup"><span data-stu-id="8cc65-148">json</span></span>|<span data-ttu-id="8cc65-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="8cc65-152">応答</span><span class="sxs-lookup"><span data-stu-id="8cc65-152">Response</span></span>

<span data-ttu-id="8cc65-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8cc65-153">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cc65-154">例</span><span class="sxs-lookup"><span data-stu-id="8cc65-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cc65-155">要求</span><span class="sxs-lookup"><span data-stu-id="8cc65-155">Request</span></span>
<span data-ttu-id="8cc65-p106">以下は、要求の例です。値、数値書式、および数式の範囲が更新されます。`null` 入力は、その特定の入力用のセルを無視するように API に指示します。値、数値書式、および数式は、個別に更新したり、同じ API 呼び出しで一緒に結合したりできます。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p106">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="8cc65-160">応答</span><span class="sxs-lookup"><span data-stu-id="8cc65-160">Response</span></span>
<span data-ttu-id="8cc65-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cc65-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
