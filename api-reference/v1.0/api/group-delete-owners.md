---
title: 所有者の削除
description: この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: f07eb16e2e7f70c3f503a5f182c015c6862ce5e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986755"
---
# <a name="remove-owner"></a><span data-ttu-id="e2965-103">所有者の削除</span><span class="sxs-lookup"><span data-stu-id="e2965-103">Remove owner</span></span>
<span data-ttu-id="e2965-104">この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。</span><span class="sxs-lookup"><span data-stu-id="e2965-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2965-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2965-105">Permissions</span></span>
<span data-ttu-id="e2965-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2965-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2965-108">Permission type</span></span>      | <span data-ttu-id="e2965-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2965-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2965-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2965-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2965-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2965-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2965-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2965-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2965-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2965-113">Not supported.</span></span>    |
|<span data-ttu-id="e2965-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2965-114">Application</span></span> | <span data-ttu-id="e2965-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2965-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2965-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2965-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e2965-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2965-117">Request headers</span></span>
| <span data-ttu-id="e2965-118">名前</span><span class="sxs-lookup"><span data-stu-id="e2965-118">Name</span></span>       | <span data-ttu-id="e2965-119">種類</span><span class="sxs-lookup"><span data-stu-id="e2965-119">Type</span></span> | <span data-ttu-id="e2965-120">説明</span><span class="sxs-lookup"><span data-stu-id="e2965-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2965-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2965-121">Authorization</span></span>  | <span data-ttu-id="e2965-122">string</span><span class="sxs-lookup"><span data-stu-id="e2965-122">string</span></span>  | <span data-ttu-id="e2965-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2965-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2965-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2965-125">Request body</span></span>
<span data-ttu-id="e2965-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2965-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2965-127">応答</span><span class="sxs-lookup"><span data-stu-id="e2965-127">Response</span></span>
<span data-ttu-id="e2965-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e2965-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2965-130">例</span><span class="sxs-lookup"><span data-stu-id="e2965-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e2965-131">要求</span><span class="sxs-lookup"><span data-stu-id="e2965-131">Request</span></span>
<span data-ttu-id="e2965-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2965-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="e2965-133">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2965-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="e2965-134">応答</span><span class="sxs-lookup"><span data-stu-id="e2965-134">Response</span></span>
<span data-ttu-id="e2965-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2965-135">The following is an example of the response.</span></span>
><span data-ttu-id="e2965-136">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e2965-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2965-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e2965-137">All the properties will be returned from an actual call.</span></span>
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
