# <a name="get-team"></a><span data-ttu-id="6cd36-101">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="6cd36-101">Get team</span></span>



<span data-ttu-id="6cd36-102">プロパティと指定した[チーム](../resources/team.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6cd36-102">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cd36-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6cd36-103">Permissions</span></span>
<span data-ttu-id="6cd36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6cd36-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cd36-106">Permission type</span></span>      | <span data-ttu-id="6cd36-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cd36-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cd36-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cd36-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6cd36-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd36-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6cd36-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cd36-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cd36-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cd36-111">Not supported.</span></span>    |
|<span data-ttu-id="6cd36-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cd36-112">Application</span></span> | <span data-ttu-id="6cd36-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd36-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="6cd36-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cd36-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cd36-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6cd36-115">Optional query parameters</span></span>
<span data-ttu-id="6cd36-116">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](../../../concepts/query_parameters.md)を展開します。</span><span class="sxs-lookup"><span data-stu-id="6cd36-116">This method supports the $select and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cd36-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cd36-117">Request headers</span></span>
| <span data-ttu-id="6cd36-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cd36-118">Header</span></span>       | <span data-ttu-id="6cd36-119">値</span><span class="sxs-lookup"><span data-stu-id="6cd36-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cd36-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cd36-120">Authorization</span></span>  | <span data-ttu-id="6cd36-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6cd36-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cd36-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cd36-123">Request body</span></span>
<span data-ttu-id="6cd36-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6cd36-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cd36-125">応答</span><span class="sxs-lookup"><span data-stu-id="6cd36-125">Response</span></span>

<span data-ttu-id="6cd36-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[チーム](../resources/team.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6cd36-126">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6cd36-127">例</span><span class="sxs-lookup"><span data-stu-id="6cd36-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6cd36-128">要求</span><span class="sxs-lookup"><span data-stu-id="6cd36-128">Request</span></span>
<span data-ttu-id="6cd36-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6cd36-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="6cd36-130">応答</span><span class="sxs-lookup"><span data-stu-id="6cd36-130">Response</span></span>
<span data-ttu-id="6cd36-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6cd36-131">The following is an example of the response.</span></span> 

><span data-ttu-id="6cd36-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6cd36-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
