---
title: 'educationSubmission: 呼び戻し'
description: '学生が提出を希望していることを示します。 この操作は、学生のみが行うことができます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 847dfc4d3e868243ea8120fee927fe1397a4826c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322949"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="130d3-104">educationSubmission: 呼び戻し</span><span class="sxs-lookup"><span data-stu-id="130d3-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="130d3-105">学生が提出を希望していることを示します。</span><span class="sxs-lookup"><span data-stu-id="130d3-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="130d3-106">この操作は、学生のみが行うことができます。</span><span class="sxs-lookup"><span data-stu-id="130d3-106">This action can only be done by a student.</span></span> <span data-ttu-id="130d3-107">送信の状態は "送信済み" から "作業" に変更されます。</span><span class="sxs-lookup"><span data-stu-id="130d3-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="130d3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="130d3-108">Permissions</span></span>
<span data-ttu-id="130d3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="130d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130d3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="130d3-111">Permission type</span></span>      | <span data-ttu-id="130d3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="130d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="130d3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="130d3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="130d3-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="130d3-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="130d3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="130d3-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="130d3-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="130d3-116">Not supported</span></span>  |
|<span data-ttu-id="130d3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="130d3-117">Application</span></span> |<span data-ttu-id="130d3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="130d3-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="130d3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="130d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="130d3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="130d3-120">Request headers</span></span>
| <span data-ttu-id="130d3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="130d3-121">Header</span></span>       | <span data-ttu-id="130d3-122">値</span><span class="sxs-lookup"><span data-stu-id="130d3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="130d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="130d3-123">Authorization</span></span>  | <span data-ttu-id="130d3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="130d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="130d3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="130d3-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="130d3-127">応答</span><span class="sxs-lookup"><span data-stu-id="130d3-127">Response</span></span>
<span data-ttu-id="130d3-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="130d3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130d3-130">例</span><span class="sxs-lookup"><span data-stu-id="130d3-130">Example</span></span>
<span data-ttu-id="130d3-131">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="130d3-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="130d3-132">要求</span><span class="sxs-lookup"><span data-stu-id="130d3-132">Request</span></span>
<span data-ttu-id="130d3-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="130d3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="130d3-134">応答</span><span class="sxs-lookup"><span data-stu-id="130d3-134">Response</span></span>
<span data-ttu-id="130d3-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="130d3-135">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
