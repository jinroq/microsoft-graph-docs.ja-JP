# <a name="group-removefavorite"></a><span data-ttu-id="78204-101">グループ: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="78204-101">group: removeFavorite</span></span>
<span data-ttu-id="78204-p101">現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="78204-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="78204-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78204-104">Permissions</span></span>
<span data-ttu-id="78204-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78204-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78204-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78204-107">Permission type</span></span>      | <span data-ttu-id="78204-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78204-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78204-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78204-109">Delegated (work or school account)</span></span> | <span data-ttu-id="78204-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78204-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="78204-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78204-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78204-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78204-112">Not supported.</span></span>    |
|<span data-ttu-id="78204-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78204-113">Application</span></span> | <span data-ttu-id="78204-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78204-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78204-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78204-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="78204-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78204-116">Request headers</span></span>
| <span data-ttu-id="78204-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78204-117">Header</span></span>       | <span data-ttu-id="78204-118">値</span><span class="sxs-lookup"><span data-stu-id="78204-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78204-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="78204-119">Authorization</span></span>  | <span data-ttu-id="78204-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78204-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78204-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="78204-122">Request body</span></span>
<span data-ttu-id="78204-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78204-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78204-124">応答</span><span class="sxs-lookup"><span data-stu-id="78204-124">Response</span></span>
<span data-ttu-id="78204-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="78204-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78204-127">例</span><span class="sxs-lookup"><span data-stu-id="78204-127">Example</span></span>
<span data-ttu-id="78204-128">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="78204-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="78204-129">要求</span><span class="sxs-lookup"><span data-stu-id="78204-129">Request</span></span>
<span data-ttu-id="78204-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78204-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="78204-131">応答</span><span class="sxs-lookup"><span data-stu-id="78204-131">Response</span></span>
<span data-ttu-id="78204-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78204-132">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->