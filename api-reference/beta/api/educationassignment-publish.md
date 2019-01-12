---
title: 'educationAssignment: 発行'
description: この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。 クラスの先生だけでは、この呼び出しを行うことができます。 割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。 この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c7cdaebb91490270cc0a8f205b41a89b662a7a13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926702"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="2f61c-106">educationAssignment: 発行</span><span class="sxs-lookup"><span data-stu-id="2f61c-106">educationAssignment: publish</span></span>

> <span data-ttu-id="2f61c-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2f61c-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f61c-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f61c-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f61c-109">この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。</span><span class="sxs-lookup"><span data-stu-id="2f61c-109">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="2f61c-110">クラスの先生だけでは、この呼び出しを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="2f61c-110">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="2f61c-111">割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="2f61c-111">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="2f61c-112">この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2f61c-112">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f61c-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f61c-113">Permissions</span></span>
<span data-ttu-id="2f61c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f61c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f61c-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f61c-116">Permission type</span></span>      | <span data-ttu-id="2f61c-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f61c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f61c-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f61c-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f61c-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f61c-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2f61c-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f61c-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f61c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f61c-121">Not supported.</span></span>  |
|<span data-ttu-id="2f61c-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f61c-122">Application</span></span> | <span data-ttu-id="2f61c-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f61c-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f61c-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f61c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="2f61c-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f61c-125">Request headers</span></span>
| <span data-ttu-id="2f61c-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f61c-126">Header</span></span>       | <span data-ttu-id="2f61c-127">値</span><span class="sxs-lookup"><span data-stu-id="2f61c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f61c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f61c-128">Authorization</span></span>  | <span data-ttu-id="2f61c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f61c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f61c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f61c-131">Request body</span></span>
<span data-ttu-id="2f61c-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f61c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f61c-133">応答</span><span class="sxs-lookup"><span data-stu-id="2f61c-133">Response</span></span>
<span data-ttu-id="2f61c-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2f61c-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f61c-136">例</span><span class="sxs-lookup"><span data-stu-id="2f61c-136">Example</span></span>
<span data-ttu-id="2f61c-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2f61c-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f61c-138">要求</span><span class="sxs-lookup"><span data-stu-id="2f61c-138">Request</span></span>
<span data-ttu-id="2f61c-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f61c-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="2f61c-140">応答</span><span class="sxs-lookup"><span data-stu-id="2f61c-140">Response</span></span>
<span data-ttu-id="2f61c-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f61c-141">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
