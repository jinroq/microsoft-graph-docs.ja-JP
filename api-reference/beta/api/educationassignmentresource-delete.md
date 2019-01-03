---
title: EducationAssignmentResource を削除します。
description: .
author: dipakboyed
ms.openlocfilehash: 304ec56c8b2da36626f226104568cd353e58e88b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322646"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="8fa4f-103">EducationAssignmentResource を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-103">Delete educationAssignmentResource</span></span>

> <span data-ttu-id="8fa4f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fa4f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fa4f-106">割り当てからリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-106">Delete a resource from an assignment.</span></span> <span data-ttu-id="8fa4f-107">クラスの教師だけでは、リソースを削除できます。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-107">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="8fa4f-108">受講者に割り当てが公開された後、先生は"distributeToStudents"としてマークされているリソースを削除できません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-108">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="8fa4f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8fa4f-109">Permissions</span></span>
<span data-ttu-id="8fa4f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fa4f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8fa4f-112">Permission type</span></span>      | <span data-ttu-id="8fa4f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8fa4f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fa4f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8fa4f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8fa4f-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fa4f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8fa4f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8fa4f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8fa4f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-117">Not supported.</span></span>  |
|<span data-ttu-id="8fa4f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8fa4f-118">Application</span></span> | <span data-ttu-id="8fa4f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8fa4f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8fa4f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8fa4f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fa4f-121">Request headers</span></span>
| <span data-ttu-id="8fa4f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fa4f-122">Header</span></span>       | <span data-ttu-id="8fa4f-123">値</span><span class="sxs-lookup"><span data-stu-id="8fa4f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fa4f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fa4f-124">Authorization</span></span>  | <span data-ttu-id="8fa4f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fa4f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8fa4f-127">Request body</span></span>
<span data-ttu-id="8fa4f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8fa4f-129">応答</span><span class="sxs-lookup"><span data-stu-id="8fa4f-129">Response</span></span>
<span data-ttu-id="8fa4f-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fa4f-132">例</span><span class="sxs-lookup"><span data-stu-id="8fa4f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fa4f-133">要求</span><span class="sxs-lookup"><span data-stu-id="8fa4f-133">Request</span></span>
<span data-ttu-id="8fa4f-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="8fa4f-135">応答</span><span class="sxs-lookup"><span data-stu-id="8fa4f-135">Response</span></span>
<span data-ttu-id="8fa4f-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fa4f-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->