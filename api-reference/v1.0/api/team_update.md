# <a name="update-team"></a><span data-ttu-id="8fda5-101">チームを更新します。</span><span class="sxs-lookup"><span data-stu-id="8fda5-101">Update team</span></span>



<span data-ttu-id="8fda5-102">指定された[チーム](../resources/team.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8fda5-102">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8fda5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8fda5-103">Permissions</span></span>
<span data-ttu-id="8fda5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fda5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="8fda5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8fda5-106">Permission type</span></span>      | <span data-ttu-id="8fda5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8fda5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fda5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8fda5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8fda5-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fda5-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fda5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8fda5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fda5-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fda5-111">Not supported.</span></span>    |
|<span data-ttu-id="8fda5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8fda5-112">Application</span></span> | <span data-ttu-id="8fda5-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fda5-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="8fda5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8fda5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8fda5-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fda5-115">Request headers</span></span>
| <span data-ttu-id="8fda5-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fda5-116">Header</span></span>       | <span data-ttu-id="8fda5-117">値</span><span class="sxs-lookup"><span data-stu-id="8fda5-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fda5-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fda5-118">Authorization</span></span>  | <span data-ttu-id="8fda5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8fda5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8fda5-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fda5-121">Content-Type</span></span>  | <span data-ttu-id="8fda5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8fda5-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fda5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="8fda5-123">Request body</span></span>
<span data-ttu-id="8fda5-124">要求の本文には、[チーム](../resources/team.md)のオブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="8fda5-124">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8fda5-125">応答</span><span class="sxs-lookup"><span data-stu-id="8fda5-125">Response</span></span>

<span data-ttu-id="8fda5-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8fda5-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8fda5-127">例</span><span class="sxs-lookup"><span data-stu-id="8fda5-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8fda5-128">要求</span><span class="sxs-lookup"><span data-stu-id="8fda5-128">Request</span></span>
<span data-ttu-id="8fda5-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fda5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="8fda5-130">応答</span><span class="sxs-lookup"><span data-stu-id="8fda5-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
