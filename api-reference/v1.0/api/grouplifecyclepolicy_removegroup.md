# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="248a4-101">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="248a4-101">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="248a4-102">ライフ サイクル ポリシーからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="248a4-102">Removes a group from a web.</span></span>

## <a name="permissions"></a><span data-ttu-id="248a4-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="248a4-103">Permissions</span></span>

<span data-ttu-id="248a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="248a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="248a4-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="248a4-106">Permission type</span></span>      | <span data-ttu-id="248a4-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="248a4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="248a4-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="248a4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="248a4-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="248a4-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="248a4-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="248a4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="248a4-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="248a4-111">Not supported.</span></span>    |
|<span data-ttu-id="248a4-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="248a4-112">Application</span></span> | <span data-ttu-id="248a4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="248a4-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="248a4-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="248a4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="248a4-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="248a4-115">Request headers</span></span>

| <span data-ttu-id="248a4-116">名前</span><span class="sxs-lookup"><span data-stu-id="248a4-116">Name</span></span> | <span data-ttu-id="248a4-117">説明</span><span class="sxs-lookup"><span data-stu-id="248a4-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="248a4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="248a4-118">Authorization</span></span> | <span data-ttu-id="248a4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="248a4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="248a4-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="248a4-121">Content-Type</span></span>  | <span data-ttu-id="248a4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="248a4-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="248a4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="248a4-123">Request body</span></span>
<span data-ttu-id="248a4-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="248a4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="248a4-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="248a4-125">Parameter</span></span> | <span data-ttu-id="248a4-126">型</span><span class="sxs-lookup"><span data-stu-id="248a4-126">Type</span></span> | <span data-ttu-id="248a4-127">説明</span><span class="sxs-lookup"><span data-stu-id="248a4-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="248a4-128">groupId</span><span class="sxs-lookup"><span data-stu-id="248a4-128">groupId</span></span>|<span data-ttu-id="248a4-129">Guid</span><span class="sxs-lookup"><span data-stu-id="248a4-129">Guid</span></span>| <span data-ttu-id="248a4-130">ポリシーから削除するグループの ID です。</span><span class="sxs-lookup"><span data-stu-id="248a4-130">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="248a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="248a4-131">Response</span></span>

<span data-ttu-id="248a4-132">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="248a4-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="248a4-133">グループがポリシーから削除された場合、応答本体で、**true**値が返されます。</span><span class="sxs-lookup"><span data-stu-id="248a4-133">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="248a4-134">それ以外の場合、返信の本文で **false** 値が返されます。</span><span class="sxs-lookup"><span data-stu-id="248a4-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="248a4-135">例</span><span class="sxs-lookup"><span data-stu-id="248a4-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="248a4-136">要求</span><span class="sxs-lookup"><span data-stu-id="248a4-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="248a4-137">応答</span><span class="sxs-lookup"><span data-stu-id="248a4-137">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->