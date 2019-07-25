---
title: グループの削除-Microsoft Graph API
description: Microsoft Graph API (REST) のグループリソース (エンティティ) の delete メソッドについて説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 15bd2c55fd7f5a056510a5025bc816e029267af3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890713"
---
# <a name="delete-group"></a><span data-ttu-id="f4c16-103">グループの削除</span><span class="sxs-lookup"><span data-stu-id="f4c16-103">Delete group</span></span>

<span data-ttu-id="f4c16-104">グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="f4c16-104">Delete group.</span></span>  

<span data-ttu-id="f4c16-105">削除すると、Office 365 グループが一時コンテナーに移動され、30日以内に復元できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f4c16-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="f4c16-106">それ以降、これらのユーザーは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="f4c16-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="f4c16-107">詳細については、「[deletedItems](../resources/directory.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4c16-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="f4c16-108">これは、Office 365 グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f4c16-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c16-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4c16-109">Permissions</span></span>

<span data-ttu-id="f4c16-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4c16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4c16-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4c16-112">Permission type</span></span>      | <span data-ttu-id="f4c16-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4c16-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4c16-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4c16-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4c16-115">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4c16-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f4c16-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4c16-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c16-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4c16-117">Not supported.</span></span>    |
|<span data-ttu-id="f4c16-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4c16-118">Application</span></span> | <span data-ttu-id="f4c16-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c16-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4c16-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4c16-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4c16-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4c16-121">Request headers</span></span>

| <span data-ttu-id="f4c16-122">名前</span><span class="sxs-lookup"><span data-stu-id="f4c16-122">Name</span></span>       | <span data-ttu-id="f4c16-123">型</span><span class="sxs-lookup"><span data-stu-id="f4c16-123">Type</span></span> | <span data-ttu-id="f4c16-124">説明</span><span class="sxs-lookup"><span data-stu-id="f4c16-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4c16-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c16-125">Authorization</span></span>  | <span data-ttu-id="f4c16-126">string</span><span class="sxs-lookup"><span data-stu-id="f4c16-126">string</span></span>  | <span data-ttu-id="f4c16-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f4c16-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4c16-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4c16-129">Request body</span></span>

<span data-ttu-id="f4c16-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4c16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c16-131">応答</span><span class="sxs-lookup"><span data-stu-id="f4c16-131">Response</span></span>

<span data-ttu-id="f4c16-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f4c16-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c16-134">例</span><span class="sxs-lookup"><span data-stu-id="f4c16-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4c16-135">要求</span><span class="sxs-lookup"><span data-stu-id="f4c16-135">Request</span></span>

<span data-ttu-id="f4c16-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4c16-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f4c16-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f4c16-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4c16-138">C#</span><span class="sxs-lookup"><span data-stu-id="f4c16-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4c16-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4c16-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4c16-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="f4c16-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4c16-141">Java</span><span class="sxs-lookup"><span data-stu-id="f4c16-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4c16-142">応答</span><span class="sxs-lookup"><span data-stu-id="f4c16-142">Response</span></span>

<span data-ttu-id="f4c16-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4c16-143">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
