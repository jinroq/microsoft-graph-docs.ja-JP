# <a name="delete-an-activity"></a><span data-ttu-id="a192d-101">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="a192d-101">Delete an activity</span></span>

<span data-ttu-id="a192d-102">アプリの既存のユーザー アクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="a192d-102">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a192d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a192d-103">Permissions</span></span>

<span data-ttu-id="a192d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a192d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a192d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a192d-106">Permission type</span></span>      | <span data-ttu-id="a192d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a192d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a192d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a192d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a192d-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a192d-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a192d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a192d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a192d-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a192d-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a192d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a192d-112">Application</span></span> | <span data-ttu-id="a192d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a192d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a192d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a192d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a192d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a192d-115">Request headers</span></span>

|<span data-ttu-id="a192d-116">名前</span><span class="sxs-lookup"><span data-stu-id="a192d-116">Name</span></span> | <span data-ttu-id="a192d-117">型</span><span class="sxs-lookup"><span data-stu-id="a192d-117">Type</span></span> | <span data-ttu-id="a192d-118">説明</span><span class="sxs-lookup"><span data-stu-id="a192d-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a192d-119">承認</span><span class="sxs-lookup"><span data-stu-id="a192d-119">Authorization</span></span> | <span data-ttu-id="a192d-120">文字列</span><span class="sxs-lookup"><span data-stu-id="a192d-120">string</span></span> | <span data-ttu-id="a192d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a192d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a192d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a192d-123">Request body</span></span>

<span data-ttu-id="a192d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="a192d-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="a192d-125">応答</span><span class="sxs-lookup"><span data-stu-id="a192d-125">Response</span></span>

<span data-ttu-id="a192d-126">成功すると、履歴項目が削除された場合、このメソッドは `204 No Content`  応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a192d-126">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="a192d-127">例</span><span class="sxs-lookup"><span data-stu-id="a192d-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a192d-128">要求</span><span class="sxs-lookup"><span data-stu-id="a192d-128">Request</span></span>

<span data-ttu-id="a192d-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a192d-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="a192d-130">応答</span><span class="sxs-lookup"><span data-stu-id="a192d-130">Response</span></span>

<span data-ttu-id="a192d-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a192d-131">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->