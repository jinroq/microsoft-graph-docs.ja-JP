# <a name="create-plannerplan"></a><span data-ttu-id="f3f2d-101">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f3f2d-101">Create plannerPlan</span></span>

<span data-ttu-id="f3f2d-102">この API を使用して、新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-102">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3f2d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3f2d-103">Permissions</span></span>
<span data-ttu-id="f3f2d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3f2d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3f2d-106">Permission type</span></span>      | <span data-ttu-id="f3f2d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3f2d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3f2d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3f2d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f2d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f2d-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3f2d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3f2d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f2d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-111">Not supported.</span></span>    |
|<span data-ttu-id="f3f2d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3f2d-112">Application</span></span> | <span data-ttu-id="f3f2d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3f2d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3f2d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/plans

```
## <a name="request-headers"></a><span data-ttu-id="f3f2d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3f2d-115">Request headers</span></span>
| <span data-ttu-id="f3f2d-116">名前</span><span class="sxs-lookup"><span data-stu-id="f3f2d-116">Name</span></span>       | <span data-ttu-id="f3f2d-117">説明</span><span class="sxs-lookup"><span data-stu-id="f3f2d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3f2d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3f2d-118">Authorization</span></span>  | <span data-ttu-id="f3f2d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3f2d-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3f2d-121">Request body</span></span>
<span data-ttu-id="f3f2d-p103">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。**plannerPlan** 所有者プロパティは、[group](../resources/group.md) オブジェクトの ID に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3f2d-124">応答</span><span class="sxs-lookup"><span data-stu-id="f3f2d-124">Response</span></span>

<span data-ttu-id="f3f2d-125">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-125">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="f3f2d-p104">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-p104">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f3f2d-129">例</span><span class="sxs-lookup"><span data-stu-id="f3f2d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3f2d-130">要求</span><span class="sxs-lookup"><span data-stu-id="f3f2d-130">Request</span></span>
<span data-ttu-id="f3f2d-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
<span data-ttu-id="f3f2d-132">要求本文で、[plannerPlan](../resources/plannerplan.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-132">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f3f2d-133">応答</span><span class="sxs-lookup"><span data-stu-id="f3f2d-133">Response</span></span>
<span data-ttu-id="f3f2d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3f2d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->