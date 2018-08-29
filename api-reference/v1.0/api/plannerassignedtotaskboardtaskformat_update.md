# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="07352-101">Update plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="07352-101">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="07352-102">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07352-102">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07352-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07352-103">Permissions</span></span>
<span data-ttu-id="07352-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="07352-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07352-106">Permission type</span></span>      | <span data-ttu-id="07352-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07352-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07352-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07352-108">Delegated (work or school account)</span></span> | <span data-ttu-id="07352-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07352-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07352-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07352-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07352-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07352-111">Not supported.</span></span>    |
|<span data-ttu-id="07352-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07352-112">Application</span></span> | <span data-ttu-id="07352-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07352-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07352-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07352-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="07352-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07352-115">Optional request headers</span></span>
| <span data-ttu-id="07352-116">名前</span><span class="sxs-lookup"><span data-stu-id="07352-116">Name</span></span>       | <span data-ttu-id="07352-117">説明</span><span class="sxs-lookup"><span data-stu-id="07352-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="07352-118">承認</span><span class="sxs-lookup"><span data-stu-id="07352-118">Authorization</span></span>  | <span data-ttu-id="07352-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07352-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07352-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="07352-121">If-Match</span></span>  | <span data-ttu-id="07352-p103">更新する **plannerAssignedToTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="07352-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07352-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="07352-124">Request body</span></span>
<span data-ttu-id="07352-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="07352-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07352-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07352-128">Property</span></span>     | <span data-ttu-id="07352-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="07352-129">Type</span></span>   |<span data-ttu-id="07352-130">説明</span><span class="sxs-lookup"><span data-stu-id="07352-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07352-131">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="07352-131">orderHintsByAssignee</span></span>|[<span data-ttu-id="07352-132">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="07352-132">plannerOrderHintsByAssignee</span></span>](../resources/plannerOrderHintsByAssignee.md)|<span data-ttu-id="07352-p105">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](../resources/planner_order_hint_format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="07352-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="07352-136">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="07352-136">unassignedOrderHint</span></span>|<span data-ttu-id="07352-137">String</span><span class="sxs-lookup"><span data-stu-id="07352-137">String</span></span>|<span data-ttu-id="07352-p106">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](../resources/planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="07352-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="07352-140">応答</span><span class="sxs-lookup"><span data-stu-id="07352-140">Response</span></span>

<span data-ttu-id="07352-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07352-141">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="07352-p107">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07352-p107">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="07352-145">例</span><span class="sxs-lookup"><span data-stu-id="07352-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07352-146">要求</span><span class="sxs-lookup"><span data-stu-id="07352-146">Request</span></span>
<span data-ttu-id="07352-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07352-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="07352-148">応答</span><span class="sxs-lookup"><span data-stu-id="07352-148">Response</span></span>
<span data-ttu-id="07352-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07352-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->