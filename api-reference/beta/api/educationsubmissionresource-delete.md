---
title: EducationSubmissionResource を削除します。
description: 提出書類からリソースを削除します。 これは、受講者によってのみ実行できます。 リソースは、割り当てからコピーされた場合は、現在のコピーが削除された後、リソースの新しいコピーが作成されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a735cb1451e8d3eb8df13e6fa395c3e02393f451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518983"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="e7c2c-105">EducationSubmissionResource を削除します。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7c2c-106">提出書類からリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="e7c2c-107">これは、受講者によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-107">This can only be done by the student.</span></span> <span data-ttu-id="e7c2c-108">リソースは、割り当てからコピーされた場合は、現在のコピーが削除された後、リソースの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="e7c2c-109">これにより、リソースを元の状態に「リセット」することができます。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="e7c2c-110">リソースは割り当てからコピーされませんでしたが、受講者から追加された、リソースが単に削除されます。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7c2c-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7c2c-111">Permissions</span></span>
<span data-ttu-id="e7c2c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c2c-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7c2c-114">Permission type</span></span>      | <span data-ttu-id="e7c2c-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7c2c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7c2c-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7c2c-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e7c2c-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7c2c-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e7c2c-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7c2c-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e7c2c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-119">Not supported.</span></span>  |
|<span data-ttu-id="e7c2c-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7c2c-120">Application</span></span> | <span data-ttu-id="e7c2c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7c2c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7c2c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e7c2c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7c2c-123">Request headers</span></span>
| <span data-ttu-id="e7c2c-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7c2c-124">Header</span></span>       | <span data-ttu-id="e7c2c-125">値</span><span class="sxs-lookup"><span data-stu-id="e7c2c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7c2c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c2c-126">Authorization</span></span>  | <span data-ttu-id="e7c2c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7c2c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7c2c-129">Request body</span></span>
<span data-ttu-id="e7c2c-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e7c2c-131">応答</span><span class="sxs-lookup"><span data-stu-id="e7c2c-131">Response</span></span>
<span data-ttu-id="e7c2c-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c2c-134">例</span><span class="sxs-lookup"><span data-stu-id="e7c2c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7c2c-135">要求</span><span class="sxs-lookup"><span data-stu-id="e7c2c-135">Request</span></span>
<span data-ttu-id="e7c2c-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="e7c2c-137">応答</span><span class="sxs-lookup"><span data-stu-id="e7c2c-137">Response</span></span>
<span data-ttu-id="e7c2c-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7c2c-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
