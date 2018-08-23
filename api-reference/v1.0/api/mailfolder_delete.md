# <a name="delete-mailfolder"></a><span data-ttu-id="230e0-101">mailFolder を削除する</span><span class="sxs-lookup"><span data-stu-id="230e0-101">Delete mailFolder</span></span>

<span data-ttu-id="230e0-102">指定した [mailFolder](../resources/mailfolder.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="230e0-102">Delete the specified mailFolder object.</span></span>

<span data-ttu-id="230e0-103">いずれかが存在する場合は、フォルダー ID または [既知のフォルダー名](../resources/mailfolder.md) のいずれかによりメール フォルダーを指定できます。</span><span class="sxs-lookup"><span data-stu-id="230e0-103">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="230e0-104">**注** 回復可能なアイテムの削除フォルダー (既知フォルダー名 `recoverableitemsdeletions` で表される) 内のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="230e0-104">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="230e0-105">詳細については、 [削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) と [削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="230e0-105">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="230e0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="230e0-106">Permissions</span></span>
<span data-ttu-id="230e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="230e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="230e0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="230e0-109">Permission type</span></span>      | <span data-ttu-id="230e0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="230e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="230e0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="230e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="230e0-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="230e0-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="230e0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="230e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="230e0-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="230e0-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="230e0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="230e0-115">Application</span></span> | <span data-ttu-id="230e0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="230e0-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="230e0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="230e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="230e0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="230e0-118">Request headers</span></span>
| <span data-ttu-id="230e0-119">名前</span><span class="sxs-lookup"><span data-stu-id="230e0-119">Name</span></span>       | <span data-ttu-id="230e0-120">型</span><span class="sxs-lookup"><span data-stu-id="230e0-120">Type</span></span> | <span data-ttu-id="230e0-121">説明</span><span class="sxs-lookup"><span data-stu-id="230e0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="230e0-122">承認</span><span class="sxs-lookup"><span data-stu-id="230e0-122">Authorization</span></span>  | <span data-ttu-id="230e0-123">文字列</span><span class="sxs-lookup"><span data-stu-id="230e0-123">string</span></span>  | <span data-ttu-id="230e0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="230e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="230e0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="230e0-126">Request body</span></span>
<span data-ttu-id="230e0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="230e0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="230e0-128">応答</span><span class="sxs-lookup"><span data-stu-id="230e0-128">Response</span></span>

<span data-ttu-id="230e0-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="230e0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="230e0-131">例</span><span class="sxs-lookup"><span data-stu-id="230e0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="230e0-132">要求</span><span class="sxs-lookup"><span data-stu-id="230e0-132">Request</span></span>
<span data-ttu-id="230e0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="230e0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="230e0-134">応答</span><span class="sxs-lookup"><span data-stu-id="230e0-134">Response</span></span>
<span data-ttu-id="230e0-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="230e0-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->