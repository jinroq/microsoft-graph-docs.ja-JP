# <a name="get-plannertaskdetails"></a><span data-ttu-id="93b72-101">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="93b72-101">Get plannerTaskDetails</span></span>

<span data-ttu-id="93b72-102">**plannertaskdetails** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="93b72-102">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="93b72-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93b72-103">Permissions</span></span>
<span data-ttu-id="93b72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="93b72-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93b72-106">Permission type</span></span>      | <span data-ttu-id="93b72-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93b72-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93b72-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93b72-108">Delegated (work or school account)</span></span> | <span data-ttu-id="93b72-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93b72-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93b72-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93b72-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93b72-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93b72-111">Not supported.</span></span>    |
|<span data-ttu-id="93b72-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93b72-112">Application</span></span> | <span data-ttu-id="93b72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93b72-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93b72-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93b72-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="93b72-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93b72-115">Request headers</span></span>
| <span data-ttu-id="93b72-116">名前</span><span class="sxs-lookup"><span data-stu-id="93b72-116">Name</span></span>      |<span data-ttu-id="93b72-117">説明</span><span class="sxs-lookup"><span data-stu-id="93b72-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93b72-118">承認</span><span class="sxs-lookup"><span data-stu-id="93b72-118">Authorization</span></span>  | <span data-ttu-id="93b72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="93b72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93b72-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="93b72-121">Request body</span></span>
<span data-ttu-id="93b72-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="93b72-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93b72-123">応答</span><span class="sxs-lookup"><span data-stu-id="93b72-123">Response</span></span>

<span data-ttu-id="93b72-124">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerTaskDetails](../resources/plannertaskdetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="93b72-124">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="93b72-p103">このメソッドは、いずれかの [HTTP 状態コード](../../../concepts/errors.md)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner_overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b72-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="93b72-128">例</span><span class="sxs-lookup"><span data-stu-id="93b72-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93b72-129">要求</span><span class="sxs-lookup"><span data-stu-id="93b72-129">Request</span></span>
<span data-ttu-id="93b72-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="93b72-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="93b72-131">応答</span><span class="sxs-lookup"><span data-stu-id="93b72-131">Response</span></span>
<span data-ttu-id="93b72-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="93b72-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
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
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->