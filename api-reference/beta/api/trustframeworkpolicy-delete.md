---
title: TrustFrameworkPolicy の削除
description: この操作により、Azure AD B2C テナントから既存の trustFrameworkPolicy オブジェクトが削除されます。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f13c70edfe5cd38407c5b1bfe04998a16d0c376
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450871"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="acf0c-103">TrustFrameworkPolicy の削除</span><span class="sxs-lookup"><span data-stu-id="acf0c-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="acf0c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="acf0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acf0c-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acf0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acf0c-106">既存の[Trustframeworkpolicy](../resources/trustframeworkpolicy.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="acf0c-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="acf0c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="acf0c-107">Permissions</span></span>

<span data-ttu-id="acf0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acf0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="acf0c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acf0c-110">Permission type</span></span>      | <span data-ttu-id="acf0c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="acf0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acf0c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acf0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acf0c-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="acf0c-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="acf0c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acf0c-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="acf0c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acf0c-115">Not supported.</span></span>|
|<span data-ttu-id="acf0c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acf0c-116">Application</span></span>|<span data-ttu-id="acf0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acf0c-117">Not supported.</span></span>|

<span data-ttu-id="acf0c-118">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="acf0c-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="acf0c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acf0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="acf0c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acf0c-120">Request headers</span></span>

|<span data-ttu-id="acf0c-121">名前</span><span class="sxs-lookup"><span data-stu-id="acf0c-121">Name</span></span>|<span data-ttu-id="acf0c-122">説明</span><span class="sxs-lookup"><span data-stu-id="acf0c-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="acf0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acf0c-123">Authorization</span></span>|<span data-ttu-id="acf0c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="acf0c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="acf0c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="acf0c-126">Request body</span></span>

<span data-ttu-id="acf0c-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="acf0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acf0c-128">応答</span><span class="sxs-lookup"><span data-stu-id="acf0c-128">Response</span></span>

<span data-ttu-id="acf0c-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="acf0c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="acf0c-130">例</span><span class="sxs-lookup"><span data-stu-id="acf0c-130">Example</span></span>

<span data-ttu-id="acf0c-131">次の例では、 **Trustframeworkpolicy**を削除します。</span><span class="sxs-lookup"><span data-stu-id="acf0c-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="acf0c-132">要求</span><span class="sxs-lookup"><span data-stu-id="acf0c-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="acf0c-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="acf0c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="acf0c-134">C#</span><span class="sxs-lookup"><span data-stu-id="acf0c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="acf0c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="acf0c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="acf0c-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="acf0c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="acf0c-137">応答</span><span class="sxs-lookup"><span data-stu-id="acf0c-137">Response</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
