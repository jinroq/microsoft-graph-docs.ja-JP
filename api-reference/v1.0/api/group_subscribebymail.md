# <a name="group-subscribebymail"></a><span data-ttu-id="93d3f-101">グループ: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="93d3f-101">group: subscribeByMail</span></span>

<span data-ttu-id="93d3f-p101">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="93d3f-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d3f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93d3f-104">Permissions</span></span>
<span data-ttu-id="93d3f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93d3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="93d3f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93d3f-107">Permission type</span></span>      | <span data-ttu-id="93d3f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93d3f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d3f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93d3f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="93d3f-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d3f-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93d3f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93d3f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d3f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93d3f-112">Not supported.</span></span>    |
|<span data-ttu-id="93d3f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93d3f-113">Application</span></span> | <span data-ttu-id="93d3f-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d3f-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93d3f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93d3f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="93d3f-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93d3f-116">Request headers</span></span>
| <span data-ttu-id="93d3f-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93d3f-117">Header</span></span>       | <span data-ttu-id="93d3f-118">値</span><span class="sxs-lookup"><span data-stu-id="93d3f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93d3f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="93d3f-119">Authorization</span></span>  | <span data-ttu-id="93d3f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="93d3f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93d3f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="93d3f-122">Request body</span></span>
<span data-ttu-id="93d3f-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="93d3f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d3f-124">応答</span><span class="sxs-lookup"><span data-stu-id="93d3f-124">Response</span></span>
<span data-ttu-id="93d3f-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="93d3f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93d3f-127">例</span><span class="sxs-lookup"><span data-stu-id="93d3f-127">Example</span></span>
<span data-ttu-id="93d3f-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="93d3f-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="93d3f-129">要求</span><span class="sxs-lookup"><span data-stu-id="93d3f-129">Request</span></span>
<span data-ttu-id="93d3f-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="93d3f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="93d3f-131">応答</span><span class="sxs-lookup"><span data-stu-id="93d3f-131">Response</span></span>
<span data-ttu-id="93d3f-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="93d3f-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->