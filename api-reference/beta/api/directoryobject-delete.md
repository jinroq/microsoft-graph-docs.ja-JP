---
title: directoryObject を削除する
description: DirectoryObject を削除します。
author: lleonard-msft
ms.openlocfilehash: f53ffc488529c2af4b566ada52f213d1fc132c60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361412"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="aac41-103">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="aac41-103">Delete directoryObject</span></span>

> <span data-ttu-id="aac41-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aac41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aac41-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aac41-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aac41-106">DirectoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="aac41-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="aac41-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aac41-107">Permissions</span></span>
<span data-ttu-id="aac41-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aac41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aac41-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aac41-110">Permission type</span></span>      | <span data-ttu-id="aac41-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aac41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac41-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aac41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aac41-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aac41-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aac41-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aac41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac41-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aac41-115">Not supported.</span></span>    |
|<span data-ttu-id="aac41-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aac41-116">Application</span></span> | <span data-ttu-id="aac41-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aac41-117">Not supported.</span></span> |

<span data-ttu-id="aac41-118">**注:** ユーザー、グループ、および連絡先は、ディレクトリ オブジェクトの種類です。</span><span class="sxs-lookup"><span data-stu-id="aac41-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="aac41-119">その結果、ユーザーを削除する場合は、次のアクセス許可ことができ、使用する必要があります: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac41-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="aac41-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aac41-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="aac41-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aac41-121">Request headers</span></span>
| <span data-ttu-id="aac41-122">名前</span><span class="sxs-lookup"><span data-stu-id="aac41-122">Name</span></span>       | <span data-ttu-id="aac41-123">種類</span><span class="sxs-lookup"><span data-stu-id="aac41-123">Type</span></span> | <span data-ttu-id="aac41-124">説明</span><span class="sxs-lookup"><span data-stu-id="aac41-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aac41-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac41-125">Authorization</span></span>  | <span data-ttu-id="aac41-126">string</span><span class="sxs-lookup"><span data-stu-id="aac41-126">string</span></span>  | <span data-ttu-id="aac41-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aac41-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aac41-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="aac41-129">Request body</span></span>
<span data-ttu-id="aac41-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aac41-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac41-131">応答</span><span class="sxs-lookup"><span data-stu-id="aac41-131">Response</span></span>

<span data-ttu-id="aac41-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="aac41-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac41-134">例</span><span class="sxs-lookup"><span data-stu-id="aac41-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aac41-135">要求</span><span class="sxs-lookup"><span data-stu-id="aac41-135">Request</span></span>
<span data-ttu-id="aac41-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aac41-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="aac41-137">応答</span><span class="sxs-lookup"><span data-stu-id="aac41-137">Response</span></span>
<span data-ttu-id="aac41-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="aac41-138">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->