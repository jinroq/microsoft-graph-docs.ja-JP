# <a name="update-chartaxis"></a><span data-ttu-id="fb85b-101">ChartAxis を更新する</span><span class="sxs-lookup"><span data-stu-id="fb85b-101">Update chartaxis</span></span>

<span data-ttu-id="fb85b-102">chartaxis オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb85b-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb85b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb85b-103">Permissions</span></span>
<span data-ttu-id="fb85b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb85b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb85b-106">Permission type</span></span>      | <span data-ttu-id="fb85b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb85b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb85b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb85b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb85b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb85b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb85b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb85b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb85b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb85b-111">Not supported.</span></span>    |
|<span data-ttu-id="fb85b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb85b-112">Application</span></span> | <span data-ttu-id="fb85b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb85b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb85b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb85b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="fb85b-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb85b-115">Optional request headers</span></span>
| <span data-ttu-id="fb85b-116">名前</span><span class="sxs-lookup"><span data-stu-id="fb85b-116">Name</span></span>       | <span data-ttu-id="fb85b-117">説明</span><span class="sxs-lookup"><span data-stu-id="fb85b-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fb85b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb85b-118">Authorization</span></span>  | <span data-ttu-id="fb85b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb85b-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb85b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb85b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb85b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb85b-124">Request body</span></span>
<span data-ttu-id="fb85b-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fb85b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb85b-128">Property</span></span>     | <span data-ttu-id="fb85b-129">型</span><span class="sxs-lookup"><span data-stu-id="fb85b-129">Type</span></span>   |<span data-ttu-id="fb85b-130">説明</span><span class="sxs-lookup"><span data-stu-id="fb85b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb85b-131">majorUnit</span><span class="sxs-lookup"><span data-stu-id="fb85b-131">majorUnit</span></span>|<span data-ttu-id="fb85b-132">object</span><span class="sxs-lookup"><span data-stu-id="fb85b-132">object</span></span>|<span data-ttu-id="fb85b-p105">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb85b-136">maximum</span><span class="sxs-lookup"><span data-stu-id="fb85b-136">maximum</span></span>|<span data-ttu-id="fb85b-137">object</span><span class="sxs-lookup"><span data-stu-id="fb85b-137">object</span></span>|<span data-ttu-id="fb85b-p106">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb85b-141">minimum</span><span class="sxs-lookup"><span data-stu-id="fb85b-141">minimum</span></span>|<span data-ttu-id="fb85b-142">object</span><span class="sxs-lookup"><span data-stu-id="fb85b-142">object</span></span>|<span data-ttu-id="fb85b-p107">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb85b-146">minorUnit</span><span class="sxs-lookup"><span data-stu-id="fb85b-146">minorUnit</span></span>|<span data-ttu-id="fb85b-147">object</span><span class="sxs-lookup"><span data-stu-id="fb85b-147">object</span></span>|<span data-ttu-id="fb85b-p108">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="fb85b-151">応答</span><span class="sxs-lookup"><span data-stu-id="fb85b-151">Response</span></span>

<span data-ttu-id="fb85b-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartAxis](../resources/chartaxis.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fb85b-152">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb85b-153">例</span><span class="sxs-lookup"><span data-stu-id="fb85b-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb85b-154">要求</span><span class="sxs-lookup"><span data-stu-id="fb85b-154">Request</span></span>
<span data-ttu-id="fb85b-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb85b-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="fb85b-156">応答</span><span class="sxs-lookup"><span data-stu-id="fb85b-156">Response</span></span>
<span data-ttu-id="fb85b-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb85b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->