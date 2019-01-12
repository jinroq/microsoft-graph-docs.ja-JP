---
title: educationClass を削除する
description: クラスを削除します。 クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9b25e95dfa109ef48d67374ba7569a32af22ba50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935067"
---
# <a name="delete-educationclass"></a><span data-ttu-id="c4b19-104">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="c4b19-104">Delete educationClass</span></span>

> <span data-ttu-id="c4b19-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4b19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4b19-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4b19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4b19-107">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="c4b19-107">Delete a class.</span></span> <span data-ttu-id="c4b19-108">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="c4b19-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b19-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4b19-109">Permissions</span></span>
<span data-ttu-id="c4b19-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4b19-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b19-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4b19-112">Permission type</span></span>      | <span data-ttu-id="c4b19-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4b19-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4b19-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4b19-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c4b19-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4b19-115">Not supported.</span></span>  |
|<span data-ttu-id="c4b19-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4b19-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c4b19-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4b19-117">Not supported.</span></span>  |
|<span data-ttu-id="c4b19-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4b19-118">Application</span></span> | <span data-ttu-id="c4b19-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b19-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c4b19-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4b19-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c4b19-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4b19-121">Request headers</span></span>
| <span data-ttu-id="c4b19-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4b19-122">Header</span></span>       | <span data-ttu-id="c4b19-123">値</span><span class="sxs-lookup"><span data-stu-id="c4b19-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4b19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4b19-124">Authorization</span></span>  | <span data-ttu-id="c4b19-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4b19-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4b19-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4b19-127">Request body</span></span>
<span data-ttu-id="c4b19-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4b19-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c4b19-129">応答</span><span class="sxs-lookup"><span data-stu-id="c4b19-129">Response</span></span>
<span data-ttu-id="c4b19-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c4b19-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b19-132">例</span><span class="sxs-lookup"><span data-stu-id="c4b19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4b19-133">要求</span><span class="sxs-lookup"><span data-stu-id="c4b19-133">Request</span></span>
<span data-ttu-id="c4b19-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4b19-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="c4b19-135">応答</span><span class="sxs-lookup"><span data-stu-id="c4b19-135">Response</span></span>
<span data-ttu-id="c4b19-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4b19-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
