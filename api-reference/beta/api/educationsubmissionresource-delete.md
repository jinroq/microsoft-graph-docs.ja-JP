---
title: EducationSubmissionResource を削除します。
description: 提出書類からリソースを削除します。 これは、受講者によってのみ実行できます。 リソースは、割り当てからコピーされた場合は、現在のコピーが削除された後、リソースの新しいコピーが作成されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 657e05a5a60dd90c8fd0c769b7d978c4be617201
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945728"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="1e430-105">EducationSubmissionResource を削除します。</span><span class="sxs-lookup"><span data-stu-id="1e430-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="1e430-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e430-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e430-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e430-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e430-108">提出書類からリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="1e430-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="1e430-109">これは、受講者によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="1e430-109">This can only be done by the student.</span></span> <span data-ttu-id="1e430-110">リソースは、割り当てからコピーされた場合は、現在のコピーが削除された後、リソースの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1e430-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="1e430-111">これにより、リソースを元の状態に「リセット」することができます。</span><span class="sxs-lookup"><span data-stu-id="1e430-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="1e430-112">リソースは割り当てからコピーされませんでしたが、受講者から追加された、リソースが単に削除されます。</span><span class="sxs-lookup"><span data-stu-id="1e430-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e430-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e430-113">Permissions</span></span>
<span data-ttu-id="1e430-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e430-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e430-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e430-116">Permission type</span></span>      | <span data-ttu-id="1e430-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e430-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e430-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e430-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="1e430-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e430-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1e430-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e430-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1e430-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e430-121">Not supported.</span></span>  |
|<span data-ttu-id="1e430-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e430-122">Application</span></span> | <span data-ttu-id="1e430-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e430-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1e430-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e430-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1e430-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e430-125">Request headers</span></span>
| <span data-ttu-id="1e430-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e430-126">Header</span></span>       | <span data-ttu-id="1e430-127">値</span><span class="sxs-lookup"><span data-stu-id="1e430-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e430-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e430-128">Authorization</span></span>  | <span data-ttu-id="1e430-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e430-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e430-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e430-131">Request body</span></span>
<span data-ttu-id="1e430-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e430-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1e430-133">応答</span><span class="sxs-lookup"><span data-stu-id="1e430-133">Response</span></span>
<span data-ttu-id="1e430-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1e430-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e430-136">例</span><span class="sxs-lookup"><span data-stu-id="1e430-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e430-137">要求</span><span class="sxs-lookup"><span data-stu-id="1e430-137">Request</span></span>
<span data-ttu-id="1e430-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e430-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="1e430-139">応答</span><span class="sxs-lookup"><span data-stu-id="1e430-139">Response</span></span>
<span data-ttu-id="1e430-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e430-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
