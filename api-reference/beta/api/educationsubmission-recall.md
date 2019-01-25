---
title: 'educationSubmission: リコール'
description: '受講者が提出書類を取り戻すしようとしたことを示します。 このアクションは、学生によってのみ実行できます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0be94d2888223ca31e37b71e490c4a9fdc28b7d0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520418"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="bffa6-104">educationSubmission: リコール</span><span class="sxs-lookup"><span data-stu-id="bffa6-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bffa6-105">受講者が提出書類を取り戻すしようとしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="bffa6-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="bffa6-106">このアクションは、学生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="bffa6-106">This action can only be done by a student.</span></span> <span data-ttu-id="bffa6-107">「送信」からの提出書類のステータスを変更すると、「処理中」に戻るには。</span><span class="sxs-lookup"><span data-stu-id="bffa6-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="bffa6-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bffa6-108">Permissions</span></span>
<span data-ttu-id="bffa6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bffa6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bffa6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bffa6-111">Permission type</span></span>      | <span data-ttu-id="bffa6-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bffa6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bffa6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bffa6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="bffa6-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bffa6-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bffa6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bffa6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bffa6-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="bffa6-116">Not supported</span></span>  |
|<span data-ttu-id="bffa6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bffa6-117">Application</span></span> |<span data-ttu-id="bffa6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bffa6-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="bffa6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bffa6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="bffa6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bffa6-120">Request headers</span></span>
| <span data-ttu-id="bffa6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bffa6-121">Header</span></span>       | <span data-ttu-id="bffa6-122">値</span><span class="sxs-lookup"><span data-stu-id="bffa6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bffa6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bffa6-123">Authorization</span></span>  | <span data-ttu-id="bffa6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bffa6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bffa6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bffa6-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bffa6-127">応答</span><span class="sxs-lookup"><span data-stu-id="bffa6-127">Response</span></span>
<span data-ttu-id="bffa6-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bffa6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bffa6-130">例</span><span class="sxs-lookup"><span data-stu-id="bffa6-130">Example</span></span>
<span data-ttu-id="bffa6-131">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bffa6-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bffa6-132">要求</span><span class="sxs-lookup"><span data-stu-id="bffa6-132">Request</span></span>
<span data-ttu-id="bffa6-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffa6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="bffa6-134">応答</span><span class="sxs-lookup"><span data-stu-id="bffa6-134">Response</span></span>
<span data-ttu-id="bffa6-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffa6-135">The following is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-recall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
