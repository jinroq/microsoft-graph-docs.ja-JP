---
title: EducationSubmissionResource の削除
description: 提出物からリソースを削除します。 この操作は、学生だけが行うことができます。 リソースが割り当てからコピーされた場合は、現在のコピーが削除された後に、リソースの新しいコピーが作成されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: de8c30b63abf130535669236a170510f9ccda65d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323793"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="11720-105">EducationSubmissionResource の削除</span><span class="sxs-lookup"><span data-stu-id="11720-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11720-106">提出物からリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="11720-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="11720-107">この操作は、学生だけが行うことができます。</span><span class="sxs-lookup"><span data-stu-id="11720-107">This can only be done by the student.</span></span> <span data-ttu-id="11720-108">リソースが割り当てからコピーされた場合は、現在のコピーが削除された後に、リソースの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="11720-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="11720-109">これにより、リソースを元の状態に "リセット" することができます。</span><span class="sxs-lookup"><span data-stu-id="11720-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="11720-110">リソースが割り当てからコピーされていないが、学生から追加された場合は、リソースは単に削除されます。</span><span class="sxs-lookup"><span data-stu-id="11720-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="11720-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11720-111">Permissions</span></span>
<span data-ttu-id="11720-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11720-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11720-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11720-114">Permission type</span></span>      | <span data-ttu-id="11720-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11720-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11720-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11720-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="11720-117">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="11720-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="11720-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11720-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="11720-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11720-119">Not supported.</span></span>  |
|<span data-ttu-id="11720-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11720-120">Application</span></span> | <span data-ttu-id="11720-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11720-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="11720-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11720-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="11720-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11720-123">Request headers</span></span>
| <span data-ttu-id="11720-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11720-124">Header</span></span>       | <span data-ttu-id="11720-125">値</span><span class="sxs-lookup"><span data-stu-id="11720-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11720-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="11720-126">Authorization</span></span>  | <span data-ttu-id="11720-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11720-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11720-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="11720-129">Request body</span></span>
<span data-ttu-id="11720-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11720-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="11720-131">応答</span><span class="sxs-lookup"><span data-stu-id="11720-131">Response</span></span>
<span data-ttu-id="11720-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="11720-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11720-134">例</span><span class="sxs-lookup"><span data-stu-id="11720-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11720-135">要求</span><span class="sxs-lookup"><span data-stu-id="11720-135">Request</span></span>
<span data-ttu-id="11720-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11720-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11720-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="11720-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11720-138">C#</span><span class="sxs-lookup"><span data-stu-id="11720-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11720-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11720-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11720-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="11720-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="11720-141">Java</span><span class="sxs-lookup"><span data-stu-id="11720-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="11720-142">応答</span><span class="sxs-lookup"><span data-stu-id="11720-142">Response</span></span>
<span data-ttu-id="11720-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11720-143">The following is an example of the response.</span></span> 

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
  ]
}
-->
