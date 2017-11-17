# <a name="update-worksheet"></a><span data-ttu-id="f917d-101">ワークシートを更新する</span><span class="sxs-lookup"><span data-stu-id="f917d-101">Update worksheet</span></span>

<span data-ttu-id="f917d-102">ワークシート オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f917d-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f917d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f917d-103">Permissions</span></span>
<span data-ttu-id="f917d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f917d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f917d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f917d-106">Permission type</span></span>      | <span data-ttu-id="f917d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f917d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f917d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f917d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f917d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f917d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f917d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f917d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f917d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f917d-111">Not supported.</span></span>    |
|<span data-ttu-id="f917d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f917d-112">Application</span></span> | <span data-ttu-id="f917d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f917d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f917d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f917d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f917d-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f917d-115">Optional request headers</span></span>
| <span data-ttu-id="f917d-116">名前</span><span class="sxs-lookup"><span data-stu-id="f917d-116">Name</span></span>       | <span data-ttu-id="f917d-117">説明</span><span class="sxs-lookup"><span data-stu-id="f917d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f917d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="f917d-118">Authorization</span></span>  | <span data-ttu-id="f917d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f917d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f917d-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="f917d-121">Request body</span></span>
<span data-ttu-id="f917d-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f917d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f917d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f917d-125">Property</span></span>     | <span data-ttu-id="f917d-126">型</span><span class="sxs-lookup"><span data-stu-id="f917d-126">Type</span></span>   |<span data-ttu-id="f917d-127">説明</span><span class="sxs-lookup"><span data-stu-id="f917d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f917d-128">name</span><span class="sxs-lookup"><span data-stu-id="f917d-128">name</span></span>|<span data-ttu-id="f917d-129">string</span><span class="sxs-lookup"><span data-stu-id="f917d-129">string</span></span>|<span data-ttu-id="f917d-130">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="f917d-130">The display name of the worksheet.</span></span>|
|<span data-ttu-id="f917d-131">position</span><span class="sxs-lookup"><span data-stu-id="f917d-131">position</span></span>|<span data-ttu-id="f917d-132">int</span><span class="sxs-lookup"><span data-stu-id="f917d-132">int</span></span>|<span data-ttu-id="f917d-133">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="f917d-133">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="f917d-134">visibility</span><span class="sxs-lookup"><span data-stu-id="f917d-134">visibility</span></span>|<span data-ttu-id="f917d-135">string</span><span class="sxs-lookup"><span data-stu-id="f917d-135">string</span></span>|<span data-ttu-id="f917d-p104">ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。</span><span class="sxs-lookup"><span data-stu-id="f917d-p104">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="f917d-138">応答</span><span class="sxs-lookup"><span data-stu-id="f917d-138">Response</span></span>

<span data-ttu-id="f917d-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[ワークシート](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f917d-139">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f917d-140">例</span><span class="sxs-lookup"><span data-stu-id="f917d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f917d-141">要求</span><span class="sxs-lookup"><span data-stu-id="f917d-141">Request</span></span>
<span data-ttu-id="f917d-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f917d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="f917d-143">応答</span><span class="sxs-lookup"><span data-stu-id="f917d-143">Response</span></span>
<span data-ttu-id="f917d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f917d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->