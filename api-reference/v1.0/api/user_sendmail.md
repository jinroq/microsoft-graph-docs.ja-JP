# <a name="send-mail"></a><span data-ttu-id="3c240-101">メールを送信する</span><span class="sxs-lookup"><span data-stu-id="3c240-101">Send mail</span></span>

<span data-ttu-id="3c240-p101">要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="3c240-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="3c240-104">[添付ファイル](../resources/fileattachment.md)を同じ **sendMail** アクション呼び出しに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3c240-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c240-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c240-105">Permissions</span></span>
<span data-ttu-id="3c240-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c240-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3c240-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c240-108">Permission type</span></span>      | <span data-ttu-id="3c240-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c240-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c240-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c240-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c240-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3c240-111">Mail.Send</span></span>    |
|<span data-ttu-id="3c240-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c240-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c240-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3c240-113">Mail.Send</span></span>    |
|<span data-ttu-id="3c240-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c240-114">Application</span></span> | <span data-ttu-id="3c240-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3c240-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c240-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c240-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="3c240-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c240-117">Request headers</span></span>
| <span data-ttu-id="3c240-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c240-118">Header</span></span>       | <span data-ttu-id="3c240-119">値</span><span class="sxs-lookup"><span data-stu-id="3c240-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c240-120">承認</span><span class="sxs-lookup"><span data-stu-id="3c240-120">Authorization</span></span>  | <span data-ttu-id="3c240-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3c240-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c240-123">コンテンツ-種類</span><span class="sxs-lookup"><span data-stu-id="3c240-123">Content-Type</span></span>  | <span data-ttu-id="3c240-124">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="3c240-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c240-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c240-125">Request body</span></span>
<span data-ttu-id="3c240-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3c240-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c240-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3c240-127">Parameter</span></span>    | <span data-ttu-id="3c240-128">型</span><span class="sxs-lookup"><span data-stu-id="3c240-128">Type</span></span>   |<span data-ttu-id="3c240-129">説明</span><span class="sxs-lookup"><span data-stu-id="3c240-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c240-130">メッセージ</span><span class="sxs-lookup"><span data-stu-id="3c240-130">message</span></span>|[<span data-ttu-id="3c240-131">メッセージ</span><span class="sxs-lookup"><span data-stu-id="3c240-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="3c240-p104">送信するメッセージです。必須。</span><span class="sxs-lookup"><span data-stu-id="3c240-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="3c240-134">SavetoSentItems</span><span class="sxs-lookup"><span data-stu-id="3c240-134">SavetoSentItems</span></span>|<span data-ttu-id="3c240-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="3c240-135">Boolean</span></span>|<span data-ttu-id="3c240-p105">[送信済みアイテム] 内のメッセージを保存するかどうかを示します。パラメーターを false にする場合にのみ指定します。既定では true です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3c240-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3c240-139">応答</span><span class="sxs-lookup"><span data-stu-id="3c240-139">Response</span></span>

<span data-ttu-id="3c240-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3c240-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c240-142">例</span><span class="sxs-lookup"><span data-stu-id="3c240-142">Example</span></span>
<span data-ttu-id="3c240-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3c240-143">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="3c240-144">要求 1</span><span class="sxs-lookup"><span data-stu-id="3c240-144">Request 1</span></span>
<span data-ttu-id="3c240-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c240-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response-1"></a><span data-ttu-id="3c240-146">応答 1</span><span class="sxs-lookup"><span data-stu-id="3c240-146">Response 1</span></span>
<span data-ttu-id="3c240-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3c240-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="3c240-148">要求 2</span><span class="sxs-lookup"><span data-stu-id="3c240-148">Request 2</span></span>
<span data-ttu-id="3c240-149">次の例では、カスタムのインターネット メッセージ ヘッダーを持つメッセージを作成し、メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="3c240-149">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="3c240-150">応答 2</span><span class="sxs-lookup"><span data-stu-id="3c240-150">Response 2</span></span>
<span data-ttu-id="3c240-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3c240-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
