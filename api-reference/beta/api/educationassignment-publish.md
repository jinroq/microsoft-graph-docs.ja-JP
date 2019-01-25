---
title: 'educationAssignment: 発行'
description: この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。 クラスの先生だけでは、この呼び出しを行うことができます。 割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。 この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: bac9c38d5fbd2ce80693a468c0a2d229085f32cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508714"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="f162c-106">educationAssignment: 発行</span><span class="sxs-lookup"><span data-stu-id="f162c-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f162c-107">この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。</span><span class="sxs-lookup"><span data-stu-id="f162c-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="f162c-108">クラスの先生だけでは、この呼び出しを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f162c-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="f162c-109">割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="f162c-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="f162c-110">この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f162c-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="f162c-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f162c-111">Permissions</span></span>
<span data-ttu-id="f162c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f162c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f162c-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f162c-114">Permission type</span></span>      | <span data-ttu-id="f162c-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f162c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f162c-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f162c-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f162c-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f162c-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f162c-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f162c-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f162c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f162c-119">Not supported.</span></span>  |
|<span data-ttu-id="f162c-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f162c-120">Application</span></span> | <span data-ttu-id="f162c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f162c-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f162c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f162c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="f162c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f162c-123">Request headers</span></span>
| <span data-ttu-id="f162c-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f162c-124">Header</span></span>       | <span data-ttu-id="f162c-125">値</span><span class="sxs-lookup"><span data-stu-id="f162c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f162c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f162c-126">Authorization</span></span>  | <span data-ttu-id="f162c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f162c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f162c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f162c-129">Request body</span></span>
<span data-ttu-id="f162c-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f162c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f162c-131">応答</span><span class="sxs-lookup"><span data-stu-id="f162c-131">Response</span></span>
<span data-ttu-id="f162c-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f162c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f162c-134">例</span><span class="sxs-lookup"><span data-stu-id="f162c-134">Example</span></span>
<span data-ttu-id="f162c-135">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f162c-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f162c-136">要求</span><span class="sxs-lookup"><span data-stu-id="f162c-136">Request</span></span>
<span data-ttu-id="f162c-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f162c-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="f162c-138">応答</span><span class="sxs-lookup"><span data-stu-id="f162c-138">Response</span></span>
<span data-ttu-id="f162c-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f162c-139">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
