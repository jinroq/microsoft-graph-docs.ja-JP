---
title: AccessReview を削除します。
description: Azure AD のレビュー機能にアクセス、accessReview オブジェクトを削除します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 21bfebd8e4c266669e441191bade72be692df51c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971761"
---
# <a name="delete-accessreview"></a><span data-ttu-id="1543f-103">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="1543f-103">Delete accessReview</span></span>

> <span data-ttu-id="1543f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1543f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1543f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1543f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1543f-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1543f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1543f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1543f-107">Permissions</span></span>
<span data-ttu-id="1543f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1543f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1543f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1543f-110">Permission type</span></span>                        | <span data-ttu-id="1543f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1543f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1543f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1543f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1543f-113">AccessReview.ReadWrite.All と、デバッギングを削除する呼び出しの完全なシナリオを ProgramControl.ReadWrite.All する必要があり、</span><span class="sxs-lookup"><span data-stu-id="1543f-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="1543f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1543f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1543f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1543f-115">Not supported.</span></span> |
|<span data-ttu-id="1543f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1543f-116">Application</span></span>                            | <span data-ttu-id="1543f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1543f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1543f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1543f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="1543f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1543f-119">Request headers</span></span>
| <span data-ttu-id="1543f-120">名前</span><span class="sxs-lookup"><span data-stu-id="1543f-120">Name</span></span>         | <span data-ttu-id="1543f-121">種類</span><span class="sxs-lookup"><span data-stu-id="1543f-121">Type</span></span>        | <span data-ttu-id="1543f-122">説明</span><span class="sxs-lookup"><span data-stu-id="1543f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1543f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1543f-123">Authorization</span></span> | <span data-ttu-id="1543f-124">string</span><span class="sxs-lookup"><span data-stu-id="1543f-124">string</span></span> | <span data-ttu-id="1543f-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="1543f-125">Bearer \{token\}.</span></span> <span data-ttu-id="1543f-126">必須。</span><span class="sxs-lookup"><span data-stu-id="1543f-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1543f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1543f-127">Request body</span></span>
<span data-ttu-id="1543f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1543f-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1543f-129">応答</span><span class="sxs-lookup"><span data-stu-id="1543f-129">Response</span></span>
<span data-ttu-id="1543f-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1543f-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1543f-132">例</span><span class="sxs-lookup"><span data-stu-id="1543f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1543f-133">要求</span><span class="sxs-lookup"><span data-stu-id="1543f-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="1543f-134">応答</span><span class="sxs-lookup"><span data-stu-id="1543f-134">Response</span></span>
><span data-ttu-id="1543f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1543f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
