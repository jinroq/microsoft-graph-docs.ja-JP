# <a name="add-member"></a><span data-ttu-id="ee645-101">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="ee645-101">Add member</span></span>

<span data-ttu-id="ee645-p101">この API を使用して、**メンバー**のナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループにメンバーを追加できます。ユーザーや他のグループを追加できます。重要事項:Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="ee645-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee645-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee645-105">Prerequisites</span></span>
<span data-ttu-id="ee645-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="ee645-106">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="ee645-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee645-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ee645-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee645-108">Request headers</span></span>
| <span data-ttu-id="ee645-109">名前</span><span class="sxs-lookup"><span data-stu-id="ee645-109">Name</span></span>       | <span data-ttu-id="ee645-110">型</span><span class="sxs-lookup"><span data-stu-id="ee645-110">Type</span></span> | <span data-ttu-id="ee645-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee645-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee645-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee645-112">Authorization</span></span>  | <span data-ttu-id="ee645-113">string</span><span class="sxs-lookup"><span data-stu-id="ee645-113">string</span></span>  | <span data-ttu-id="ee645-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee645-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee645-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee645-116">Request body</span></span>
<span data-ttu-id="ee645-117">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee645-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ee645-118">応答</span><span class="sxs-lookup"><span data-stu-id="ee645-118">Response</span></span>

<span data-ttu-id="ee645-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ee645-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee645-121">例</span><span class="sxs-lookup"><span data-stu-id="ee645-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee645-122">要求</span><span class="sxs-lookup"><span data-stu-id="ee645-122">Request</span></span>
<span data-ttu-id="ee645-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee645-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="ee645-124">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee645-124">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="ee645-125">応答</span><span class="sxs-lookup"><span data-stu-id="ee645-125">Response</span></span>
<span data-ttu-id="ee645-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee645-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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