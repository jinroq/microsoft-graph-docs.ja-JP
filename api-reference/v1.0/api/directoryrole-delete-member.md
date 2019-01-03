---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: lleonard-msft
ms.openlocfilehash: a0c2976fdab3e548e9bf27cc19b7049926562ea7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350534"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="e35c2-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="e35c2-103">Remove directory role member</span></span>

<span data-ttu-id="e35c2-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="e35c2-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="e35c2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e35c2-105">Permissions</span></span>

<span data-ttu-id="e35c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e35c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e35c2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e35c2-108">Permission type</span></span>      | <span data-ttu-id="e35c2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e35c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e35c2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e35c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e35c2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e35c2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e35c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e35c2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e35c2-113">Not supported.</span></span>    |
|<span data-ttu-id="e35c2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e35c2-114">Application</span></span> | <span data-ttu-id="e35c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e35c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e35c2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e35c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e35c2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e35c2-117">Request headers</span></span>

| <span data-ttu-id="e35c2-118">名前</span><span class="sxs-lookup"><span data-stu-id="e35c2-118">Name</span></span>       | <span data-ttu-id="e35c2-119">種類</span><span class="sxs-lookup"><span data-stu-id="e35c2-119">Type</span></span> | <span data-ttu-id="e35c2-120">説明</span><span class="sxs-lookup"><span data-stu-id="e35c2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e35c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e35c2-121">Authorization</span></span>  | <span data-ttu-id="e35c2-122">string</span><span class="sxs-lookup"><span data-stu-id="e35c2-122">string</span></span>  | <span data-ttu-id="e35c2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e35c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e35c2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e35c2-125">Request body</span></span>

<span data-ttu-id="e35c2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e35c2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e35c2-127">応答</span><span class="sxs-lookup"><span data-stu-id="e35c2-127">Response</span></span>

<span data-ttu-id="e35c2-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e35c2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e35c2-130">例</span><span class="sxs-lookup"><span data-stu-id="e35c2-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e35c2-131">要求</span><span class="sxs-lookup"><span data-stu-id="e35c2-131">Request</span></span>

<span data-ttu-id="e35c2-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e35c2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="e35c2-133">応答</span><span class="sxs-lookup"><span data-stu-id="e35c2-133">Response</span></span>

<span data-ttu-id="e35c2-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e35c2-134">Here is an example of the response.</span></span> 
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