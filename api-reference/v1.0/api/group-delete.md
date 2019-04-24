---
title: グループの削除-Microsoft Graph API
description: Microsoft Graph API (REST) のグループリソース (エンティティ) の delete メソッドについて説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1e252ddfddfcd82bcd3f790c75b34f016f54c9fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522609"
---
# <a name="delete-group"></a><span data-ttu-id="63d31-103">グループの削除</span><span class="sxs-lookup"><span data-stu-id="63d31-103">Delete group</span></span>

<span data-ttu-id="63d31-104">グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="63d31-104">Delete group.</span></span>  

<span data-ttu-id="63d31-105">削除すると、Office 365 グループが一時コンテナーに移動され、30日以内に復元できるようになります。</span><span class="sxs-lookup"><span data-stu-id="63d31-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="63d31-106">それ以降、これらのユーザーは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="63d31-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="63d31-107">詳細については、「[deletedItems](../resources/directory.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63d31-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="63d31-108">これは、Office 365 グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="63d31-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="63d31-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="63d31-109">Permissions</span></span>

<span data-ttu-id="63d31-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63d31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63d31-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63d31-112">Permission type</span></span>      | <span data-ttu-id="63d31-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="63d31-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63d31-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63d31-114">Delegated (work or school account)</span></span> | <span data-ttu-id="63d31-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d31-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63d31-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63d31-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63d31-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63d31-117">Not supported.</span></span>    |
|<span data-ttu-id="63d31-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63d31-118">Application</span></span> | <span data-ttu-id="63d31-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d31-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63d31-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63d31-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63d31-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63d31-121">Request headers</span></span>

| <span data-ttu-id="63d31-122">名前</span><span class="sxs-lookup"><span data-stu-id="63d31-122">Name</span></span>       | <span data-ttu-id="63d31-123">型</span><span class="sxs-lookup"><span data-stu-id="63d31-123">Type</span></span> | <span data-ttu-id="63d31-124">説明</span><span class="sxs-lookup"><span data-stu-id="63d31-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63d31-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63d31-125">Authorization</span></span>  | <span data-ttu-id="63d31-126">string</span><span class="sxs-lookup"><span data-stu-id="63d31-126">string</span></span>  | <span data-ttu-id="63d31-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="63d31-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63d31-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="63d31-129">Request body</span></span>

<span data-ttu-id="63d31-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="63d31-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63d31-131">応答</span><span class="sxs-lookup"><span data-stu-id="63d31-131">Response</span></span>

<span data-ttu-id="63d31-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="63d31-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63d31-134">例</span><span class="sxs-lookup"><span data-stu-id="63d31-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="63d31-135">要求</span><span class="sxs-lookup"><span data-stu-id="63d31-135">Request</span></span>

<span data-ttu-id="63d31-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="63d31-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

### <a name="response"></a><span data-ttu-id="63d31-137">応答</span><span class="sxs-lookup"><span data-stu-id="63d31-137">Response</span></span>

<span data-ttu-id="63d31-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="63d31-138">The following is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
