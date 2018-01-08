# <a name="get-conversation-thread"></a><span data-ttu-id="a2933-101">会話スレッドを取得する</span><span class="sxs-lookup"><span data-stu-id="a2933-101">Get conversation thread</span></span>
<span data-ttu-id="a2933-102">[thread](../resources/conversationthread.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2933-102">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2933-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2933-103">Permissions</span></span>
<span data-ttu-id="a2933-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2933-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2933-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2933-106">Permission type</span></span>      | <span data-ttu-id="a2933-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2933-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2933-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2933-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a2933-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2933-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2933-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2933-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2933-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2933-111">Not supported.</span></span>    |
|<span data-ttu-id="a2933-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2933-112">Application</span></span> | <span data-ttu-id="a2933-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2933-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2933-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2933-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2933-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2933-115">Optional query parameters</span></span>
<span data-ttu-id="a2933-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2933-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2933-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2933-117">Request headers</span></span>
| <span data-ttu-id="a2933-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2933-118">Header</span></span>       | <span data-ttu-id="a2933-119">値</span><span class="sxs-lookup"><span data-stu-id="a2933-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2933-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2933-120">Authorization</span></span>  | <span data-ttu-id="a2933-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2933-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2933-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2933-123">Request body</span></span>
<span data-ttu-id="a2933-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2933-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2933-125">応答</span><span class="sxs-lookup"><span data-stu-id="a2933-125">Response</span></span>
<span data-ttu-id="a2933-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2933-126">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2933-127">例</span><span class="sxs-lookup"><span data-stu-id="a2933-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a2933-128">要求</span><span class="sxs-lookup"><span data-stu-id="a2933-128">Request</span></span>
<span data-ttu-id="a2933-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2933-129">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="a2933-130">応答</span><span class="sxs-lookup"><span data-stu-id="a2933-130">Response</span></span>
<span data-ttu-id="a2933-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2933-131">The following is an example of a response.</span></span>
><span data-ttu-id="a2933-132">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a2933-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a2933-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2933-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
