# <a name="list-acceptedsenders"></a><span data-ttu-id="7f754-101">acceptedSenders のリスト化</span><span class="sxs-lookup"><span data-stu-id="7f754-101">List acceptedSenders</span></span>
<span data-ttu-id="7f754-102">このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f754-102">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="7f754-p101">承諾済み送信者リスト内のユーザーは、グループの会話を投稿することができます (要求取得 URL で識別)。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="7f754-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f754-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f754-105">Permissions</span></span>
<span data-ttu-id="7f754-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f754-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f754-108">Permission type</span></span>      | <span data-ttu-id="7f754-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f754-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f754-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f754-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f754-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f754-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f754-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f754-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f754-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f754-113">Not supported.</span></span>    |
|<span data-ttu-id="7f754-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f754-114">Application</span></span> | <span data-ttu-id="7f754-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f754-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f754-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f754-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f754-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f754-117">Optional query parameters</span></span>
<span data-ttu-id="7f754-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f754-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f754-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f754-119">Request headers</span></span>
| <span data-ttu-id="7f754-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f754-120">Header</span></span>       | <span data-ttu-id="7f754-121">値</span><span class="sxs-lookup"><span data-stu-id="7f754-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f754-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f754-122">Authorization</span></span>  | <span data-ttu-id="7f754-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f754-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f754-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f754-125">Request body</span></span>
<span data-ttu-id="7f754-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f754-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f754-127">応答</span><span class="sxs-lookup"><span data-stu-id="7f754-127">Response</span></span>
<span data-ttu-id="7f754-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f754-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f754-129">例</span><span class="sxs-lookup"><span data-stu-id="7f754-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f754-130">要求</span><span class="sxs-lookup"><span data-stu-id="7f754-130">Request</span></span>
<span data-ttu-id="7f754-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f754-131">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="7f754-132">応答</span><span class="sxs-lookup"><span data-stu-id="7f754-132">Response</span></span>
<span data-ttu-id="7f754-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f754-133">The following is an example of a response.</span></span>
><span data-ttu-id="7f754-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7f754-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f754-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f754-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->