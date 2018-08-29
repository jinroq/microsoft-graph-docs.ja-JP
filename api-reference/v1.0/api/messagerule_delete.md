# <a name="delete-messagerule"></a><span data-ttu-id="81e12-101">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="81e12-101">Delete messageRule</span></span>


<span data-ttu-id="81e12-102">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="81e12-102">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81e12-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81e12-103">Permissions</span></span>
<span data-ttu-id="81e12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81e12-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81e12-106">Permission type</span></span>      | <span data-ttu-id="81e12-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81e12-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81e12-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81e12-108">Delegated (work or school account)</span></span> | <span data-ttu-id="81e12-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e12-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="81e12-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81e12-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81e12-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e12-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="81e12-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81e12-112">Application</span></span> | <span data-ttu-id="81e12-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81e12-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81e12-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81e12-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81e12-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81e12-115">Request headers</span></span>
| <span data-ttu-id="81e12-116">名前</span><span class="sxs-lookup"><span data-stu-id="81e12-116">Name</span></span>       | <span data-ttu-id="81e12-117">説明</span><span class="sxs-lookup"><span data-stu-id="81e12-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81e12-118">承認</span><span class="sxs-lookup"><span data-stu-id="81e12-118">Authorization</span></span>  | <span data-ttu-id="81e12-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81e12-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="81e12-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="81e12-121">Request body</span></span>
<span data-ttu-id="81e12-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="81e12-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="81e12-123">応答</span><span class="sxs-lookup"><span data-stu-id="81e12-123">Response</span></span>
<span data-ttu-id="81e12-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="81e12-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81e12-126">例</span><span class="sxs-lookup"><span data-stu-id="81e12-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81e12-127">要求</span><span class="sxs-lookup"><span data-stu-id="81e12-127">Request</span></span>
<span data-ttu-id="81e12-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81e12-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="81e12-129">応答</span><span class="sxs-lookup"><span data-stu-id="81e12-129">Response</span></span>
<span data-ttu-id="81e12-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="81e12-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->