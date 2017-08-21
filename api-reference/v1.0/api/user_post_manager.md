# <a name="assign-a-manager"></a><span data-ttu-id="f0802-101">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="f0802-101">Assign a manager</span></span>

<span data-ttu-id="f0802-102">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="f0802-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="f0802-103">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0802-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0802-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0802-104">Prerequisites</span></span>
<span data-ttu-id="f0802-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="f0802-105">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="f0802-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0802-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f0802-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0802-107">Request headers</span></span>
| <span data-ttu-id="f0802-108">名前</span><span class="sxs-lookup"><span data-stu-id="f0802-108">Name</span></span>       | <span data-ttu-id="f0802-109">型</span><span class="sxs-lookup"><span data-stu-id="f0802-109">Type</span></span> | <span data-ttu-id="f0802-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0802-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0802-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0802-111">Authorization</span></span>  | <span data-ttu-id="f0802-112">string</span><span class="sxs-lookup"><span data-stu-id="f0802-112">string</span></span>  | <span data-ttu-id="f0802-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0802-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0802-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0802-115">Request body</span></span>
<span data-ttu-id="f0802-116">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0802-116">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f0802-117">応答</span><span class="sxs-lookup"><span data-stu-id="f0802-117">Response</span></span>

<span data-ttu-id="f0802-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f0802-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0802-120">例</span><span class="sxs-lookup"><span data-stu-id="f0802-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0802-121">要求</span><span class="sxs-lookup"><span data-stu-id="f0802-121">Request</span></span>
<span data-ttu-id="f0802-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0802-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="f0802-123">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0802-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="f0802-124">応答</span><span class="sxs-lookup"><span data-stu-id="f0802-124">Response</span></span>
<span data-ttu-id="f0802-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0802-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
