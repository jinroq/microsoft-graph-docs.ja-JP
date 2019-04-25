---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c870e1d6d9e294aadef50fb08d9e173e5aa62f5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577876"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="48f2f-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="48f2f-103">Remove directory role member</span></span>

<span data-ttu-id="48f2f-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="48f2f-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f2f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48f2f-105">Permissions</span></span>

<span data-ttu-id="48f2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48f2f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48f2f-108">Permission type</span></span>      | <span data-ttu-id="48f2f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48f2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48f2f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48f2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48f2f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48f2f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48f2f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48f2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f2f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48f2f-113">Not supported.</span></span>    |
|<span data-ttu-id="48f2f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48f2f-114">Application</span></span> | <span data-ttu-id="48f2f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48f2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f2f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48f2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="48f2f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48f2f-117">Request headers</span></span>

| <span data-ttu-id="48f2f-118">名前</span><span class="sxs-lookup"><span data-stu-id="48f2f-118">Name</span></span>       | <span data-ttu-id="48f2f-119">型</span><span class="sxs-lookup"><span data-stu-id="48f2f-119">Type</span></span> | <span data-ttu-id="48f2f-120">説明</span><span class="sxs-lookup"><span data-stu-id="48f2f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48f2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="48f2f-121">Authorization</span></span>  | <span data-ttu-id="48f2f-122">string</span><span class="sxs-lookup"><span data-stu-id="48f2f-122">string</span></span>  | <span data-ttu-id="48f2f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48f2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48f2f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="48f2f-125">Request body</span></span>

<span data-ttu-id="48f2f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="48f2f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48f2f-127">応答</span><span class="sxs-lookup"><span data-stu-id="48f2f-127">Response</span></span>

<span data-ttu-id="48f2f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="48f2f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48f2f-130">例</span><span class="sxs-lookup"><span data-stu-id="48f2f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48f2f-131">要求</span><span class="sxs-lookup"><span data-stu-id="48f2f-131">Request</span></span>

<span data-ttu-id="48f2f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48f2f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="48f2f-133">応答</span><span class="sxs-lookup"><span data-stu-id="48f2f-133">Response</span></span>

<span data-ttu-id="48f2f-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="48f2f-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
