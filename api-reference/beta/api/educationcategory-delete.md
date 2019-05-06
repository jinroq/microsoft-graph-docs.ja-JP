---
title: EducationCategory の削除
description: 既存のカテゴリを削除します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e7f9d0682c1a279d448e82addb1434f93f2e0ec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587433"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="2dbb7-103">EducationCategory の削除</span><span class="sxs-lookup"><span data-stu-id="2dbb7-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dbb7-104">既存のカテゴリを削除します。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dbb7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2dbb7-105">Permissions</span></span>
<span data-ttu-id="2dbb7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dbb7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2dbb7-108">Permission type</span></span>      | <span data-ttu-id="2dbb7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2dbb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dbb7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2dbb7-110">Delegated (work or school account)</span></span>| <span data-ttu-id="2dbb7-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2dbb7-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="2dbb7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2dbb7-112">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="2dbb7-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-113">Not Supported.</span></span> |
|<span data-ttu-id="2dbb7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2dbb7-114">Application</span></span> | <span data-ttu-id="2dbb7-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-115">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2dbb7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2dbb7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignmentCategories/<id>
```
## <a name="request-headers"></a><span data-ttu-id="2dbb7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dbb7-117">Request headers</span></span>
| <span data-ttu-id="2dbb7-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dbb7-118">Header</span></span>       | <span data-ttu-id="2dbb7-119">値</span><span class="sxs-lookup"><span data-stu-id="2dbb7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2dbb7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dbb7-120">Authorization</span></span>  | <span data-ttu-id="2dbb7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2dbb7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2dbb7-123">Request body</span></span>
<span data-ttu-id="2dbb7-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2dbb7-125">応答</span><span class="sxs-lookup"><span data-stu-id="2dbb7-125">Response</span></span>
<span data-ttu-id="2dbb7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dbb7-128">例</span><span class="sxs-lookup"><span data-stu-id="2dbb7-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="2dbb7-129">要求</span><span class="sxs-lookup"><span data-stu-id="2dbb7-129">Request</span></span>
<span data-ttu-id="2dbb7-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
### <a name="response"></a><span data-ttu-id="2dbb7-131">応答</span><span class="sxs-lookup"><span data-stu-id="2dbb7-131">Response</span></span>
<span data-ttu-id="2dbb7-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2dbb7-132">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2dbb7-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="2dbb7-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2dbb7-134">Visual</span><span class="sxs-lookup"><span data-stu-id="2dbb7-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2dbb7-135">Java</span><span class="sxs-lookup"><span data-stu-id="2dbb7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
