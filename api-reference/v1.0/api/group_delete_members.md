# <a name="remove-member"></a><span data-ttu-id="e11a2-101">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="e11a2-101">Remove member</span></span>

<span data-ttu-id="e11a2-p101">この API を使用して、**メンバー**のナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。</span><span class="sxs-lookup"><span data-stu-id="e11a2-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e11a2-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e11a2-104">Permissions</span></span>
<span data-ttu-id="e11a2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e11a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e11a2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e11a2-107">Permission type</span></span>      | <span data-ttu-id="e11a2-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e11a2-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e11a2-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e11a2-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e11a2-110">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e11a2-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e11a2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e11a2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e11a2-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e11a2-112">Not supported.</span></span>    |
|<span data-ttu-id="e11a2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e11a2-113">Application</span></span> | <span data-ttu-id="e11a2-114">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e11a2-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e11a2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e11a2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e11a2-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e11a2-116">Request headers</span></span>
| <span data-ttu-id="e11a2-117">名前</span><span class="sxs-lookup"><span data-stu-id="e11a2-117">Name</span></span>       | <span data-ttu-id="e11a2-118">型</span><span class="sxs-lookup"><span data-stu-id="e11a2-118">Type</span></span> | <span data-ttu-id="e11a2-119">説明</span><span class="sxs-lookup"><span data-stu-id="e11a2-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e11a2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e11a2-120">Authorization</span></span>  | <span data-ttu-id="e11a2-121">string</span><span class="sxs-lookup"><span data-stu-id="e11a2-121">string</span></span>  | <span data-ttu-id="e11a2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e11a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e11a2-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="e11a2-124">Request body</span></span>
<span data-ttu-id="e11a2-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e11a2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e11a2-126">応答</span><span class="sxs-lookup"><span data-stu-id="e11a2-126">Response</span></span>

<span data-ttu-id="e11a2-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e11a2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e11a2-129">例</span><span class="sxs-lookup"><span data-stu-id="e11a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e11a2-130">要求</span><span class="sxs-lookup"><span data-stu-id="e11a2-130">Request</span></span>
<span data-ttu-id="e11a2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e11a2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="e11a2-132">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="e11a2-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="e11a2-133">応答</span><span class="sxs-lookup"><span data-stu-id="e11a2-133">Response</span></span>
<span data-ttu-id="e11a2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e11a2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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