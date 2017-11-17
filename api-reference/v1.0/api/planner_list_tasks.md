# <a name="list-tasks"></a><span data-ttu-id="40dac-101">List tasks</span><span class="sxs-lookup"><span data-stu-id="40dac-101">List tasks</span></span>

<span data-ttu-id="40dac-102">**plannertask** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="40dac-102">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="40dac-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40dac-103">Permissions</span></span>
<span data-ttu-id="40dac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40dac-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40dac-106">Permission type</span></span>      | <span data-ttu-id="40dac-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40dac-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40dac-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40dac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="40dac-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dac-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40dac-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40dac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40dac-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40dac-111">Not supported.</span></span>    |
|<span data-ttu-id="40dac-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40dac-112">Application</span></span> | <span data-ttu-id="40dac-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40dac-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40dac-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40dac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40dac-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="40dac-115">Optional query parameters</span></span>
<span data-ttu-id="40dac-116">このメソッドでは planId [フィルター](http://graph.microsoft.io/docs/overview/query_parameters)を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="40dac-116">This method requires planId [filter](http://graph.microsoft.io/docs/overview/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40dac-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40dac-117">Request headers</span></span>
| <span data-ttu-id="40dac-118">名前</span><span class="sxs-lookup"><span data-stu-id="40dac-118">Name</span></span>      |<span data-ttu-id="40dac-119">説明</span><span class="sxs-lookup"><span data-stu-id="40dac-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40dac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="40dac-120">Authorization</span></span>  | <span data-ttu-id="40dac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40dac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40dac-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="40dac-123">Request body</span></span>
<span data-ttu-id="40dac-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40dac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40dac-125">応答</span><span class="sxs-lookup"><span data-stu-id="40dac-125">Response</span></span>

<span data-ttu-id="40dac-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerTask](../resources/plannertask.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="40dac-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="40dac-p103">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40dac-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="40dac-130">例</span><span class="sxs-lookup"><span data-stu-id="40dac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40dac-131">要求</span><span class="sxs-lookup"><span data-stu-id="40dac-131">Request</span></span>
<span data-ttu-id="40dac-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40dac-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="40dac-133">応答</span><span class="sxs-lookup"><span data-stu-id="40dac-133">Response</span></span>
<span data-ttu-id="40dac-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40dac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
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
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->