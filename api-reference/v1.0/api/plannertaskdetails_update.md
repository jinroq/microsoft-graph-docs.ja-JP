# <a name="update-plannertaskdetails"></a><span data-ttu-id="f726c-101">plannertaskdetails を更新する</span><span class="sxs-lookup"><span data-stu-id="f726c-101">Update plannertaskdetails</span></span>

<span data-ttu-id="f726c-102">**plannertaskdetails** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f726c-102">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f726c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f726c-103">Permissions</span></span>
<span data-ttu-id="f726c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f726c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f726c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f726c-106">Permission type</span></span>      | <span data-ttu-id="f726c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f726c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f726c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f726c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f726c-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f726c-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f726c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f726c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f726c-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f726c-111">Not supported.</span></span>    |
|<span data-ttu-id="f726c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f726c-112">Application</span></span> | <span data-ttu-id="f726c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f726c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f726c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f726c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="f726c-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f726c-115">Optional request headers</span></span>
| <span data-ttu-id="f726c-116">名前</span><span class="sxs-lookup"><span data-stu-id="f726c-116">Name</span></span>       | <span data-ttu-id="f726c-117">説明</span><span class="sxs-lookup"><span data-stu-id="f726c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f726c-118">承認</span><span class="sxs-lookup"><span data-stu-id="f726c-118">Authorization</span></span>  | <span data-ttu-id="f726c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f726c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f726c-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="f726c-121">If-Match</span></span>  | <span data-ttu-id="f726c-p103">更新する **plannerTaskDetails** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="f726c-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f726c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f726c-124">Request body</span></span>
<span data-ttu-id="f726c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f726c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f726c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f726c-128">Property</span></span>     | <span data-ttu-id="f726c-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="f726c-129">Type</span></span>   |<span data-ttu-id="f726c-130">説明</span><span class="sxs-lookup"><span data-stu-id="f726c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f726c-131">checklist</span><span class="sxs-lookup"><span data-stu-id="f726c-131">checklist</span></span>|[<span data-ttu-id="f726c-132">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="f726c-132">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="f726c-133">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f726c-133">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="f726c-134">説明</span><span class="sxs-lookup"><span data-stu-id="f726c-134">description</span></span>|<span data-ttu-id="f726c-135">String</span><span class="sxs-lookup"><span data-stu-id="f726c-135">String</span></span>|<span data-ttu-id="f726c-136">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="f726c-136">Description of the task</span></span>|
|<span data-ttu-id="f726c-137">previewType</span><span class="sxs-lookup"><span data-stu-id="f726c-137">previewType</span></span>|<span data-ttu-id="f726c-138">string</span><span class="sxs-lookup"><span data-stu-id="f726c-138">string</span></span>|<span data-ttu-id="f726c-139">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="f726c-139">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="f726c-140">可能な値は、`automatic`、`noPreview`、`checklist`、`description`、`reference` です。</span><span class="sxs-lookup"><span data-stu-id="f726c-140">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="f726c-141">`automatic` に設定されている場合、表示されるプレビューは、タスクを閲覧しているアプリによって選択されます。</span><span class="sxs-lookup"><span data-stu-id="f726c-141">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="f726c-142">references</span><span class="sxs-lookup"><span data-stu-id="f726c-142">references</span></span>|[<span data-ttu-id="f726c-143">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="f726c-143">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="f726c-144">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f726c-144">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="f726c-145">応答</span><span class="sxs-lookup"><span data-stu-id="f726c-145">Response</span></span>

<span data-ttu-id="f726c-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerTaskDetails](../resources/plannertaskdetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f726c-146">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="f726c-p106">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f726c-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f726c-150">例</span><span class="sxs-lookup"><span data-stu-id="f726c-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f726c-151">要求</span><span class="sxs-lookup"><span data-stu-id="f726c-151">Request</span></span>
<span data-ttu-id="f726c-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f726c-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
Content-type: application/json
Content-length: 857
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "previewType": "noPreview",
  "references": {
    "http%3A//developer%2Emicrosoft%2Ecom":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "previewPriority": " !",
      "type": "Other"
    },
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "previewPriority": "  !!",
    },
    "http%3A//www%2Ebing%2Ecom": null
  },
  "checklist": {
    "95e27074-6c4a-447a-aa24-9d718a0b86fa":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "title": "Update task details",
      "ischecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="f726c-153">応答</span><span class="sxs-lookup"><span data-stu-id="f726c-153">Response</span></span>
<span data-ttu-id="f726c-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f726c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1793

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "8599273",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "http%3A//developer%2Emicrosoft%2Ecom": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "type": "Other",
      "previewPriority": "90727736",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Try reading task details",
      "orderHint": "a93c93c5^",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "95e27074-6c4a-447a-aa24-9d718a0b86f": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Update task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->