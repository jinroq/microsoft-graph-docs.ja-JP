# <a name="remove-member"></a><span data-ttu-id="00bdb-101">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="00bdb-101">Remove member</span></span>

<span data-ttu-id="00bdb-p101">この API を使用して、**メンバー**のナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。</span><span class="sxs-lookup"><span data-stu-id="00bdb-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00bdb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="00bdb-104">Prerequisites</span></span>
<span data-ttu-id="00bdb-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="00bdb-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="00bdb-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00bdb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="00bdb-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00bdb-107">Request headers</span></span>
| <span data-ttu-id="00bdb-108">名前</span><span class="sxs-lookup"><span data-stu-id="00bdb-108">Name</span></span>       | <span data-ttu-id="00bdb-109">型</span><span class="sxs-lookup"><span data-stu-id="00bdb-109">Type</span></span> | <span data-ttu-id="00bdb-110">説明</span><span class="sxs-lookup"><span data-stu-id="00bdb-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00bdb-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="00bdb-111">Authorization</span></span>  | <span data-ttu-id="00bdb-112">string</span><span class="sxs-lookup"><span data-stu-id="00bdb-112">string</span></span>  | <span data-ttu-id="00bdb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00bdb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00bdb-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="00bdb-115">Request body</span></span>
<span data-ttu-id="00bdb-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00bdb-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00bdb-117">応答</span><span class="sxs-lookup"><span data-stu-id="00bdb-117">Response</span></span>

<span data-ttu-id="00bdb-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="00bdb-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00bdb-120">例</span><span class="sxs-lookup"><span data-stu-id="00bdb-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00bdb-121">要求</span><span class="sxs-lookup"><span data-stu-id="00bdb-121">Request</span></span>
<span data-ttu-id="00bdb-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00bdb-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="00bdb-123">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="00bdb-123">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="00bdb-124">応答</span><span class="sxs-lookup"><span data-stu-id="00bdb-124">Response</span></span>
<span data-ttu-id="00bdb-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00bdb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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