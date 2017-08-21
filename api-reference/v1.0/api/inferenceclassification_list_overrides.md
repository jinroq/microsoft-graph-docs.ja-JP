# <a name="list-overrides"></a><span data-ttu-id="83380-101">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83380-101">List overrides</span></span>

<span data-ttu-id="83380-102">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="83380-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="83380-p101">それぞれのオーバーライドは、送信者の SMTP アドレスに対応します。最初は、ユーザーにはオーバーライドはありません。</span><span class="sxs-lookup"><span data-stu-id="83380-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83380-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="83380-105">Prerequisites</span></span>
<span data-ttu-id="83380-106">この API を実行するために必要な**スコープ**は、次のとおりです。*Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="83380-106">The following **scopes** are required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="83380-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83380-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="83380-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83380-108">Request headers</span></span>
| <span data-ttu-id="83380-109">名前</span><span class="sxs-lookup"><span data-stu-id="83380-109">Name</span></span>       | <span data-ttu-id="83380-110">型</span><span class="sxs-lookup"><span data-stu-id="83380-110">Type</span></span> | <span data-ttu-id="83380-111">説明</span><span class="sxs-lookup"><span data-stu-id="83380-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83380-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="83380-112">Authorization</span></span>  | <span data-ttu-id="83380-113">string</span><span class="sxs-lookup"><span data-stu-id="83380-113">string</span></span>  | <span data-ttu-id="83380-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83380-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83380-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="83380-116">Request body</span></span>
<span data-ttu-id="83380-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83380-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83380-118">応答</span><span class="sxs-lookup"><span data-stu-id="83380-118">Response</span></span>

<span data-ttu-id="83380-p103">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトのコレクションを返します。ユーザーがオーバーライドを設定していない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="83380-p103">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="83380-121">例</span><span class="sxs-lookup"><span data-stu-id="83380-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83380-122">要求</span><span class="sxs-lookup"><span data-stu-id="83380-122">Request</span></span>
<span data-ttu-id="83380-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83380-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="83380-124">応答</span><span class="sxs-lookup"><span data-stu-id="83380-124">Response</span></span>
<span data-ttu-id="83380-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83380-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Fanny Downs",
        "address": "fannyd@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->