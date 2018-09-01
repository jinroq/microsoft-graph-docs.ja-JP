# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="83550-101">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="83550-101">workbookRange: rowsBelow</span></span>

<span data-ttu-id="83550-102">指定した範囲の下にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="83550-102">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="83550-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83550-103">Permissions</span></span>
<span data-ttu-id="83550-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83550-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83550-106">Permission type</span></span>      | <span data-ttu-id="83550-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83550-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83550-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83550-108">Delegated (work or school account)</span></span> | <span data-ttu-id="83550-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83550-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83550-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83550-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83550-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83550-111">Not supported.</span></span>    |
|<span data-ttu-id="83550-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83550-112">Application</span></span> | <span data-ttu-id="83550-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83550-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83550-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83550-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="83550-115">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="83550-115">Function parameters</span></span>

| <span data-ttu-id="83550-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="83550-116">Parameter</span></span>    | <span data-ttu-id="83550-117">型</span><span class="sxs-lookup"><span data-stu-id="83550-117">Type</span></span>   |<span data-ttu-id="83550-118">説明</span><span class="sxs-lookup"><span data-stu-id="83550-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83550-119">カウント</span><span class="sxs-lookup"><span data-stu-id="83550-119">count</span></span>|<span data-ttu-id="83550-120">Int32</span><span class="sxs-lookup"><span data-stu-id="83550-120">Int32</span></span>| <span data-ttu-id="83550-p102">省略可能。結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="83550-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="83550-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83550-126">Request headers</span></span>
| <span data-ttu-id="83550-127">名前</span><span class="sxs-lookup"><span data-stu-id="83550-127">Name</span></span>       | <span data-ttu-id="83550-128">説明</span><span class="sxs-lookup"><span data-stu-id="83550-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83550-129">承認</span><span class="sxs-lookup"><span data-stu-id="83550-129">Authorization</span></span>  | <span data-ttu-id="83550-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83550-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83550-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="83550-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="83550-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="83550-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83550-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="83550-135">Request body</span></span>
<span data-ttu-id="83550-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83550-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83550-137">応答</span><span class="sxs-lookup"><span data-stu-id="83550-137">Response</span></span>
<span data-ttu-id="83550-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83550-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83550-139">例</span><span class="sxs-lookup"><span data-stu-id="83550-139">Example</span></span>
<span data-ttu-id="83550-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="83550-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="83550-141">要求</span><span class="sxs-lookup"><span data-stu-id="83550-141">Request</span></span>
<span data-ttu-id="83550-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83550-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="83550-143">応答</span><span class="sxs-lookup"><span data-stu-id="83550-143">Response</span></span>
<span data-ttu-id="83550-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83550-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<span data-ttu-id="83550-147">`count` パラメーター なしで呼び出された場合、 この関数は1つの行の既定値になります。</span><span class="sxs-lookup"><span data-stu-id="83550-147">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="83550-148">要求</span><span class="sxs-lookup"><span data-stu-id="83550-148">Request</span></span>
<span data-ttu-id="83550-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83550-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="83550-150">応答</span><span class="sxs-lookup"><span data-stu-id="83550-150">Response</span></span>
<span data-ttu-id="83550-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83550-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
