---
title: educationCategory の削除
description: 既存のカテゴリを削除します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c68f4a9950437ddcebc0cd40237bef07c597648
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801016"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="cde78-103">educationCategory の削除</span><span class="sxs-lookup"><span data-stu-id="cde78-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde78-104">既存のカテゴリを削除します。</span><span class="sxs-lookup"><span data-stu-id="cde78-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="cde78-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cde78-105">Permissions</span></span>
<span data-ttu-id="cde78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cde78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cde78-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cde78-108">Permission type</span></span>      | <span data-ttu-id="cde78-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cde78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cde78-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cde78-110">Delegated (work or school account)</span></span>| <span data-ttu-id="cde78-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="cde78-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="cde78-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cde78-112">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="cde78-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cde78-113">Not Supported.</span></span> |
|<span data-ttu-id="cde78-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cde78-114">Application</span></span> | <span data-ttu-id="cde78-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cde78-115">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cde78-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cde78-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignmentCategories/<id>
```
## <a name="request-headers"></a><span data-ttu-id="cde78-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cde78-117">Request headers</span></span>
| <span data-ttu-id="cde78-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cde78-118">Header</span></span>       | <span data-ttu-id="cde78-119">値</span><span class="sxs-lookup"><span data-stu-id="cde78-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cde78-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cde78-120">Authorization</span></span>  | <span data-ttu-id="cde78-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cde78-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cde78-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cde78-123">Request body</span></span>
<span data-ttu-id="cde78-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cde78-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cde78-125">応答</span><span class="sxs-lookup"><span data-stu-id="cde78-125">Response</span></span>
<span data-ttu-id="cde78-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cde78-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cde78-128">例</span><span class="sxs-lookup"><span data-stu-id="cde78-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="cde78-129">要求</span><span class="sxs-lookup"><span data-stu-id="cde78-129">Request</span></span>
<span data-ttu-id="cde78-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cde78-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
### <a name="response"></a><span data-ttu-id="cde78-131">応答</span><span class="sxs-lookup"><span data-stu-id="cde78-131">Response</span></span>
<span data-ttu-id="cde78-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cde78-132">The following is an example of the response.</span></span> 


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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
