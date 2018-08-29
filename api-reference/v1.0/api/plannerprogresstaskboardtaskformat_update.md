# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="f7f18-101">Update plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f7f18-101">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="f7f18-102">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f7f18-102">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7f18-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7f18-103">Permissions</span></span>
<span data-ttu-id="f7f18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7f18-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7f18-106">Permission type</span></span>      | <span data-ttu-id="f7f18-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7f18-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7f18-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7f18-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f7f18-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f18-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7f18-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7f18-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7f18-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7f18-111">Not supported.</span></span>    |
|<span data-ttu-id="f7f18-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7f18-112">Application</span></span> | <span data-ttu-id="f7f18-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7f18-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7f18-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7f18-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="f7f18-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7f18-115">Optional request headers</span></span>
| <span data-ttu-id="f7f18-116">名前</span><span class="sxs-lookup"><span data-stu-id="f7f18-116">Name</span></span>       | <span data-ttu-id="f7f18-117">説明</span><span class="sxs-lookup"><span data-stu-id="f7f18-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f7f18-118">承認</span><span class="sxs-lookup"><span data-stu-id="f7f18-118">Authorization</span></span>  | <span data-ttu-id="f7f18-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7f18-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="f7f18-121">If-Match</span></span>  | <span data-ttu-id="f7f18-p103">更新する **plannerProgressTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f18-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7f18-124">Request body</span></span>
<span data-ttu-id="f7f18-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7f18-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7f18-128">Property</span></span>     | <span data-ttu-id="f7f18-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="f7f18-129">Type</span></span>   |<span data-ttu-id="f7f18-130">説明</span><span class="sxs-lookup"><span data-stu-id="f7f18-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7f18-131">orderHint</span><span class="sxs-lookup"><span data-stu-id="f7f18-131">orderHint</span></span>|<span data-ttu-id="f7f18-132">String</span><span class="sxs-lookup"><span data-stu-id="f7f18-132">String</span></span>|<span data-ttu-id="f7f18-p105">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](../resources/planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f7f18-135">応答</span><span class="sxs-lookup"><span data-stu-id="f7f18-135">Response</span></span>

<span data-ttu-id="f7f18-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f7f18-136">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="f7f18-p106">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f7f18-140">例</span><span class="sxs-lookup"><span data-stu-id="f7f18-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7f18-141">要求</span><span class="sxs-lookup"><span data-stu-id="f7f18-141">Request</span></span>
<span data-ttu-id="f7f18-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f7f18-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="f7f18-143">応答</span><span class="sxs-lookup"><span data-stu-id="f7f18-143">Response</span></span>
<span data-ttu-id="f7f18-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f7f18-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->