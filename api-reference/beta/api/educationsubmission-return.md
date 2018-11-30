---
title: 'educationSubmission: 戻る'
description: " フィードバックを提供するか、グレーディングを行うことを示します。 このアクションは、先生によってのみ実行できます。"
ms.openlocfilehash: de81f5429119556753462781f701fb7c936826b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066373"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="0125f-104">educationSubmission: 戻る</span><span class="sxs-lookup"><span data-stu-id="0125f-104">educationSubmission: return</span></span>

> <span data-ttu-id="0125f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0125f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0125f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0125f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0125f-107">この操作によって、評価とフィードバックを受講者に利用可能なこの送信に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="0125f-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="0125f-108">これは「取得」から「送信」の提出書類のステータスが変更され、フィードバックを提供するか、グレーディングを行うことを示します。</span><span class="sxs-lookup"><span data-stu-id="0125f-108">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="0125f-109">このアクションは、先生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="0125f-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="0125f-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0125f-110">Permissions</span></span>
<span data-ttu-id="0125f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0125f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0125f-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0125f-113">Permission type</span></span>      | <span data-ttu-id="0125f-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0125f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0125f-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0125f-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="0125f-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0125f-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0125f-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0125f-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0125f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0125f-118">Not supported.</span></span>  |
|<span data-ttu-id="0125f-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0125f-119">Application</span></span> | <span data-ttu-id="0125f-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0125f-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0125f-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0125f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="0125f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0125f-122">Request headers</span></span>
| <span data-ttu-id="0125f-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0125f-123">Header</span></span>       | <span data-ttu-id="0125f-124">値</span><span class="sxs-lookup"><span data-stu-id="0125f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0125f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0125f-125">Authorization</span></span>  | <span data-ttu-id="0125f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0125f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0125f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0125f-128">Request body</span></span>
<span data-ttu-id="0125f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0125f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0125f-130">応答</span><span class="sxs-lookup"><span data-stu-id="0125f-130">Response</span></span>
<span data-ttu-id="0125f-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0125f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0125f-133">例</span><span class="sxs-lookup"><span data-stu-id="0125f-133">Example</span></span>
<span data-ttu-id="0125f-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0125f-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0125f-135">要求</span><span class="sxs-lookup"><span data-stu-id="0125f-135">Request</span></span>
<span data-ttu-id="0125f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0125f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="0125f-137">応答</span><span class="sxs-lookup"><span data-stu-id="0125f-137">Response</span></span>
<span data-ttu-id="0125f-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0125f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->