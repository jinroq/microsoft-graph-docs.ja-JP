---
title: 'group: renew'
description: グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b334c863cd13cee7b046d7e7701302b0607b59f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014754"
---
# <a name="group-renew"></a><span data-ttu-id="da537-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="da537-104">group: renew</span></span>

<span data-ttu-id="da537-105">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="da537-105">Renews a group's expiration.</span></span> <span data-ttu-id="da537-106">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="da537-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="da537-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da537-107">Permissions</span></span>

<span data-ttu-id="da537-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da537-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="da537-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da537-110">Permission type</span></span>      | <span data-ttu-id="da537-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da537-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da537-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da537-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da537-113">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da537-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="da537-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da537-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da537-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="da537-115">Not supported</span></span> |
|<span data-ttu-id="da537-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da537-116">Application</span></span> | <span data-ttu-id="da537-117">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da537-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da537-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da537-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="da537-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da537-119">Request headers</span></span>
| <span data-ttu-id="da537-120">名前</span><span class="sxs-lookup"><span data-stu-id="da537-120">Name</span></span>       | <span data-ttu-id="da537-121">説明</span><span class="sxs-lookup"><span data-stu-id="da537-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da537-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da537-122">Authorization</span></span>  | <span data-ttu-id="da537-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="da537-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="da537-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="da537-124">Request body</span></span>

<span data-ttu-id="da537-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="da537-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da537-126">応答</span><span class="sxs-lookup"><span data-stu-id="da537-126">Response</span></span>

<span data-ttu-id="da537-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="da537-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da537-129">例</span><span class="sxs-lookup"><span data-stu-id="da537-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da537-130">要求</span><span class="sxs-lookup"><span data-stu-id="da537-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="da537-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="da537-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da537-132">C#</span><span class="sxs-lookup"><span data-stu-id="da537-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da537-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="da537-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da537-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="da537-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da537-135">Java</span><span class="sxs-lookup"><span data-stu-id="da537-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da537-136">応答</span><span class="sxs-lookup"><span data-stu-id="da537-136">Response</span></span>
<span data-ttu-id="da537-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da537-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
