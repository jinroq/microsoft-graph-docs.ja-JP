# <a name="post-forward"></a><span data-ttu-id="0528b-101">投稿: 転送</span><span class="sxs-lookup"><span data-stu-id="0528b-101">post: forward</span></span>

<span data-ttu-id="0528b-p101">受信者に投稿を転送します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="0528b-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0528b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0528b-104">Permissions</span></span>
<span data-ttu-id="0528b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0528b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0528b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0528b-107">Permission type</span></span>      | <span data-ttu-id="0528b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0528b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0528b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0528b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0528b-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0528b-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0528b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0528b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0528b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0528b-112">Not supported.</span></span>    |
|<span data-ttu-id="0528b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0528b-113">Application</span></span> | <span data-ttu-id="0528b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0528b-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0528b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0528b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="0528b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0528b-116">Request headers</span></span>
| <span data-ttu-id="0528b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0528b-117">Header</span></span>       | <span data-ttu-id="0528b-118">値</span><span class="sxs-lookup"><span data-stu-id="0528b-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0528b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0528b-119">Authorization</span></span>  | <span data-ttu-id="0528b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0528b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0528b-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="0528b-122">Request body</span></span>
<span data-ttu-id="0528b-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0528b-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0528b-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0528b-124">Parameter</span></span>    | <span data-ttu-id="0528b-125">型</span><span class="sxs-lookup"><span data-stu-id="0528b-125">Type</span></span>   |<span data-ttu-id="0528b-126">説明</span><span class="sxs-lookup"><span data-stu-id="0528b-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0528b-127">comment</span><span class="sxs-lookup"><span data-stu-id="0528b-127">comment</span></span>|<span data-ttu-id="0528b-128">String</span><span class="sxs-lookup"><span data-stu-id="0528b-128">String</span></span>|<span data-ttu-id="0528b-129">投稿と共に転送されるオプションのコメント。</span><span class="sxs-lookup"><span data-stu-id="0528b-129">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="0528b-130">toRecipients</span><span class="sxs-lookup"><span data-stu-id="0528b-130">toRecipients</span></span>|<span data-ttu-id="0528b-131">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="0528b-131">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="0528b-132">スレッドの転送先となる受信者。</span><span class="sxs-lookup"><span data-stu-id="0528b-132">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="0528b-133">応答</span><span class="sxs-lookup"><span data-stu-id="0528b-133">Response</span></span>

<span data-ttu-id="0528b-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0528b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0528b-136">例</span><span class="sxs-lookup"><span data-stu-id="0528b-136">Example</span></span>
<span data-ttu-id="0528b-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0528b-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0528b-138">要求</span><span class="sxs-lookup"><span data-stu-id="0528b-138">Request</span></span>
<span data-ttu-id="0528b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0528b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="0528b-140">応答</span><span class="sxs-lookup"><span data-stu-id="0528b-140">Response</span></span>
<span data-ttu-id="0528b-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0528b-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
