# <a name="add-member"></a><span data-ttu-id="e5dc0-101">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="e5dc0-101">Add member</span></span>
<span data-ttu-id="e5dc0-102">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-102">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

<span data-ttu-id="e5dc0-103">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-103">You can add users or other groups.</span></span> <span data-ttu-id="e5dc0-104">重要: Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-104">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5dc0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5dc0-105">Permissions</span></span>
<span data-ttu-id="e5dc0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e5dc0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5dc0-108">Permission type</span></span>      | <span data-ttu-id="e5dc0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5dc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5dc0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5dc0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5dc0-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5dc0-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5dc0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5dc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5dc0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-113">Not supported.</span></span>    |
|<span data-ttu-id="e5dc0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5dc0-114">Application</span></span> | <span data-ttu-id="e5dc0-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5dc0-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5dc0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5dc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e5dc0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5dc0-117">Request headers</span></span>
| <span data-ttu-id="e5dc0-118">名前</span><span class="sxs-lookup"><span data-stu-id="e5dc0-118">Name</span></span>       | <span data-ttu-id="e5dc0-119">型</span><span class="sxs-lookup"><span data-stu-id="e5dc0-119">Type</span></span> | <span data-ttu-id="e5dc0-120">説明</span><span class="sxs-lookup"><span data-stu-id="e5dc0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5dc0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5dc0-121">Authorization</span></span>  | <span data-ttu-id="e5dc0-122">string</span><span class="sxs-lookup"><span data-stu-id="e5dc0-122">string</span></span>  | <span data-ttu-id="e5dc0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5dc0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5dc0-125">Request body</span></span>
<span data-ttu-id="e5dc0-126">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e5dc0-127">応答</span><span class="sxs-lookup"><span data-stu-id="e5dc0-127">Response</span></span>
<span data-ttu-id="e5dc0-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5dc0-130">例</span><span class="sxs-lookup"><span data-stu-id="e5dc0-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e5dc0-131">要求</span><span class="sxs-lookup"><span data-stu-id="e5dc0-131">Request</span></span>
<span data-ttu-id="e5dc0-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="e5dc0-133">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの `id` の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="e5dc0-134">応答</span><span class="sxs-lookup"><span data-stu-id="e5dc0-134">Response</span></span>
<span data-ttu-id="e5dc0-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-135">The following is an example of the response.</span></span>
><span data-ttu-id="e5dc0-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5dc0-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e5dc0-137">All the properties will be returned from an actual call.</span></span>
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