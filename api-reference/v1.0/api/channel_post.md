# <a name="create-channel"></a><span data-ttu-id="5cbbc-101">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-101">Create Channel</span></span>



<span data-ttu-id="5cbbc-102">要求の本体に指定されている、マイクロソフトのチームでは、新しい[チャネル](../resources/channel.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-102">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="5cbbc-103">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="5cbbc-104">詳細についてはの[既知の問題点のリスト](../../../concepts/known_issues.md#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cbbc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5cbbc-105">Permissions</span></span>
<span data-ttu-id="5cbbc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5cbbc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5cbbc-108">Permission type</span></span>      | <span data-ttu-id="5cbbc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5cbbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cbbc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5cbbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5cbbc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cbbc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cbbc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cbbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cbbc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-113">Not supported.</span></span>    |
|<span data-ttu-id="5cbbc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5cbbc-114">Application</span></span> | <span data-ttu-id="5cbbc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cbbc-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="5cbbc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cbbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="5cbbc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cbbc-117">Request headers</span></span>
| <span data-ttu-id="5cbbc-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cbbc-118">Header</span></span>       | <span data-ttu-id="5cbbc-119">値</span><span class="sxs-lookup"><span data-stu-id="5cbbc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cbbc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cbbc-120">Authorization</span></span>  | <span data-ttu-id="5cbbc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cbbc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cbbc-123">Content-Type</span></span>  | <span data-ttu-id="5cbbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5cbbc-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cbbc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5cbbc-125">Request body</span></span>
<span data-ttu-id="5cbbc-126">要求の本文には、[チャネル](../resources/channel.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5cbbc-127">応答</span><span class="sxs-lookup"><span data-stu-id="5cbbc-127">Response</span></span>

<span data-ttu-id="5cbbc-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体での応答コードおよび[チャネル](../resources/channel.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-128">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cbbc-129">例</span><span class="sxs-lookup"><span data-stu-id="5cbbc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cbbc-130">要求</span><span class="sxs-lookup"><span data-stu-id="5cbbc-130">Request</span></span>
<span data-ttu-id="5cbbc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="5cbbc-132">応答</span><span class="sxs-lookup"><span data-stu-id="5cbbc-132">Response</span></span>
<span data-ttu-id="5cbbc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5cbbc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
