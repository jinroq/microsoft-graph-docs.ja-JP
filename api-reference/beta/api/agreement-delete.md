---
title: 契約を削除します。
description: 契約オブジェクトを削除します。
ms.openlocfilehash: 919fc628e5f8ff9b6c016e085671f47ed6d56a5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069288"
---
# <a name="delete-agreement"></a><span data-ttu-id="271f3-103">契約を削除します。</span><span class="sxs-lookup"><span data-stu-id="271f3-103">Delete agreement</span></span>

> <span data-ttu-id="271f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="271f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="271f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="271f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="271f3-106">[契約](../resources/agreement.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="271f3-106">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="271f3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="271f3-107">Permissions</span></span>
<span data-ttu-id="271f3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="271f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="271f3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="271f3-110">Permission type</span></span>                        | <span data-ttu-id="271f3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="271f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="271f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="271f3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="271f3-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271f3-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="271f3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="271f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271f3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="271f3-115">Not supported.</span></span> |
|<span data-ttu-id="271f3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="271f3-116">Application</span></span>                            | <span data-ttu-id="271f3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="271f3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="271f3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="271f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="271f3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="271f3-119">Request headers</span></span>
| <span data-ttu-id="271f3-120">名前</span><span class="sxs-lookup"><span data-stu-id="271f3-120">Name</span></span>         | <span data-ttu-id="271f3-121">型</span><span class="sxs-lookup"><span data-stu-id="271f3-121">Type</span></span>        | <span data-ttu-id="271f3-122">説明</span><span class="sxs-lookup"><span data-stu-id="271f3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="271f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="271f3-123">Authorization</span></span> | <span data-ttu-id="271f3-124">string</span><span class="sxs-lookup"><span data-stu-id="271f3-124">string</span></span> | <span data-ttu-id="271f3-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="271f3-125">Bearer \{token\}.</span></span> <span data-ttu-id="271f3-126">必須。</span><span class="sxs-lookup"><span data-stu-id="271f3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="271f3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="271f3-127">Request body</span></span>
<span data-ttu-id="271f3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="271f3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="271f3-129">応答</span><span class="sxs-lookup"><span data-stu-id="271f3-129">Response</span></span>
<span data-ttu-id="271f3-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="271f3-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="271f3-132">例</span><span class="sxs-lookup"><span data-stu-id="271f3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="271f3-133">要求</span><span class="sxs-lookup"><span data-stu-id="271f3-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="271f3-134">応答</span><span class="sxs-lookup"><span data-stu-id="271f3-134">Response</span></span>
><span data-ttu-id="271f3-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="271f3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->