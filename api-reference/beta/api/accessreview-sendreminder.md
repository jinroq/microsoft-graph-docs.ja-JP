---
title: SendReminder accessReview
description: 'Azure AD のレビュー機能をアクセスは、現在アクティブな accessReview のレビュー担当者に通知を送信します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。 '
ms.openlocfilehash: fd8c204db207ae9f58c4dd5e6337e65efe160824
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069287"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="5ccb7-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="5ccb7-104">SendReminder accessReview</span></span>

> <span data-ttu-id="5ccb7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ccb7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ccb7-107">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、現在アクティブな[accessReview](../resources/accessreview.md)のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="5ccb7-108">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5ccb7-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ccb7-109">Permissions</span></span>
<span data-ttu-id="5ccb7-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ccb7-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ccb7-112">Permission type</span></span>                        | <span data-ttu-id="5ccb7-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ccb7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ccb7-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ccb7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ccb7-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ccb7-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="5ccb7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ccb7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ccb7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-117">Not supported.</span></span> |
|<span data-ttu-id="5ccb7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ccb7-118">Application</span></span>                            | <span data-ttu-id="5ccb7-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ccb7-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ccb7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="5ccb7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ccb7-121">Request headers</span></span>
| <span data-ttu-id="5ccb7-122">名前</span><span class="sxs-lookup"><span data-stu-id="5ccb7-122">Name</span></span>         | <span data-ttu-id="5ccb7-123">型</span><span class="sxs-lookup"><span data-stu-id="5ccb7-123">Type</span></span>        | <span data-ttu-id="5ccb7-124">説明</span><span class="sxs-lookup"><span data-stu-id="5ccb7-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5ccb7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ccb7-125">Authorization</span></span> | <span data-ttu-id="5ccb7-126">string</span><span class="sxs-lookup"><span data-stu-id="5ccb7-126">string</span></span> | <span data-ttu-id="5ccb7-127">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-127">Bearer \{token\}.</span></span> <span data-ttu-id="5ccb7-128">必須。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ccb7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ccb7-129">Request body</span></span>
<span data-ttu-id="5ccb7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5ccb7-131">応答</span><span class="sxs-lookup"><span data-stu-id="5ccb7-131">Response</span></span>
<span data-ttu-id="5ccb7-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ccb7-134">例</span><span class="sxs-lookup"><span data-stu-id="5ccb7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ccb7-135">要求</span><span class="sxs-lookup"><span data-stu-id="5ccb7-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="5ccb7-136">応答</span><span class="sxs-lookup"><span data-stu-id="5ccb7-136">Response</span></span>
><span data-ttu-id="5ccb7-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ccb7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->