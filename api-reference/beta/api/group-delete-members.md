---
title: メンバーを削除する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0b985a5bc7c70e55a4e5ecfcc395595b7041fa30
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329651"
---
# <a name="remove-member"></a><span data-ttu-id="7f598-104">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="7f598-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f598-p102">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。</span><span class="sxs-lookup"><span data-stu-id="7f598-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f598-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f598-107">Permissions</span></span>
<span data-ttu-id="7f598-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f598-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f598-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f598-110">Permission type</span></span>      | <span data-ttu-id="7f598-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f598-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f598-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f598-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f598-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f598-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f598-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f598-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f598-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f598-115">Not supported.</span></span>    |
|<span data-ttu-id="7f598-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f598-116">Application</span></span> | <span data-ttu-id="7f598-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f598-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f598-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f598-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7f598-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f598-119">Request headers</span></span>
| <span data-ttu-id="7f598-120">名前</span><span class="sxs-lookup"><span data-stu-id="7f598-120">Name</span></span>       | <span data-ttu-id="7f598-121">型</span><span class="sxs-lookup"><span data-stu-id="7f598-121">Type</span></span> | <span data-ttu-id="7f598-122">説明</span><span class="sxs-lookup"><span data-stu-id="7f598-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f598-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f598-123">Authorization</span></span>  | <span data-ttu-id="7f598-124">string</span><span class="sxs-lookup"><span data-stu-id="7f598-124">string</span></span>  | <span data-ttu-id="7f598-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f598-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f598-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f598-127">Request body</span></span>
<span data-ttu-id="7f598-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f598-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f598-129">応答</span><span class="sxs-lookup"><span data-stu-id="7f598-129">Response</span></span>
<span data-ttu-id="7f598-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7f598-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f598-132">例</span><span class="sxs-lookup"><span data-stu-id="7f598-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f598-133">要求</span><span class="sxs-lookup"><span data-stu-id="7f598-133">Request</span></span>
<span data-ttu-id="7f598-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f598-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="7f598-135">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f598-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="7f598-136">応答</span><span class="sxs-lookup"><span data-stu-id="7f598-136">Response</span></span>
<span data-ttu-id="7f598-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f598-137">The following is an example of the response.</span></span>
><span data-ttu-id="7f598-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7f598-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f598-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7f598-139">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
