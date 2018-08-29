# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="6aa5f-101">educationClass を educationSchool に追加する</span><span class="sxs-lookup"><span data-stu-id="6aa5f-101">Add educationClass to educationSchool</span></span>

<span data-ttu-id="6aa5f-102">学校にクラスを追加します。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-102">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aa5f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6aa5f-103">Permissions</span></span>
<span data-ttu-id="6aa5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6aa5f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6aa5f-106">Permission type</span></span>      | <span data-ttu-id="6aa5f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6aa5f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aa5f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6aa5f-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="6aa5f-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-109">Not supported.</span></span>  |
|<span data-ttu-id="6aa5f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6aa5f-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6aa5f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-111">Not supported.</span></span>  |
|<span data-ttu-id="6aa5f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6aa5f-112">Application</span></span> | <span data-ttu-id="6aa5f-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa5f-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6aa5f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6aa5f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6aa5f-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6aa5f-115">Request headers</span></span>
| <span data-ttu-id="6aa5f-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6aa5f-116">Header</span></span>       | <span data-ttu-id="6aa5f-117">値</span><span class="sxs-lookup"><span data-stu-id="6aa5f-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6aa5f-118">承認</span><span class="sxs-lookup"><span data-stu-id="6aa5f-118">Authorization</span></span>  | <span data-ttu-id="6aa5f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6aa5f-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6aa5f-121">Content-Type</span></span>  | <span data-ttu-id="6aa5f-122">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="6aa5f-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6aa5f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6aa5f-123">Request body</span></span>
<span data-ttu-id="6aa5f-124">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-124">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="6aa5f-125">応答</span><span class="sxs-lookup"><span data-stu-id="6aa5f-125">Response</span></span>
<span data-ttu-id="6aa5f-126">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-126">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa5f-127">例</span><span class="sxs-lookup"><span data-stu-id="6aa5f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6aa5f-128">要求</span><span class="sxs-lookup"><span data-stu-id="6aa5f-128">Request</span></span>
<span data-ttu-id="6aa5f-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="6aa5f-130">応答</span><span class="sxs-lookup"><span data-stu-id="6aa5f-130">Response</span></span> 
<span data-ttu-id="6aa5f-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6aa5f-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->