# <a name="add-a-student"></a><span data-ttu-id="ea0c0-101">生徒を追加する</span><span class="sxs-lookup"><span data-stu-id="ea0c0-101">Add a student</span></span>

<span data-ttu-id="ea0c0-102">クラスにメンバーを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-102">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea0c0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea0c0-103">Permissions</span></span>
<span data-ttu-id="ea0c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea0c0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea0c0-106">Permission type</span></span>      | <span data-ttu-id="ea0c0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea0c0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea0c0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea0c0-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="ea0c0-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-109">Not supported.</span></span>  |
|<span data-ttu-id="ea0c0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea0c0-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ea0c0-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-111">Not supported.</span></span>  |
|<span data-ttu-id="ea0c0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea0c0-112">Application</span></span> | <span data-ttu-id="ea0c0-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea0c0-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ea0c0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea0c0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ea0c0-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea0c0-115">Request headers</span></span>
| <span data-ttu-id="ea0c0-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea0c0-116">Header</span></span>       | <span data-ttu-id="ea0c0-117">値</span><span class="sxs-lookup"><span data-stu-id="ea0c0-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea0c0-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea0c0-118">Authorization</span></span>  | <span data-ttu-id="ea0c0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea0c0-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea0c0-121">Content-Type</span></span>  | <span data-ttu-id="ea0c0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea0c0-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea0c0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea0c0-123">Request body</span></span>
<span data-ttu-id="ea0c0-124">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ea0c0-125">応答</span><span class="sxs-lookup"><span data-stu-id="ea0c0-125">Response</span></span>
<span data-ttu-id="ea0c0-126">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea0c0-127">例</span><span class="sxs-lookup"><span data-stu-id="ea0c0-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea0c0-128">要求</span><span class="sxs-lookup"><span data-stu-id="ea0c0-128">Request</span></span>
<span data-ttu-id="ea0c0-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="ea0c0-130">応答</span><span class="sxs-lookup"><span data-stu-id="ea0c0-130">Response</span></span>
<span data-ttu-id="ea0c0-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea0c0-131">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->