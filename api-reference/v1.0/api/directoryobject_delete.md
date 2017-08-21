# <a name="delete-directoryobject"></a><span data-ttu-id="53119-101">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="53119-101">Delete directoryObject</span></span>

<span data-ttu-id="53119-102">directoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="53119-102">Deletes a directoryObject.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53119-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="53119-103">Prerequisites</span></span>
<span data-ttu-id="53119-104">この API を実行するには、以下の**スコープ**が必要です。_Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="53119-104">The following **scopes** is required to execute this API: _Directory.AccessAsUser.All_</span></span>

<span data-ttu-id="53119-p101">**注:**ユーザー、グループ、および連絡先は、ディレクトリ オブジェクトの種類です。結果としてユーザーを削除する必要がある場合、次の**スコープ**を使用する必要があります。_User.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="53119-p101">**NOTE:** Users, groups, and contacts are types of directory object. As a result,if you need to delete users, the following **scope** can and should be used: _User.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="53119-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53119-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="53119-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53119-108">Request headers</span></span>
| <span data-ttu-id="53119-109">名前</span><span class="sxs-lookup"><span data-stu-id="53119-109">Name</span></span>       | <span data-ttu-id="53119-110">型</span><span class="sxs-lookup"><span data-stu-id="53119-110">Type</span></span> | <span data-ttu-id="53119-111">説明</span><span class="sxs-lookup"><span data-stu-id="53119-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53119-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="53119-112">Authorization</span></span>  | <span data-ttu-id="53119-113">string</span><span class="sxs-lookup"><span data-stu-id="53119-113">string</span></span>  | <span data-ttu-id="53119-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53119-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53119-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="53119-116">Request body</span></span>
<span data-ttu-id="53119-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53119-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53119-118">応答</span><span class="sxs-lookup"><span data-stu-id="53119-118">Response</span></span>

<span data-ttu-id="53119-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="53119-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53119-121">例</span><span class="sxs-lookup"><span data-stu-id="53119-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53119-122">要求</span><span class="sxs-lookup"><span data-stu-id="53119-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="53119-123">応答</span><span class="sxs-lookup"><span data-stu-id="53119-123">Response</span></span>

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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->