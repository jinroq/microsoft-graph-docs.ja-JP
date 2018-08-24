# <a name="add-group-owner"></a><span data-ttu-id="fe7a0-101">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="fe7a0-101">Add group owner</span></span>
<span data-ttu-id="fe7a0-p101">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe7a0-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe7a0-104">Permissions</span></span>
<span data-ttu-id="fe7a0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe7a0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe7a0-107">Permission type</span></span>      | <span data-ttu-id="fe7a0-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe7a0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe7a0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe7a0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fe7a0-110">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe7a0-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe7a0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe7a0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe7a0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-112">Not supported.</span></span>    |
|<span data-ttu-id="fe7a0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe7a0-113">Application</span></span> | <span data-ttu-id="fe7a0-114">Group.ReadWrite.All と Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe7a0-114">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe7a0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe7a0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fe7a0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe7a0-116">Request headers</span></span>
| <span data-ttu-id="fe7a0-117">名前</span><span class="sxs-lookup"><span data-stu-id="fe7a0-117">Name</span></span>       | <span data-ttu-id="fe7a0-118">型</span><span class="sxs-lookup"><span data-stu-id="fe7a0-118">Type</span></span> | <span data-ttu-id="fe7a0-119">説明</span><span class="sxs-lookup"><span data-stu-id="fe7a0-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe7a0-120">承認</span><span class="sxs-lookup"><span data-stu-id="fe7a0-120">Authorization</span></span>  | <span data-ttu-id="fe7a0-121">文字列</span><span class="sxs-lookup"><span data-stu-id="fe7a0-121">string</span></span>  | <span data-ttu-id="fe7a0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe7a0-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe7a0-124">Request body</span></span>
<span data-ttu-id="fe7a0-125">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-125">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fe7a0-126">応答</span><span class="sxs-lookup"><span data-stu-id="fe7a0-126">Response</span></span>
<span data-ttu-id="fe7a0-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe7a0-129">例</span><span class="sxs-lookup"><span data-stu-id="fe7a0-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe7a0-130">要求</span><span class="sxs-lookup"><span data-stu-id="fe7a0-130">Request</span></span>
<span data-ttu-id="fe7a0-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="fe7a0-132">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="fe7a0-133">応答</span><span class="sxs-lookup"><span data-stu-id="fe7a0-133">Response</span></span>
<span data-ttu-id="fe7a0-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-134">The following is an example of the response.</span></span>
><span data-ttu-id="fe7a0-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe7a0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
