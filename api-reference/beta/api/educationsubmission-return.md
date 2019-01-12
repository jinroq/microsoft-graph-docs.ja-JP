---
title: 'educationSubmission: 戻る'
description: この操作によって、評価とフィードバックを受講者に利用可能なこの送信に関連付けられています。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39e57044571b43df0515755035e23a38980376fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930650"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="47a8d-103">educationSubmission: 戻る</span><span class="sxs-lookup"><span data-stu-id="47a8d-103">educationSubmission: return</span></span>

> <span data-ttu-id="47a8d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47a8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a8d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47a8d-106">この操作によって、評価とフィードバックを受講者に利用可能なこの送信に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="47a8d-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="47a8d-107">これは「取得」から「送信」の提出書類のステータスが変更され、フィードバックを提供するか、グレーディングを行うことを示します。</span><span class="sxs-lookup"><span data-stu-id="47a8d-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="47a8d-108">このアクションは、先生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="47a8d-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="47a8d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="47a8d-109">Permissions</span></span>
<span data-ttu-id="47a8d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47a8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a8d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47a8d-112">Permission type</span></span>      | <span data-ttu-id="47a8d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="47a8d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a8d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47a8d-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="47a8d-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47a8d-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="47a8d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47a8d-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47a8d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a8d-117">Not supported.</span></span>  |
|<span data-ttu-id="47a8d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47a8d-118">Application</span></span> | <span data-ttu-id="47a8d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47a8d-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47a8d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47a8d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="47a8d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47a8d-121">Request headers</span></span>
| <span data-ttu-id="47a8d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47a8d-122">Header</span></span>       | <span data-ttu-id="47a8d-123">値</span><span class="sxs-lookup"><span data-stu-id="47a8d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47a8d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47a8d-124">Authorization</span></span>  | <span data-ttu-id="47a8d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="47a8d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47a8d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="47a8d-127">Request body</span></span>
<span data-ttu-id="47a8d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="47a8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47a8d-129">応答</span><span class="sxs-lookup"><span data-stu-id="47a8d-129">Response</span></span>
<span data-ttu-id="47a8d-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="47a8d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47a8d-132">例</span><span class="sxs-lookup"><span data-stu-id="47a8d-132">Example</span></span>
<span data-ttu-id="47a8d-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="47a8d-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47a8d-134">要求</span><span class="sxs-lookup"><span data-stu-id="47a8d-134">Request</span></span>
<span data-ttu-id="47a8d-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47a8d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="47a8d-136">応答</span><span class="sxs-lookup"><span data-stu-id="47a8d-136">Response</span></span>
<span data-ttu-id="47a8d-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47a8d-137">The following is an example of the response.</span></span>

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
