---
title: trustframeworkpolicy の削除
description: この操作により、Azure AD B2C テナントから既存の trustframeworkpolicy オブジェクトが削除されます。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2583cbf5fd8feee12b18482c515490d2de8ce8be
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989402"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="0c4fb-103">trustframeworkpolicy の削除</span><span class="sxs-lookup"><span data-stu-id="0c4fb-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="0c4fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4fb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c4fb-106">既存の[trustframeworkpolicy](../resources/trustframeworkpolicy.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c4fb-107">Permissions</span></span>

<span data-ttu-id="0c4fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="0c4fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c4fb-110">Permission type</span></span>      | <span data-ttu-id="0c4fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c4fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c4fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4fb-113">ポリシー。 trustframework</span><span class="sxs-lookup"><span data-stu-id="0c4fb-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="0c4fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c4fb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0c4fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-115">Not supported.</span></span>|
|<span data-ttu-id="0c4fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c4fb-116">Application</span></span>|<span data-ttu-id="0c4fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-117">Not supported.</span></span>|

<span data-ttu-id="0c4fb-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c4fb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c4fb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c4fb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c4fb-120">Request headers</span></span>

|<span data-ttu-id="0c4fb-121">名前</span><span class="sxs-lookup"><span data-stu-id="0c4fb-121">Name</span></span>|<span data-ttu-id="0c4fb-122">説明</span><span class="sxs-lookup"><span data-stu-id="0c4fb-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0c4fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c4fb-123">Authorization</span></span>|<span data-ttu-id="0c4fb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4fb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c4fb-126">Request body</span></span>

<span data-ttu-id="0c4fb-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4fb-128">応答</span><span class="sxs-lookup"><span data-stu-id="0c4fb-128">Response</span></span>

<span data-ttu-id="0c4fb-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c4fb-130">例</span><span class="sxs-lookup"><span data-stu-id="0c4fb-130">Example</span></span>

<span data-ttu-id="0c4fb-131">次の例では、 **trustframeworkpolicy**を削除します。</span><span class="sxs-lookup"><span data-stu-id="0c4fb-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="0c4fb-132">要求</span><span class="sxs-lookup"><span data-stu-id="0c4fb-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a><span data-ttu-id="0c4fb-133">応答</span><span class="sxs-lookup"><span data-stu-id="0c4fb-133">Response</span></span>

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
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
