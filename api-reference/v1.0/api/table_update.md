# <a name="update-table"></a><span data-ttu-id="e93f1-101">テーブルを更新する</span><span class="sxs-lookup"><span data-stu-id="e93f1-101">Update table</span></span>

<span data-ttu-id="e93f1-102">table オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e93f1-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e93f1-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e93f1-103">Permissions</span></span>
<span data-ttu-id="e93f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e93f1-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e93f1-106">Permission type</span></span>      | <span data-ttu-id="e93f1-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e93f1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e93f1-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e93f1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e93f1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e93f1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e93f1-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e93f1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e93f1-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93f1-111">Not supported.</span></span>    |
|<span data-ttu-id="e93f1-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e93f1-112">Application</span></span> | <span data-ttu-id="e93f1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93f1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e93f1-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e93f1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e93f1-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e93f1-115">Optional request headers</span></span>
| <span data-ttu-id="e93f1-116">名前</span><span class="sxs-lookup"><span data-stu-id="e93f1-116">Name</span></span>       | <span data-ttu-id="e93f1-117">説明</span><span class="sxs-lookup"><span data-stu-id="e93f1-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e93f1-118">承認</span><span class="sxs-lookup"><span data-stu-id="e93f1-118">Authorization</span></span>  | <span data-ttu-id="e93f1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e93f1-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e93f1-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e93f1-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e93f1-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="e93f1-124">Request body</span></span>
<span data-ttu-id="e93f1-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e93f1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e93f1-128">Property</span></span>     | <span data-ttu-id="e93f1-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="e93f1-129">Type</span></span>   |<span data-ttu-id="e93f1-130">説明</span><span class="sxs-lookup"><span data-stu-id="e93f1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e93f1-131">name</span><span class="sxs-lookup"><span data-stu-id="e93f1-131">name</span></span>|<span data-ttu-id="e93f1-132">string</span><span class="sxs-lookup"><span data-stu-id="e93f1-132">string</span></span>|<span data-ttu-id="e93f1-133">テーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="e93f1-133">Name of the table.</span></span>|
|<span data-ttu-id="e93f1-134">showHeaders</span><span class="sxs-lookup"><span data-stu-id="e93f1-134">showHeaders</span></span>|<span data-ttu-id="e93f1-135">boolean</span><span class="sxs-lookup"><span data-stu-id="e93f1-135">boolean</span></span>|<span data-ttu-id="e93f1-p105">ヘッダー行を表示するかどうかを示します。この値によって、ヘッダー行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="e93f1-138">showTotals</span><span class="sxs-lookup"><span data-stu-id="e93f1-138">showTotals</span></span>|<span data-ttu-id="e93f1-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e93f1-139">boolean</span></span>|<span data-ttu-id="e93f1-p106">集計行を表示するかどうかを示します。この値によって、集計行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="e93f1-142">style</span><span class="sxs-lookup"><span data-stu-id="e93f1-142">style</span></span>|<span data-ttu-id="e93f1-143">string</span><span class="sxs-lookup"><span data-stu-id="e93f1-143">string</span></span>|<span data-ttu-id="e93f1-144">表スタイルを表す定数の値です。</span><span class="sxs-lookup"><span data-stu-id="e93f1-144">Constant value that represents the Table style.</span></span> <span data-ttu-id="e93f1-145">可能な値は、TableStyleLight1 〜 TableStyleLight21、TableStyleMedium1 〜 TableStyleMedium28、TableStyleStyleDark1 〜 TableStyleStyleDark11 です。</span><span class="sxs-lookup"><span data-stu-id="e93f1-145">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="e93f1-146">ブック内にあるカスタムのユーザー定義スタイルも指定することができます。</span><span class="sxs-lookup"><span data-stu-id="e93f1-146">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="e93f1-147">応答</span><span class="sxs-lookup"><span data-stu-id="e93f1-147">Response</span></span>

<span data-ttu-id="e93f1-148">成功した場合、このメソッドは `200 OK` 応答コードを返し、応答本文で [WorkbookTable](../resources/table.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e93f1-148">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e93f1-149">例</span><span class="sxs-lookup"><span data-stu-id="e93f1-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e93f1-150">要求</span><span class="sxs-lookup"><span data-stu-id="e93f1-150">Request</span></span>
<span data-ttu-id="e93f1-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e93f1-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="e93f1-152">応答</span><span class="sxs-lookup"><span data-stu-id="e93f1-152">Response</span></span>
<span data-ttu-id="e93f1-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e93f1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
