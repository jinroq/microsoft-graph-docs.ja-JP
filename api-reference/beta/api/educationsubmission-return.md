---
title: 'educationSubmission: 戻る'
description: この操作によって、評価とフィードバックを受講者に利用可能なこの送信に関連付けられています。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b1772788230b5220b3bdc6813b122d1158e26ab2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511241"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="cabe8-103">educationSubmission: 戻る</span><span class="sxs-lookup"><span data-stu-id="cabe8-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cabe8-104">この操作によって、評価とフィードバックを受講者に利用可能なこの送信に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="cabe8-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="cabe8-105">これは「取得」から「送信」の提出書類のステータスが変更され、フィードバックを提供するか、グレーディングを行うことを示します。</span><span class="sxs-lookup"><span data-stu-id="cabe8-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="cabe8-106">このアクションは、先生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="cabe8-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="cabe8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cabe8-107">Permissions</span></span>
<span data-ttu-id="cabe8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cabe8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cabe8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cabe8-110">Permission type</span></span>      | <span data-ttu-id="cabe8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cabe8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cabe8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cabe8-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cabe8-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cabe8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="cabe8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cabe8-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cabe8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cabe8-115">Not supported.</span></span>  |
|<span data-ttu-id="cabe8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cabe8-116">Application</span></span> | <span data-ttu-id="cabe8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cabe8-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cabe8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cabe8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="cabe8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cabe8-119">Request headers</span></span>
| <span data-ttu-id="cabe8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cabe8-120">Header</span></span>       | <span data-ttu-id="cabe8-121">値</span><span class="sxs-lookup"><span data-stu-id="cabe8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cabe8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cabe8-122">Authorization</span></span>  | <span data-ttu-id="cabe8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cabe8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cabe8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cabe8-125">Request body</span></span>
<span data-ttu-id="cabe8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cabe8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cabe8-127">応答</span><span class="sxs-lookup"><span data-stu-id="cabe8-127">Response</span></span>
<span data-ttu-id="cabe8-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cabe8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cabe8-130">例</span><span class="sxs-lookup"><span data-stu-id="cabe8-130">Example</span></span>
<span data-ttu-id="cabe8-131">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cabe8-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cabe8-132">要求</span><span class="sxs-lookup"><span data-stu-id="cabe8-132">Request</span></span>
<span data-ttu-id="cabe8-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cabe8-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="cabe8-134">応答</span><span class="sxs-lookup"><span data-stu-id="cabe8-134">Response</span></span>
<span data-ttu-id="cabe8-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cabe8-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
