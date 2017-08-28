# <a name="add-member"></a><span data-ttu-id="cd3af-101">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="cd3af-101">Add member</span></span>

<span data-ttu-id="cd3af-p101">この API を使用して、**メンバー**のナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループにメンバーを追加できます。ユーザーや他のグループを追加できます。重要事項:Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="cd3af-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd3af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd3af-105">Permissions</span></span>
<span data-ttu-id="cd3af-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd3af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="cd3af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd3af-108">Permission type</span></span>      | <span data-ttu-id="cd3af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd3af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd3af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd3af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd3af-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd3af-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd3af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd3af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd3af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd3af-113">Not supported.</span></span>    |
|<span data-ttu-id="cd3af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd3af-114">Application</span></span> | <span data-ttu-id="cd3af-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd3af-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd3af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd3af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cd3af-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd3af-117">Request headers</span></span>
| <span data-ttu-id="cd3af-118">名前</span><span class="sxs-lookup"><span data-stu-id="cd3af-118">Name</span></span>       | <span data-ttu-id="cd3af-119">型</span><span class="sxs-lookup"><span data-stu-id="cd3af-119">Type</span></span> | <span data-ttu-id="cd3af-120">説明</span><span class="sxs-lookup"><span data-stu-id="cd3af-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd3af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd3af-121">Authorization</span></span>  | <span data-ttu-id="cd3af-122">string</span><span class="sxs-lookup"><span data-stu-id="cd3af-122">string</span></span>  | <span data-ttu-id="cd3af-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cd3af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd3af-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd3af-125">Request body</span></span>
<span data-ttu-id="cd3af-126">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd3af-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cd3af-127">応答</span><span class="sxs-lookup"><span data-stu-id="cd3af-127">Response</span></span>

<span data-ttu-id="cd3af-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cd3af-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd3af-130">例</span><span class="sxs-lookup"><span data-stu-id="cd3af-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd3af-131">要求</span><span class="sxs-lookup"><span data-stu-id="cd3af-131">Request</span></span>
<span data-ttu-id="cd3af-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd3af-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="cd3af-133">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd3af-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="cd3af-134">応答</span><span class="sxs-lookup"><span data-stu-id="cd3af-134">Response</span></span>
<span data-ttu-id="cd3af-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd3af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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