---
title: EducationSubmissionResource の削除
description: 提出物からリソースを削除します。 この操作は、学生だけが行うことができます。 リソースが割り当てからコピーされた場合は、現在のコピーが削除された後に、リソースの新しいコピーが作成されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 056f09adb9bb36a38d613edaf8d0c1220d69bcb3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587783"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="0a909-105">EducationSubmissionResource の削除</span><span class="sxs-lookup"><span data-stu-id="0a909-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a909-106">提出物からリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="0a909-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="0a909-107">この操作は、学生だけが行うことができます。</span><span class="sxs-lookup"><span data-stu-id="0a909-107">This can only be done by the student.</span></span> <span data-ttu-id="0a909-108">リソースが割り当てからコピーされた場合は、現在のコピーが削除された後に、リソースの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="0a909-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="0a909-109">これにより、リソースを元の状態に "リセット" することができます。</span><span class="sxs-lookup"><span data-stu-id="0a909-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="0a909-110">リソースが割り当てからコピーされていないが、学生から追加された場合は、リソースは単に削除されます。</span><span class="sxs-lookup"><span data-stu-id="0a909-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a909-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a909-111">Permissions</span></span>
<span data-ttu-id="0a909-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a909-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a909-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a909-114">Permission type</span></span>      | <span data-ttu-id="0a909-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a909-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a909-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a909-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="0a909-117">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0a909-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0a909-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a909-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0a909-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a909-119">Not supported.</span></span>  |
|<span data-ttu-id="0a909-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a909-120">Application</span></span> | <span data-ttu-id="0a909-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a909-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0a909-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a909-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0a909-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a909-123">Request headers</span></span>
| <span data-ttu-id="0a909-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a909-124">Header</span></span>       | <span data-ttu-id="0a909-125">値</span><span class="sxs-lookup"><span data-stu-id="0a909-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a909-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a909-126">Authorization</span></span>  | <span data-ttu-id="0a909-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a909-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a909-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a909-129">Request body</span></span>
<span data-ttu-id="0a909-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a909-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0a909-131">応答</span><span class="sxs-lookup"><span data-stu-id="0a909-131">Response</span></span>
<span data-ttu-id="0a909-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0a909-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a909-134">例</span><span class="sxs-lookup"><span data-stu-id="0a909-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a909-135">要求</span><span class="sxs-lookup"><span data-stu-id="0a909-135">Request</span></span>
<span data-ttu-id="0a909-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a909-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="0a909-137">応答</span><span class="sxs-lookup"><span data-stu-id="0a909-137">Response</span></span>
<span data-ttu-id="0a909-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a909-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a909-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0a909-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a909-140">Visual</span><span class="sxs-lookup"><span data-stu-id="0a909-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a909-141">Java</span><span class="sxs-lookup"><span data-stu-id="0a909-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
