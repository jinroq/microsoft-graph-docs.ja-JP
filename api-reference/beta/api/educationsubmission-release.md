---
title: 'educationSubmission: release'
description: " を指定します。 このアクションは教師のみが実行できます。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ddf437c60ae4ca56a800bd82b081b149a686eabe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955080"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="fd0aa-104">educationSubmission: release</span><span class="sxs-lookup"><span data-stu-id="fd0aa-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd0aa-105">この操作によって、この送信に関連付けられている成績とフィードバックが学生に提供されます。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="fd0aa-106">これにより、送信の状態が "送信済み" から "リリース済み" に変更され、変更が行われたことが示されます。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="fd0aa-107">このアクションは教師のみが実行できます。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd0aa-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd0aa-108">Permissions</span></span>
<span data-ttu-id="fd0aa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd0aa-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd0aa-111">Permission type</span></span>      | <span data-ttu-id="fd0aa-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd0aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd0aa-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd0aa-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd0aa-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="fd0aa-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="fd0aa-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd0aa-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd0aa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-116">Not supported.</span></span>  |
|<span data-ttu-id="fd0aa-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd0aa-117">Application</span></span> | <span data-ttu-id="fd0aa-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fd0aa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd0aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="fd0aa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd0aa-120">Request headers</span></span>
| <span data-ttu-id="fd0aa-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd0aa-121">Header</span></span>       | <span data-ttu-id="fd0aa-122">値</span><span class="sxs-lookup"><span data-stu-id="fd0aa-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd0aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd0aa-123">Authorization</span></span>  | <span data-ttu-id="fd0aa-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd0aa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd0aa-126">Request body</span></span>
<span data-ttu-id="fd0aa-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd0aa-128">応答</span><span class="sxs-lookup"><span data-stu-id="fd0aa-128">Response</span></span>
<span data-ttu-id="fd0aa-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd0aa-131">例</span><span class="sxs-lookup"><span data-stu-id="fd0aa-131">Example</span></span>
<span data-ttu-id="fd0aa-132">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd0aa-133">要求</span><span class="sxs-lookup"><span data-stu-id="fd0aa-133">Request</span></span>
<span data-ttu-id="fd0aa-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="fd0aa-135">応答</span><span class="sxs-lookup"><span data-stu-id="fd0aa-135">Response</span></span>
<span data-ttu-id="fd0aa-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd0aa-136">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
