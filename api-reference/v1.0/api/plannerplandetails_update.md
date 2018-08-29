# <a name="update-plannerplandetails"></a><span data-ttu-id="4f8ef-101">Update plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="4f8ef-101">Update plannerplandetails</span></span>

<span data-ttu-id="4f8ef-102">**plannerplandetails** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-102">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f8ef-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f8ef-103">Permissions</span></span>
<span data-ttu-id="4f8ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f8ef-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f8ef-106">Permission type</span></span>      | <span data-ttu-id="4f8ef-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f8ef-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4f8ef-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f8ef-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f8ef-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f8ef-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f8ef-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-111">Not supported.</span></span>    |
|<span data-ttu-id="4f8ef-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f8ef-112">Application</span></span> | <span data-ttu-id="4f8ef-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f8ef-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f8ef-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="4f8ef-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f8ef-115">Optional request headers</span></span>
| <span data-ttu-id="4f8ef-116">名前</span><span class="sxs-lookup"><span data-stu-id="4f8ef-116">Name</span></span>       | <span data-ttu-id="4f8ef-117">説明</span><span class="sxs-lookup"><span data-stu-id="4f8ef-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4f8ef-118">承認</span><span class="sxs-lookup"><span data-stu-id="4f8ef-118">Authorization</span></span>  | <span data-ttu-id="4f8ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f8ef-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="4f8ef-121">If-Match</span></span>  | <span data-ttu-id="4f8ef-p103">更新する plannerPlanDetails の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f8ef-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f8ef-124">Request body</span></span>
<span data-ttu-id="4f8ef-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4f8ef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f8ef-128">Property</span></span>     | <span data-ttu-id="4f8ef-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="4f8ef-129">Type</span></span>   |<span data-ttu-id="4f8ef-130">説明</span><span class="sxs-lookup"><span data-stu-id="4f8ef-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f8ef-131">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="4f8ef-131">categoryDescriptions</span></span>|[<span data-ttu-id="4f8ef-132">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="4f8ef-132">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="4f8ef-133">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="4f8ef-133">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="4f8ef-134">sharedWith</span><span class="sxs-lookup"><span data-stu-id="4f8ef-134">sharedWith</span></span>|[<span data-ttu-id="4f8ef-135">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="4f8ef-135">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="4f8ef-p105">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](../resources/group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="4f8ef-139">応答</span><span class="sxs-lookup"><span data-stu-id="4f8ef-139">Response</span></span>

<span data-ttu-id="4f8ef-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [plannerPlanDetails](../resources/plannerplandetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-140">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="4f8ef-p106">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4f8ef-144">例</span><span class="sxs-lookup"><span data-stu-id="4f8ef-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f8ef-145">要求</span><span class="sxs-lookup"><span data-stu-id="4f8ef-145">Request</span></span>
<span data-ttu-id="4f8ef-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
Content-type: application/json
Content-length: 212
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
##### <a name="response"></a><span data-ttu-id="4f8ef-147">応答</span><span class="sxs-lookup"><span data-stu-id="4f8ef-147">Response</span></span>
<span data-ttu-id="4f8ef-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f8ef-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->