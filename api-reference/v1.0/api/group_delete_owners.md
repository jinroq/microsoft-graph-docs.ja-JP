# <a name="remove-owner"></a><span data-ttu-id="6030a-101">所有者の削除</span><span class="sxs-lookup"><span data-stu-id="6030a-101">Remove owner</span></span>
<span data-ttu-id="6030a-102">この API を使用して、所有者のナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループから所有者を削除できます。</span><span class="sxs-lookup"><span data-stu-id="6030a-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="6030a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6030a-103">Permissions</span></span>
<span data-ttu-id="6030a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6030a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6030a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6030a-106">Permission type</span></span>      | <span data-ttu-id="6030a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6030a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6030a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6030a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6030a-109">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6030a-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6030a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6030a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6030a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6030a-111">Not supported.</span></span>    |
|<span data-ttu-id="6030a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6030a-112">Application</span></span> | <span data-ttu-id="6030a-113">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6030a-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6030a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6030a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6030a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6030a-115">Request headers</span></span>
| <span data-ttu-id="6030a-116">名前</span><span class="sxs-lookup"><span data-stu-id="6030a-116">Name</span></span>       | <span data-ttu-id="6030a-117">型</span><span class="sxs-lookup"><span data-stu-id="6030a-117">Type</span></span> | <span data-ttu-id="6030a-118">説明</span><span class="sxs-lookup"><span data-stu-id="6030a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6030a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6030a-119">Authorization</span></span>  | <span data-ttu-id="6030a-120">string</span><span class="sxs-lookup"><span data-stu-id="6030a-120">string</span></span>  | <span data-ttu-id="6030a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6030a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6030a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6030a-123">Request body</span></span>
<span data-ttu-id="6030a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6030a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6030a-125">応答</span><span class="sxs-lookup"><span data-stu-id="6030a-125">Response</span></span>
<span data-ttu-id="6030a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6030a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6030a-128">例</span><span class="sxs-lookup"><span data-stu-id="6030a-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6030a-129">要求</span><span class="sxs-lookup"><span data-stu-id="6030a-129">Request</span></span>
<span data-ttu-id="6030a-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6030a-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="6030a-131">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="6030a-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="6030a-132">応答</span><span class="sxs-lookup"><span data-stu-id="6030a-132">Response</span></span>
<span data-ttu-id="6030a-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6030a-133">The following is an example of a response.</span></span>
><span data-ttu-id="6030a-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6030a-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6030a-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6030a-135">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
