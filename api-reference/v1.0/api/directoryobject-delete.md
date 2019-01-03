---
title: directoryObject を削除する
description: directoryObject を削除します。
author: lleonard-msft
ms.openlocfilehash: dec525e72b523e7bbe95996d4c863c68e01baa15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313203"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="9c82e-103">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="9c82e-103">Delete directoryObject</span></span>

<span data-ttu-id="9c82e-104">directoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="9c82e-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c82e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9c82e-105">Permissions</span></span>
<span data-ttu-id="9c82e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c82e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c82e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c82e-108">Permission type</span></span>      | <span data-ttu-id="9c82e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c82e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c82e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c82e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c82e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c82e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c82e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c82e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c82e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c82e-113">Not supported.</span></span>    |
|<span data-ttu-id="9c82e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c82e-114">Application</span></span> | <span data-ttu-id="9c82e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c82e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c82e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c82e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9c82e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c82e-117">Request headers</span></span>
| <span data-ttu-id="9c82e-118">名前</span><span class="sxs-lookup"><span data-stu-id="9c82e-118">Name</span></span>       | <span data-ttu-id="9c82e-119">種類</span><span class="sxs-lookup"><span data-stu-id="9c82e-119">Type</span></span> | <span data-ttu-id="9c82e-120">説明</span><span class="sxs-lookup"><span data-stu-id="9c82e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c82e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c82e-121">Authorization</span></span>  | <span data-ttu-id="9c82e-122">string</span><span class="sxs-lookup"><span data-stu-id="9c82e-122">string</span></span>  | <span data-ttu-id="9c82e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9c82e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c82e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c82e-125">Request body</span></span>
<span data-ttu-id="9c82e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9c82e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c82e-127">応答</span><span class="sxs-lookup"><span data-stu-id="9c82e-127">Response</span></span>

<span data-ttu-id="9c82e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9c82e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c82e-130">例</span><span class="sxs-lookup"><span data-stu-id="9c82e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c82e-131">要求</span><span class="sxs-lookup"><span data-stu-id="9c82e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="9c82e-132">応答</span><span class="sxs-lookup"><span data-stu-id="9c82e-132">Response</span></span>

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