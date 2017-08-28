# <a name="delete-a-group-setting"></a><span data-ttu-id="6a233-101">グループ設定の削除</span><span class="sxs-lookup"><span data-stu-id="6a233-101">Delete a group setting</span></span>

<span data-ttu-id="6a233-102">グループ設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a233-102">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a233-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a233-103">Permissions</span></span>

<span data-ttu-id="6a233-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="6a233-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a233-106">Permission type</span></span>      | <span data-ttu-id="6a233-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a233-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a233-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a233-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6a233-109">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a233-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a233-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a233-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a233-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a233-111">Not supported.</span></span>    |
|<span data-ttu-id="6a233-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a233-112">Application</span></span> | <span data-ttu-id="6a233-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a233-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a233-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a233-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="6a233-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a233-115">Request headers</span></span>

| <span data-ttu-id="6a233-116">名前</span><span class="sxs-lookup"><span data-stu-id="6a233-116">Name</span></span> | <span data-ttu-id="6a233-117">説明</span><span class="sxs-lookup"><span data-stu-id="6a233-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6a233-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a233-118">Authorization</span></span>  | <span data-ttu-id="6a233-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a233-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a233-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a233-121">Content-Type</span></span>  | <span data-ttu-id="6a233-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6a233-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a233-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a233-123">Request body</span></span>
<span data-ttu-id="6a233-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a233-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a233-125">応答</span><span class="sxs-lookup"><span data-stu-id="6a233-125">Response</span></span>

<span data-ttu-id="6a233-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6a233-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a233-128">例</span><span class="sxs-lookup"><span data-stu-id="6a233-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a233-129">要求</span><span class="sxs-lookup"><span data-stu-id="6a233-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="6a233-130">応答</span><span class="sxs-lookup"><span data-stu-id="6a233-130">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->