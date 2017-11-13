# <a name="message-forward"></a><span data-ttu-id="3762b-101">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="3762b-101">message: forward</span></span>

<span data-ttu-id="3762b-p101">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="3762b-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3762b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3762b-104">Permissions</span></span>
<span data-ttu-id="3762b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3762b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3762b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3762b-107">Permission type</span></span>      | <span data-ttu-id="3762b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3762b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3762b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3762b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3762b-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3762b-110">Mail.Send</span></span>    |
|<span data-ttu-id="3762b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3762b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3762b-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3762b-112">Mail.Send</span></span>    |
|<span data-ttu-id="3762b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3762b-113">Application</span></span> | <span data-ttu-id="3762b-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3762b-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3762b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3762b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="3762b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3762b-116">Request headers</span></span>
| <span data-ttu-id="3762b-117">名前</span><span class="sxs-lookup"><span data-stu-id="3762b-117">Name</span></span>       | <span data-ttu-id="3762b-118">型</span><span class="sxs-lookup"><span data-stu-id="3762b-118">Type</span></span> | <span data-ttu-id="3762b-119">説明</span><span class="sxs-lookup"><span data-stu-id="3762b-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3762b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3762b-120">Authorization</span></span>  | <span data-ttu-id="3762b-121">string</span><span class="sxs-lookup"><span data-stu-id="3762b-121">string</span></span>  | <span data-ttu-id="3762b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3762b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3762b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3762b-124">Content-Type</span></span> | <span data-ttu-id="3762b-125">string</span><span class="sxs-lookup"><span data-stu-id="3762b-125">string</span></span>  | <span data-ttu-id="3762b-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="3762b-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3762b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3762b-128">Request body</span></span>
<span data-ttu-id="3762b-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3762b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3762b-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3762b-130">Parameter</span></span>    | <span data-ttu-id="3762b-131">型</span><span class="sxs-lookup"><span data-stu-id="3762b-131">Type</span></span>   |<span data-ttu-id="3762b-132">説明</span><span class="sxs-lookup"><span data-stu-id="3762b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3762b-133">comment</span><span class="sxs-lookup"><span data-stu-id="3762b-133">comment</span></span>|<span data-ttu-id="3762b-134">String</span><span class="sxs-lookup"><span data-stu-id="3762b-134">String</span></span>|<span data-ttu-id="3762b-p105">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3762b-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="3762b-137">toRecipients</span><span class="sxs-lookup"><span data-stu-id="3762b-137">toRecipients</span></span>|<span data-ttu-id="3762b-138">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="3762b-138">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="3762b-139">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="3762b-139">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="3762b-140">応答</span><span class="sxs-lookup"><span data-stu-id="3762b-140">Response</span></span>

<span data-ttu-id="3762b-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3762b-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3762b-143">例</span><span class="sxs-lookup"><span data-stu-id="3762b-143">Example</span></span>
<span data-ttu-id="3762b-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3762b-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3762b-145">要求</span><span class="sxs-lookup"><span data-stu-id="3762b-145">Request</span></span>
<span data-ttu-id="3762b-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3762b-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="3762b-147">応答</span><span class="sxs-lookup"><span data-stu-id="3762b-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3762b-148">応答</span><span class="sxs-lookup"><span data-stu-id="3762b-148">Response</span></span>
<span data-ttu-id="3762b-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3762b-149">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
