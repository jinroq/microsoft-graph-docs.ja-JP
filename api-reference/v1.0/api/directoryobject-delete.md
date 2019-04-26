---
title: directoryObject を削除する
description: directoryObject を削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fccafa016dad9892c701e852bc592564661c9cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555102"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="e92be-103">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="e92be-103">Delete directoryObject</span></span>

<span data-ttu-id="e92be-104">directoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="e92be-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="e92be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e92be-105">Permissions</span></span>
<span data-ttu-id="e92be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e92be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e92be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e92be-108">Permission type</span></span>      | <span data-ttu-id="e92be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e92be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e92be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e92be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e92be-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e92be-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e92be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e92be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e92be-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e92be-113">Not supported.</span></span>    |
|<span data-ttu-id="e92be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e92be-114">Application</span></span> | <span data-ttu-id="e92be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e92be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e92be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e92be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e92be-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e92be-117">Request headers</span></span>
| <span data-ttu-id="e92be-118">名前</span><span class="sxs-lookup"><span data-stu-id="e92be-118">Name</span></span>       | <span data-ttu-id="e92be-119">型</span><span class="sxs-lookup"><span data-stu-id="e92be-119">Type</span></span> | <span data-ttu-id="e92be-120">説明</span><span class="sxs-lookup"><span data-stu-id="e92be-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e92be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e92be-121">Authorization</span></span>  | <span data-ttu-id="e92be-122">string</span><span class="sxs-lookup"><span data-stu-id="e92be-122">string</span></span>  | <span data-ttu-id="e92be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e92be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e92be-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e92be-125">Request body</span></span>
<span data-ttu-id="e92be-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e92be-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e92be-127">応答</span><span class="sxs-lookup"><span data-stu-id="e92be-127">Response</span></span>

<span data-ttu-id="e92be-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e92be-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e92be-130">例</span><span class="sxs-lookup"><span data-stu-id="e92be-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e92be-131">要求</span><span class="sxs-lookup"><span data-stu-id="e92be-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="e92be-132">応答</span><span class="sxs-lookup"><span data-stu-id="e92be-132">Response</span></span>

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
