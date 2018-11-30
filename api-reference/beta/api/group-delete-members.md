---
title: メンバーを削除する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。
ms.openlocfilehash: be011101208d33293906ab7c8e79e242ca4c8f9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067637"
---
# <a name="remove-member"></a><span data-ttu-id="cddca-104">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="cddca-104">Remove member</span></span>

> <span data-ttu-id="cddca-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cddca-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cddca-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cddca-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cddca-p103">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。</span><span class="sxs-lookup"><span data-stu-id="cddca-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="cddca-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cddca-109">Permissions</span></span>
<span data-ttu-id="cddca-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cddca-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cddca-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cddca-112">Permission type</span></span>      | <span data-ttu-id="cddca-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cddca-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cddca-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cddca-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cddca-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cddca-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cddca-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cddca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cddca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cddca-117">Not supported.</span></span>    |
|<span data-ttu-id="cddca-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cddca-118">Application</span></span> | <span data-ttu-id="cddca-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cddca-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cddca-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cddca-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cddca-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cddca-121">Request headers</span></span>
| <span data-ttu-id="cddca-122">名前</span><span class="sxs-lookup"><span data-stu-id="cddca-122">Name</span></span>       | <span data-ttu-id="cddca-123">型</span><span class="sxs-lookup"><span data-stu-id="cddca-123">Type</span></span> | <span data-ttu-id="cddca-124">説明</span><span class="sxs-lookup"><span data-stu-id="cddca-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cddca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cddca-125">Authorization</span></span>  | <span data-ttu-id="cddca-126">string</span><span class="sxs-lookup"><span data-stu-id="cddca-126">string</span></span>  | <span data-ttu-id="cddca-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cddca-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cddca-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cddca-129">Request body</span></span>
<span data-ttu-id="cddca-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cddca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cddca-131">応答</span><span class="sxs-lookup"><span data-stu-id="cddca-131">Response</span></span>
<span data-ttu-id="cddca-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cddca-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cddca-134">例</span><span class="sxs-lookup"><span data-stu-id="cddca-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cddca-135">要求</span><span class="sxs-lookup"><span data-stu-id="cddca-135">Request</span></span>
<span data-ttu-id="cddca-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cddca-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="cddca-137">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="cddca-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="cddca-138">応答</span><span class="sxs-lookup"><span data-stu-id="cddca-138">Response</span></span>
<span data-ttu-id="cddca-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cddca-139">The following is an example of the response.</span></span>
><span data-ttu-id="cddca-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cddca-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cddca-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cddca-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
