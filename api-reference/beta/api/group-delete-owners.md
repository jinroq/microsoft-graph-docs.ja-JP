---
title: 所有者の削除
description: この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。
localization_priority: Normal
ms.openlocfilehash: af45706e6f42f3442e28dd8a04fe6863f957a6fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843359"
---
# <a name="remove-owner"></a><span data-ttu-id="76445-103">所有者の削除</span><span class="sxs-lookup"><span data-stu-id="76445-103">Remove owner</span></span>

> <span data-ttu-id="76445-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76445-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76445-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76445-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76445-106">この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。</span><span class="sxs-lookup"><span data-stu-id="76445-106">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="76445-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76445-107">Permissions</span></span>
<span data-ttu-id="76445-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76445-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76445-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76445-110">Permission type</span></span>      | <span data-ttu-id="76445-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76445-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76445-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76445-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76445-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76445-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="76445-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76445-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76445-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76445-115">Not supported.</span></span>    |
|<span data-ttu-id="76445-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76445-116">Application</span></span> | <span data-ttu-id="76445-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76445-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76445-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76445-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="76445-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76445-119">Request headers</span></span>
| <span data-ttu-id="76445-120">名前</span><span class="sxs-lookup"><span data-stu-id="76445-120">Name</span></span>       | <span data-ttu-id="76445-121">種類</span><span class="sxs-lookup"><span data-stu-id="76445-121">Type</span></span> | <span data-ttu-id="76445-122">説明</span><span class="sxs-lookup"><span data-stu-id="76445-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76445-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76445-123">Authorization</span></span>  | <span data-ttu-id="76445-124">string</span><span class="sxs-lookup"><span data-stu-id="76445-124">string</span></span>  | <span data-ttu-id="76445-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76445-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76445-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="76445-127">Request body</span></span>
<span data-ttu-id="76445-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76445-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76445-129">応答</span><span class="sxs-lookup"><span data-stu-id="76445-129">Response</span></span>
<span data-ttu-id="76445-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="76445-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76445-132">例</span><span class="sxs-lookup"><span data-stu-id="76445-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="76445-133">要求</span><span class="sxs-lookup"><span data-stu-id="76445-133">Request</span></span>
<span data-ttu-id="76445-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76445-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="76445-135">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="76445-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="76445-136">応答</span><span class="sxs-lookup"><span data-stu-id="76445-136">Response</span></span>
<span data-ttu-id="76445-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76445-137">The following is an example of the response.</span></span>
><span data-ttu-id="76445-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="76445-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76445-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="76445-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
