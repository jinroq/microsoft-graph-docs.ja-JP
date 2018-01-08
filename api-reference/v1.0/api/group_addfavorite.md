# <a name="group-addfavorite"></a><span data-ttu-id="11dcd-101">グループ: addFavorite</span><span class="sxs-lookup"><span data-stu-id="11dcd-101">group: addFavorite</span></span>
<span data-ttu-id="11dcd-p101">現在のユーザーのお気に入りのグループ一覧にグループを追加します。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="11dcd-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="11dcd-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11dcd-104">Permissions</span></span>
<span data-ttu-id="11dcd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11dcd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11dcd-107">Permission type</span></span>      | <span data-ttu-id="11dcd-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11dcd-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11dcd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11dcd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="11dcd-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dcd-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="11dcd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11dcd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11dcd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11dcd-112">Not supported.</span></span>    |
|<span data-ttu-id="11dcd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11dcd-113">Application</span></span> | <span data-ttu-id="11dcd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11dcd-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11dcd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11dcd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="11dcd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11dcd-116">Request headers</span></span>
| <span data-ttu-id="11dcd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11dcd-117">Header</span></span>       | <span data-ttu-id="11dcd-118">値</span><span class="sxs-lookup"><span data-stu-id="11dcd-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11dcd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="11dcd-119">Authorization</span></span>  | <span data-ttu-id="11dcd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11dcd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11dcd-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="11dcd-122">Prefer</span></span> | <span data-ttu-id="11dcd-123">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="11dcd-123">return=minimal.</span></span> <span data-ttu-id="11dcd-124">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="11dcd-124">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="11dcd-125">省略可能。</span><span class="sxs-lookup"><span data-stu-id="11dcd-125">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11dcd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="11dcd-126">Request body</span></span>
<span data-ttu-id="11dcd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11dcd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11dcd-128">応答</span><span class="sxs-lookup"><span data-stu-id="11dcd-128">Response</span></span>
<span data-ttu-id="11dcd-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="11dcd-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11dcd-131">例</span><span class="sxs-lookup"><span data-stu-id="11dcd-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="11dcd-132">要求</span><span class="sxs-lookup"><span data-stu-id="11dcd-132">Request</span></span>
<span data-ttu-id="11dcd-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11dcd-133">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="11dcd-134">応答</span><span class="sxs-lookup"><span data-stu-id="11dcd-134">Response</span></span>
<span data-ttu-id="11dcd-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11dcd-135">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
