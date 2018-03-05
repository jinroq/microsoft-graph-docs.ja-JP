# <a name="remove-a-student"></a><span data-ttu-id="caaa4-101">学生を削除する</span><span class="sxs-lookup"><span data-stu-id="caaa4-101">Remove a student</span></span>

<span data-ttu-id="caaa4-102">[educationClass](../resources/educationclass.md) から [educationUser](../resources/educationuser.md) を削除する</span><span class="sxs-lookup"><span data-stu-id="caaa4-102">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="caaa4-103">**メモ:** 教師_および_学生は、クラス **members** コレクションに所属します。</span><span class="sxs-lookup"><span data-stu-id="caaa4-103">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="caaa4-104">この API を呼び出す前に、削除する **educationUser** が教師でないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="caaa4-104">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="caaa4-105">[educationclass_list_teachers](educationclass_list_teachers.md) を呼び出して教師のリストを取得し、削除対象のユーザーのユーザー ID が返された教師リストにないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="caaa4-105">Get the list of teachers by calling [educationclass_list_teachers](educationclass_list_teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="caaa4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="caaa4-106">Permissions</span></span>
<span data-ttu-id="caaa4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="caaa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="caaa4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="caaa4-109">Permission type</span></span>      | <span data-ttu-id="caaa4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="caaa4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caaa4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="caaa4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="caaa4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caaa4-112">Not supported.</span></span>  |
|<span data-ttu-id="caaa4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="caaa4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="caaa4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caaa4-114">Not supported.</span></span>  |
|<span data-ttu-id="caaa4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="caaa4-115">Application</span></span> | <span data-ttu-id="caaa4-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caaa4-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="caaa4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="caaa4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="caaa4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caaa4-118">Request headers</span></span>
| <span data-ttu-id="caaa4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caaa4-119">Header</span></span>       | <span data-ttu-id="caaa4-120">値</span><span class="sxs-lookup"><span data-stu-id="caaa4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="caaa4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="caaa4-121">Authorization</span></span>  | <span data-ttu-id="caaa4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="caaa4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="caaa4-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="caaa4-124">Request body</span></span>
<span data-ttu-id="caaa4-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="caaa4-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="caaa4-126">応答</span><span class="sxs-lookup"><span data-stu-id="caaa4-126">Response</span></span>
<span data-ttu-id="caaa4-127">成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="caaa4-127">If successful, this method returns a `204 No Content` response code and an event object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caaa4-128">例</span><span class="sxs-lookup"><span data-stu-id="caaa4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="caaa4-129">要求</span><span class="sxs-lookup"><span data-stu-id="caaa4-129">Request</span></span>
<span data-ttu-id="caaa4-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="caaa4-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="caaa4-131">応答</span><span class="sxs-lookup"><span data-stu-id="caaa4-131">Response</span></span>
<span data-ttu-id="caaa4-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="caaa4-132">The following is an example of the response.</span></span> 
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
