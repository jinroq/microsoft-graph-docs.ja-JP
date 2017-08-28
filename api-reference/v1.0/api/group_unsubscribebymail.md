# <a name="group-unsubscribebymail"></a><span data-ttu-id="d0c5c-101">グループ: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="d0c5c-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="d0c5c-p101">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信しなくなります。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="permissions"></a><span data-ttu-id="d0c5c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0c5c-104">Permissions</span></span>
<span data-ttu-id="d0c5c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="d0c5c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0c5c-107">Permission type</span></span>      | <span data-ttu-id="d0c5c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0c5c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0c5c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0c5c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d0c5c-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c5c-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0c5c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0c5c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0c5c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-112">Not supported.</span></span>    |
|<span data-ttu-id="d0c5c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0c5c-113">Application</span></span> | <span data-ttu-id="d0c5c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c5c-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0c5c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0c5c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="d0c5c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0c5c-116">Request headers</span></span>
| <span data-ttu-id="d0c5c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0c5c-117">Header</span></span>       | <span data-ttu-id="d0c5c-118">値</span><span class="sxs-lookup"><span data-stu-id="d0c5c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0c5c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0c5c-119">Authorization</span></span>  | <span data-ttu-id="d0c5c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0c5c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0c5c-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d0c5c-123">応答</span><span class="sxs-lookup"><span data-stu-id="d0c5c-123">Response</span></span>
<span data-ttu-id="d0c5c-p104">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c5c-126">例</span><span class="sxs-lookup"><span data-stu-id="d0c5c-126">Example</span></span>
<span data-ttu-id="d0c5c-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d0c5c-128">要求</span><span class="sxs-lookup"><span data-stu-id="d0c5c-128">Request</span></span>
<span data-ttu-id="d0c5c-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="d0c5c-130">応答</span><span class="sxs-lookup"><span data-stu-id="d0c5c-130">Response</span></span>
<span data-ttu-id="d0c5c-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d0c5c-131">Here is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
