# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="9f690-101">Update plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9f690-101">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="9f690-102">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f690-102">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f690-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f690-103">Permissions</span></span>
<span data-ttu-id="9f690-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f690-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f690-106">Permission type</span></span>      | <span data-ttu-id="9f690-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f690-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f690-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f690-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9f690-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f690-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f690-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f690-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f690-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f690-111">Not supported.</span></span>    |
|<span data-ttu-id="9f690-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f690-112">Application</span></span> | <span data-ttu-id="9f690-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f690-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f690-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f690-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="9f690-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f690-115">Optional request headers</span></span>
| <span data-ttu-id="9f690-116">名前</span><span class="sxs-lookup"><span data-stu-id="9f690-116">Name</span></span>       | <span data-ttu-id="9f690-117">説明</span><span class="sxs-lookup"><span data-stu-id="9f690-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f690-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f690-118">Authorization</span></span>  | <span data-ttu-id="9f690-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9f690-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f690-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="9f690-121">If-Match</span></span>  | <span data-ttu-id="9f690-p103">更新する **plannerBucketTaskBoardTaskFormat** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="9f690-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f690-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f690-124">Request body</span></span>
<span data-ttu-id="9f690-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9f690-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f690-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f690-128">Property</span></span>     | <span data-ttu-id="9f690-129">型</span><span class="sxs-lookup"><span data-stu-id="9f690-129">Type</span></span>   |<span data-ttu-id="9f690-130">説明</span><span class="sxs-lookup"><span data-stu-id="9f690-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f690-131">orderHint</span><span class="sxs-lookup"><span data-stu-id="9f690-131">orderHint</span></span>|<span data-ttu-id="9f690-132">String</span><span class="sxs-lookup"><span data-stu-id="9f690-132">String</span></span>|<span data-ttu-id="9f690-p105">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](../resources/planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="9f690-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="9f690-135">応答</span><span class="sxs-lookup"><span data-stu-id="9f690-135">Response</span></span>

<span data-ttu-id="9f690-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f690-136">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="9f690-p106">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f690-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9f690-140">例</span><span class="sxs-lookup"><span data-stu-id="9f690-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f690-141">要求</span><span class="sxs-lookup"><span data-stu-id="9f690-141">Request</span></span>
<span data-ttu-id="9f690-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f690-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="9f690-143">応答</span><span class="sxs-lookup"><span data-stu-id="9f690-143">Response</span></span>
<span data-ttu-id="9f690-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f690-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->