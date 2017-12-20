# <a name="list-threads"></a><span data-ttu-id="d90e1-101">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d90e1-101">List threads</span></span>
<span data-ttu-id="d90e1-102">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="d90e1-102">Get all the threads of a group.</span></span>

><span data-ttu-id="d90e1-103">注:[会話のすべてのスレッドを取得する](conversation_list_threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="d90e1-103">Note: You can also [get all the threads of a conversation](conversation_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d90e1-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d90e1-104">Permissions</span></span>
<span data-ttu-id="d90e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d90e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d90e1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d90e1-107">Permission type</span></span>      | <span data-ttu-id="d90e1-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d90e1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d90e1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d90e1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d90e1-110">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d90e1-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d90e1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d90e1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d90e1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90e1-112">Not supported.</span></span>    |
|<span data-ttu-id="d90e1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d90e1-113">Application</span></span> | <span data-ttu-id="d90e1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90e1-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d90e1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d90e1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d90e1-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d90e1-116">Optional query parameters</span></span>
<span data-ttu-id="d90e1-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d90e1-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d90e1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d90e1-118">Request headers</span></span>
| <span data-ttu-id="d90e1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d90e1-119">Header</span></span>       | <span data-ttu-id="d90e1-120">値</span><span class="sxs-lookup"><span data-stu-id="d90e1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d90e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d90e1-121">Authorization</span></span>  | <span data-ttu-id="d90e1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d90e1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d90e1-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d90e1-124">Request body</span></span>
<span data-ttu-id="d90e1-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d90e1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d90e1-126">応答</span><span class="sxs-lookup"><span data-stu-id="d90e1-126">Response</span></span>
<span data-ttu-id="d90e1-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ConversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d90e1-127">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90e1-128">例</span><span class="sxs-lookup"><span data-stu-id="d90e1-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d90e1-129">要求</span><span class="sxs-lookup"><span data-stu-id="d90e1-129">Request</span></span>
<span data-ttu-id="d90e1-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d90e1-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="d90e1-131">応答</span><span class="sxs-lookup"><span data-stu-id="d90e1-131">Response</span></span>
<span data-ttu-id="d90e1-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d90e1-132">The following is an example of a response.</span></span>
><span data-ttu-id="d90e1-133">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d90e1-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d90e1-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d90e1-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
