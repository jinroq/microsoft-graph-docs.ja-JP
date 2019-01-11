---
title: メンバーを削除する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。
localization_priority: Normal
ms.openlocfilehash: 917e662158785111847d5d74821bfedbb61205dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864478"
---
# <a name="remove-member"></a><span data-ttu-id="16c82-104">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="16c82-104">Remove member</span></span>

> <span data-ttu-id="16c82-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16c82-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16c82-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c82-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16c82-p103">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。</span><span class="sxs-lookup"><span data-stu-id="16c82-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="16c82-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16c82-109">Permissions</span></span>
<span data-ttu-id="16c82-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16c82-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c82-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16c82-112">Permission type</span></span>      | <span data-ttu-id="16c82-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16c82-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16c82-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16c82-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16c82-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16c82-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16c82-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16c82-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16c82-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c82-117">Not supported.</span></span>    |
|<span data-ttu-id="16c82-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16c82-118">Application</span></span> | <span data-ttu-id="16c82-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16c82-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16c82-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16c82-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="16c82-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16c82-121">Request headers</span></span>
| <span data-ttu-id="16c82-122">名前</span><span class="sxs-lookup"><span data-stu-id="16c82-122">Name</span></span>       | <span data-ttu-id="16c82-123">種類</span><span class="sxs-lookup"><span data-stu-id="16c82-123">Type</span></span> | <span data-ttu-id="16c82-124">説明</span><span class="sxs-lookup"><span data-stu-id="16c82-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16c82-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16c82-125">Authorization</span></span>  | <span data-ttu-id="16c82-126">string</span><span class="sxs-lookup"><span data-stu-id="16c82-126">string</span></span>  | <span data-ttu-id="16c82-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16c82-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16c82-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="16c82-129">Request body</span></span>
<span data-ttu-id="16c82-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16c82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16c82-131">応答</span><span class="sxs-lookup"><span data-stu-id="16c82-131">Response</span></span>
<span data-ttu-id="16c82-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="16c82-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16c82-134">例</span><span class="sxs-lookup"><span data-stu-id="16c82-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16c82-135">要求</span><span class="sxs-lookup"><span data-stu-id="16c82-135">Request</span></span>
<span data-ttu-id="16c82-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16c82-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="16c82-137">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="16c82-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="16c82-138">応答</span><span class="sxs-lookup"><span data-stu-id="16c82-138">Response</span></span>
<span data-ttu-id="16c82-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16c82-139">The following is an example of the response.</span></span>
><span data-ttu-id="16c82-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="16c82-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16c82-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16c82-141">All the properties will be returned from an actual call.</span></span>
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
