# <a name="update-chartfont"></a><span data-ttu-id="e69a8-101">Update chartfont</span><span class="sxs-lookup"><span data-stu-id="e69a8-101">Update chartfont</span></span>

<span data-ttu-id="e69a8-102">chartfont オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e69a8-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e69a8-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e69a8-103">Permissions</span></span>
<span data-ttu-id="e69a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e69a8-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e69a8-106">Permission type</span></span>      | <span data-ttu-id="e69a8-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e69a8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e69a8-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e69a8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e69a8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e69a8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e69a8-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e69a8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e69a8-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e69a8-111">Not supported.</span></span>    |
|<span data-ttu-id="e69a8-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e69a8-112">Application</span></span> | <span data-ttu-id="e69a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e69a8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e69a8-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e69a8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="e69a8-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e69a8-115">Optional request headers</span></span>
| <span data-ttu-id="e69a8-116">名前</span><span class="sxs-lookup"><span data-stu-id="e69a8-116">Name</span></span>       | <span data-ttu-id="e69a8-117">説明</span><span class="sxs-lookup"><span data-stu-id="e69a8-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e69a8-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e69a8-118">Authorization</span></span>  | <span data-ttu-id="e69a8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e69a8-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="e69a8-121">Request body</span></span>
<span data-ttu-id="e69a8-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e69a8-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e69a8-125">Property</span></span>     | <span data-ttu-id="e69a8-126">型</span><span class="sxs-lookup"><span data-stu-id="e69a8-126">Type</span></span>   |<span data-ttu-id="e69a8-127">説明</span><span class="sxs-lookup"><span data-stu-id="e69a8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e69a8-128">bold</span><span class="sxs-lookup"><span data-stu-id="e69a8-128">bold</span></span>|<span data-ttu-id="e69a8-129">boolean</span><span class="sxs-lookup"><span data-stu-id="e69a8-129">boolean</span></span>|<span data-ttu-id="e69a8-130">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e69a8-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="e69a8-131">color</span><span class="sxs-lookup"><span data-stu-id="e69a8-131">color</span></span>|<span data-ttu-id="e69a8-132">string</span><span class="sxs-lookup"><span data-stu-id="e69a8-132">string</span></span>|<span data-ttu-id="e69a8-p104">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="e69a8-136">italic</span><span class="sxs-lookup"><span data-stu-id="e69a8-136">italic</span></span>|<span data-ttu-id="e69a8-137">boolean</span><span class="sxs-lookup"><span data-stu-id="e69a8-137">boolean</span></span>|<span data-ttu-id="e69a8-138">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e69a8-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="e69a8-139">name</span><span class="sxs-lookup"><span data-stu-id="e69a8-139">name</span></span>|<span data-ttu-id="e69a8-140">string</span><span class="sxs-lookup"><span data-stu-id="e69a8-140">string</span></span>|<span data-ttu-id="e69a8-141">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="e69a8-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="e69a8-142">size</span><span class="sxs-lookup"><span data-stu-id="e69a8-142">size</span></span>|<span data-ttu-id="e69a8-143">double</span><span class="sxs-lookup"><span data-stu-id="e69a8-143">double</span></span>|<span data-ttu-id="e69a8-144">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="e69a8-144">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="e69a8-145">underline</span><span class="sxs-lookup"><span data-stu-id="e69a8-145">underline</span></span>|<span data-ttu-id="e69a8-146">string</span><span class="sxs-lookup"><span data-stu-id="e69a8-146">string</span></span>|<span data-ttu-id="e69a8-p105">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p105">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="e69a8-149">応答</span><span class="sxs-lookup"><span data-stu-id="e69a8-149">Response</span></span>

<span data-ttu-id="e69a8-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartFont](../resources/chartfont.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e69a8-150">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e69a8-151">例</span><span class="sxs-lookup"><span data-stu-id="e69a8-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e69a8-152">要求</span><span class="sxs-lookup"><span data-stu-id="e69a8-152">Request</span></span>
<span data-ttu-id="e69a8-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e69a8-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="e69a8-154">応答</span><span class="sxs-lookup"><span data-stu-id="e69a8-154">Response</span></span>
<span data-ttu-id="e69a8-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e69a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->