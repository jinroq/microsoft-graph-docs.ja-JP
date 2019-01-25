---
title: SendReminder accessReview
description: 'Azure AD のレビュー機能をアクセスは、現在アクティブな accessReview のレビュー担当者に通知を送信します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518549"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="4bea3-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="4bea3-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bea3-105">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、現在アクティブな[accessReview](../resources/accessreview.md)のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="4bea3-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="4bea3-106">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="4bea3-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4bea3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4bea3-107">Permissions</span></span>
<span data-ttu-id="4bea3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bea3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bea3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bea3-110">Permission type</span></span>                        | <span data-ttu-id="4bea3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bea3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bea3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bea3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bea3-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bea3-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4bea3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bea3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bea3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bea3-115">Not supported.</span></span> |
|<span data-ttu-id="4bea3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bea3-116">Application</span></span>                            | <span data-ttu-id="4bea3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bea3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bea3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bea3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="4bea3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bea3-119">Request headers</span></span>
| <span data-ttu-id="4bea3-120">名前</span><span class="sxs-lookup"><span data-stu-id="4bea3-120">Name</span></span>         | <span data-ttu-id="4bea3-121">型</span><span class="sxs-lookup"><span data-stu-id="4bea3-121">Type</span></span>        | <span data-ttu-id="4bea3-122">説明</span><span class="sxs-lookup"><span data-stu-id="4bea3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4bea3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bea3-123">Authorization</span></span> | <span data-ttu-id="4bea3-124">string</span><span class="sxs-lookup"><span data-stu-id="4bea3-124">string</span></span> | <span data-ttu-id="4bea3-125">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="4bea3-125">Bearer \{token\}.</span></span> <span data-ttu-id="4bea3-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="4bea3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bea3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bea3-127">Request body</span></span>
<span data-ttu-id="4bea3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4bea3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4bea3-129">応答</span><span class="sxs-lookup"><span data-stu-id="4bea3-129">Response</span></span>
<span data-ttu-id="4bea3-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4bea3-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bea3-132">例</span><span class="sxs-lookup"><span data-stu-id="4bea3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bea3-133">要求</span><span class="sxs-lookup"><span data-stu-id="4bea3-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="4bea3-134">応答</span><span class="sxs-lookup"><span data-stu-id="4bea3-134">Response</span></span>
><span data-ttu-id="4bea3-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4bea3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
