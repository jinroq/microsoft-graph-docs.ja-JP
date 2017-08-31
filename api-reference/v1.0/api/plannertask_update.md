# <a name="update-plannertask"></a><span data-ttu-id="7c0a7-101">Update plannertask</span><span class="sxs-lookup"><span data-stu-id="7c0a7-101">Update plannertask</span></span>

<span data-ttu-id="7c0a7-102">**plannertask** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-102">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c0a7-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c0a7-103">Permissions</span></span>
<span data-ttu-id="7c0a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c0a7-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c0a7-106">Permission type</span></span>      | <span data-ttu-id="7c0a7-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c0a7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c0a7-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c0a7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7c0a7-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0a7-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c0a7-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c0a7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c0a7-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-111">Not supported.</span></span>    |
|<span data-ttu-id="7c0a7-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c0a7-112">Application</span></span> | <span data-ttu-id="7c0a7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c0a7-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c0a7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="7c0a7-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c0a7-115">Optional request headers</span></span>
| <span data-ttu-id="7c0a7-116">名前</span><span class="sxs-lookup"><span data-stu-id="7c0a7-116">Name</span></span>       | <span data-ttu-id="7c0a7-117">説明</span><span class="sxs-lookup"><span data-stu-id="7c0a7-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7c0a7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c0a7-118">Authorization</span></span>  | <span data-ttu-id="7c0a7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c0a7-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="7c0a7-121">If-Match</span></span>  | <span data-ttu-id="7c0a7-p103">更新する **plannerTask** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c0a7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c0a7-124">Request body</span></span>
<span data-ttu-id="7c0a7-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c0a7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c0a7-128">Property</span></span>     | <span data-ttu-id="7c0a7-129">型</span><span class="sxs-lookup"><span data-stu-id="7c0a7-129">Type</span></span>   |<span data-ttu-id="7c0a7-130">説明</span><span class="sxs-lookup"><span data-stu-id="7c0a7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c0a7-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="7c0a7-131">appliedCategories</span></span>|[<span data-ttu-id="7c0a7-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="7c0a7-132">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="7c0a7-p105">タスクが適用されているカテゴリ。可能な値については、「[適用されるカテゴリ](../resources/plannerappliedcategories.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="7c0a7-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="7c0a7-135">assigneePriority</span></span>|<span data-ttu-id="7c0a7-136">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-136">String</span></span>|<span data-ttu-id="7c0a7-p106">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](../resources/planner_order_hint_format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="7c0a7-139">assignments</span><span class="sxs-lookup"><span data-stu-id="7c0a7-139">assignments</span></span>|[<span data-ttu-id="7c0a7-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="7c0a7-140">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="7c0a7-141">タスクが割り当てられているユーザーのセット。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-141">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="7c0a7-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="7c0a7-142">bucketId</span></span>|<span data-ttu-id="7c0a7-143">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-143">String</span></span>|<span data-ttu-id="7c0a7-p107">タスクが属しているバケット ID。バケットは、タスクがある計画に含まれている必要があります。28 文字長で、大文字と小文字の区別があります。[書式検証](../resources/planner_identifiers_disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p107">Bucket id to which the task belongs. The bucket needs to be in the plan that the task is in. It is 28 characters long and case sensitive. [Format validation](../resources/planner_identifiers_disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="7c0a7-148">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="7c0a7-148">conversationThreadId</span></span>|<span data-ttu-id="7c0a7-149">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-149">String</span></span>|<span data-ttu-id="7c0a7-p108">タスク内の会話のスレッド ID。これは、グループ内に作成された会話スレッド オブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="7c0a7-152">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0a7-152">dueDateTime</span></span>|<span data-ttu-id="7c0a7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0a7-153">DateTimeOffset</span></span>|<span data-ttu-id="7c0a7-p109">タスクが期限切れになる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c0a7-157">orderHint</span><span class="sxs-lookup"><span data-stu-id="7c0a7-157">orderHint</span></span>|<span data-ttu-id="7c0a7-158">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-158">String</span></span>|<span data-ttu-id="7c0a7-p110">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は「[プランナーでの順序のヒントの使用](../resources/planner_order_hint_format.md)」で定義されています。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="7c0a7-161">percentComplete</span><span class="sxs-lookup"><span data-stu-id="7c0a7-161">percentComplete</span></span>|<span data-ttu-id="7c0a7-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0a7-162">Int32</span></span>|<span data-ttu-id="7c0a7-p111">タスクの完了の割合。`100` に設定すると、タスクが完了したと見なされます。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="7c0a7-165">planId</span><span class="sxs-lookup"><span data-stu-id="7c0a7-165">planId</span></span>|<span data-ttu-id="7c0a7-166">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-166">String</span></span>|<span data-ttu-id="7c0a7-167">タスクが属している計画 ID。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-167">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="7c0a7-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0a7-168">startDateTime</span></span>|<span data-ttu-id="7c0a7-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0a7-169">DateTimeOffset</span></span>|<span data-ttu-id="7c0a7-p112">タスクが開始される日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c0a7-173">title</span><span class="sxs-lookup"><span data-stu-id="7c0a7-173">title</span></span>|<span data-ttu-id="7c0a7-174">String</span><span class="sxs-lookup"><span data-stu-id="7c0a7-174">String</span></span>|<span data-ttu-id="7c0a7-175">タスクのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="7c0a7-176">応答</span><span class="sxs-lookup"><span data-stu-id="7c0a7-176">Response</span></span>

<span data-ttu-id="7c0a7-177">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerTask](../resources/plannertask.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="7c0a7-p113">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p113">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7c0a7-181">例</span><span class="sxs-lookup"><span data-stu-id="7c0a7-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c0a7-182">要求</span><span class="sxs-lookup"><span data-stu-id="7c0a7-182">Request</span></span>
<span data-ttu-id="7c0a7-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-183">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
Content-type: application/json
Content-length: 247
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
##### <a name="response"></a><span data-ttu-id="7c0a7-184">応答</span><span class="sxs-lookup"><span data-stu-id="7c0a7-184">Response</span></span>
<span data-ttu-id="7c0a7-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c0a7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1423

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->