---
title: EducationAssignment を削除します。
description: 既存の割り当てを削除します。 クラス内での教師だけでは、割り当てを削除できます。
ms.openlocfilehash: e9965efa458459cff0c3914dbc12b37153a6ab51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071399"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="c8d0c-104">EducationAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-104">Delete educationAssignment</span></span>

> <span data-ttu-id="c8d0c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8d0c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8d0c-107">既存の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-107">Delete an existing assignment.</span></span> <span data-ttu-id="c8d0c-108">クラス内での教師だけでは、割り当てを削除できます。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-108">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8d0c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8d0c-109">Permissions</span></span>
<span data-ttu-id="c8d0c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d0c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8d0c-112">Permission type</span></span>      | <span data-ttu-id="c8d0c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8d0c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8d0c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8d0c-114">Delegated (work or school account)</span></span>| <span data-ttu-id="c8d0c-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8d0c-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="c8d0c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8d0c-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="c8d0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-117">Not Supported.</span></span> |
|<span data-ttu-id="c8d0c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8d0c-118">Application</span></span> | <span data-ttu-id="c8d0c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-119">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c8d0c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8d0c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="c8d0c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8d0c-121">Request headers</span></span>
| <span data-ttu-id="c8d0c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8d0c-122">Header</span></span>       | <span data-ttu-id="c8d0c-123">値</span><span class="sxs-lookup"><span data-stu-id="c8d0c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8d0c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8d0c-124">Authorization</span></span>  | <span data-ttu-id="c8d0c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8d0c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8d0c-127">Request body</span></span>
<span data-ttu-id="c8d0c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c8d0c-129">応答</span><span class="sxs-lookup"><span data-stu-id="c8d0c-129">Response</span></span>
<span data-ttu-id="c8d0c-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8d0c-132">例</span><span class="sxs-lookup"><span data-stu-id="c8d0c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8d0c-133">要求</span><span class="sxs-lookup"><span data-stu-id="c8d0c-133">Request</span></span>
<span data-ttu-id="c8d0c-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="c8d0c-135">応答</span><span class="sxs-lookup"><span data-stu-id="c8d0c-135">Response</span></span>
<span data-ttu-id="c8d0c-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8d0c-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->