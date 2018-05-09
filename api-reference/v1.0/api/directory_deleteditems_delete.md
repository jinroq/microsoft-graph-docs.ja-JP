# <a name="permanently-delete-item"></a><span data-ttu-id="e7b37-101">アイテムを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="e7b37-101">Permanently delete item</span></span>

<span data-ttu-id="e7b37-102">[[削除済みアイテム]](../resources/directory.md) からアイテムを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="e7b37-102">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e7b37-103">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e7b37-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="e7b37-104">[削除済みアイテム] から、アイテムを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="e7b37-104">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="e7b37-105">ただし、アイテムを完全に削除すると、そのアイテムを復元することが**不可能**になります。</span><span class="sxs-lookup"><span data-stu-id="e7b37-105">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7b37-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7b37-106">Permissions</span></span>
<span data-ttu-id="e7b37-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7b37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="e7b37-109">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="e7b37-109">For users:</span></span>

|<span data-ttu-id="e7b37-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7b37-110">Permission type</span></span>      | <span data-ttu-id="e7b37-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7b37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7b37-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7b37-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7b37-113">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7b37-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e7b37-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7b37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7b37-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7b37-115">Not supported.</span></span> |
|<span data-ttu-id="e7b37-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7b37-116">Application</span></span> | <span data-ttu-id="e7b37-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b37-117">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="e7b37-118">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="e7b37-118">For groups:</span></span>

|<span data-ttu-id="e7b37-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7b37-119">Permission type</span></span>      | <span data-ttu-id="e7b37-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7b37-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7b37-121">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7b37-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e7b37-122">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7b37-122">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e7b37-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7b37-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7b37-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7b37-124">Not supported.</span></span>    |
|<span data-ttu-id="e7b37-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7b37-125">Application</span></span> | <span data-ttu-id="e7b37-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b37-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7b37-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7b37-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e7b37-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7b37-128">Request headers</span></span>
| <span data-ttu-id="e7b37-129">名前</span><span class="sxs-lookup"><span data-stu-id="e7b37-129">Name</span></span>       | <span data-ttu-id="e7b37-130">説明</span><span class="sxs-lookup"><span data-stu-id="e7b37-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7b37-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b37-131">Authorization</span></span>  | <span data-ttu-id="e7b37-132">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="e7b37-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e7b37-133">Accept</span><span class="sxs-lookup"><span data-stu-id="e7b37-133">Accept</span></span>  | <span data-ttu-id="e7b37-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b37-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7b37-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7b37-135">Request body</span></span>
<span data-ttu-id="e7b37-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7b37-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7b37-137">応答</span><span class="sxs-lookup"><span data-stu-id="e7b37-137">Response</span></span>

<span data-ttu-id="e7b37-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e7b37-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b37-140">例</span><span class="sxs-lookup"><span data-stu-id="e7b37-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7b37-141">要求</span><span class="sxs-lookup"><span data-stu-id="e7b37-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="e7b37-142">応答</span><span class="sxs-lookup"><span data-stu-id="e7b37-142">Response</span></span>
<span data-ttu-id="e7b37-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7b37-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->