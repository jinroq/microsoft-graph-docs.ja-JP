# <a name="add-group-owner"></a><span data-ttu-id="17e95-101">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="17e95-101">Add group owner</span></span>
<span data-ttu-id="17e95-p101">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="17e95-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17e95-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="17e95-104">Prerequisites</span></span>
<span data-ttu-id="17e95-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="17e95-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="17e95-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17e95-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="17e95-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17e95-107">Request headers</span></span>
| <span data-ttu-id="17e95-108">名前</span><span class="sxs-lookup"><span data-stu-id="17e95-108">Name</span></span>       | <span data-ttu-id="17e95-109">型</span><span class="sxs-lookup"><span data-stu-id="17e95-109">Type</span></span> | <span data-ttu-id="17e95-110">説明</span><span class="sxs-lookup"><span data-stu-id="17e95-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17e95-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="17e95-111">Authorization</span></span>  | <span data-ttu-id="17e95-112">string</span><span class="sxs-lookup"><span data-stu-id="17e95-112">string</span></span>  | <span data-ttu-id="17e95-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17e95-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17e95-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="17e95-115">Request body</span></span>
<span data-ttu-id="17e95-116">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="17e95-116">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="17e95-117">応答</span><span class="sxs-lookup"><span data-stu-id="17e95-117">Response</span></span>

<span data-ttu-id="17e95-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="17e95-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17e95-120">例</span><span class="sxs-lookup"><span data-stu-id="17e95-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17e95-121">要求</span><span class="sxs-lookup"><span data-stu-id="17e95-121">Request</span></span>
<span data-ttu-id="17e95-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17e95-122">Here is an example of the request.</span></span>
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
<span data-ttu-id="17e95-123">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="17e95-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="17e95-124">応答</span><span class="sxs-lookup"><span data-stu-id="17e95-124">Response</span></span>
<span data-ttu-id="17e95-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17e95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
