---
title: educationAssignment の削除
description: 既存の割り当てを削除します。 割り当てを削除できるのは、クラス内の教師だけです。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2356330a75558ea88b94c9266fb2d4a387e87b59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464741"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="29d7b-104">educationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="29d7b-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29d7b-105">既存の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="29d7b-105">Delete an existing assignment.</span></span> <span data-ttu-id="29d7b-106">割り当てを削除できるのは、クラス内の教師だけです。</span><span class="sxs-lookup"><span data-stu-id="29d7b-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="29d7b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29d7b-107">Permissions</span></span>
<span data-ttu-id="29d7b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29d7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d7b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29d7b-110">Permission type</span></span>      | <span data-ttu-id="29d7b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29d7b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d7b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29d7b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="29d7b-113">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="29d7b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="29d7b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29d7b-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="29d7b-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="29d7b-115">Not Supported.</span></span> |
|<span data-ttu-id="29d7b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29d7b-116">Application</span></span> | <span data-ttu-id="29d7b-117">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="29d7b-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="29d7b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29d7b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="29d7b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d7b-119">Request headers</span></span>
| <span data-ttu-id="29d7b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d7b-120">Header</span></span>       | <span data-ttu-id="29d7b-121">値</span><span class="sxs-lookup"><span data-stu-id="29d7b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29d7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d7b-122">Authorization</span></span>  | <span data-ttu-id="29d7b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29d7b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29d7b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="29d7b-125">Request body</span></span>
<span data-ttu-id="29d7b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29d7b-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="29d7b-127">応答</span><span class="sxs-lookup"><span data-stu-id="29d7b-127">Response</span></span>
<span data-ttu-id="29d7b-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="29d7b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d7b-130">例</span><span class="sxs-lookup"><span data-stu-id="29d7b-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="29d7b-131">要求</span><span class="sxs-lookup"><span data-stu-id="29d7b-131">Request</span></span>
<span data-ttu-id="29d7b-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29d7b-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="29d7b-133">応答</span><span class="sxs-lookup"><span data-stu-id="29d7b-133">Response</span></span>
<span data-ttu-id="29d7b-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29d7b-134">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
