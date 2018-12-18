---
title: 'educationSubmission: リコール'
description: '受講者が提出書類を取り戻すしようとしたことを示します。 このアクションは、学生によってのみ実行できます。 '
author: dipakboyed
ms.openlocfilehash: ad49302ac9010923d0da2e31686ae4f6967bb50b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302318"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="94b20-104">educationSubmission: リコール</span><span class="sxs-lookup"><span data-stu-id="94b20-104">educationSubmission: recall</span></span>

> <span data-ttu-id="94b20-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94b20-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94b20-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b20-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94b20-107">受講者が提出書類を取り戻すしようとしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="94b20-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="94b20-108">このアクションは、学生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="94b20-108">This action can only be done by a student.</span></span> <span data-ttu-id="94b20-109">「送信」からの提出書類のステータスを変更すると、「処理中」に戻るには。</span><span class="sxs-lookup"><span data-stu-id="94b20-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="94b20-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94b20-110">Permissions</span></span>
<span data-ttu-id="94b20-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94b20-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b20-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94b20-113">Permission type</span></span>      | <span data-ttu-id="94b20-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94b20-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94b20-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94b20-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="94b20-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b20-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="94b20-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94b20-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="94b20-118">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="94b20-118">Not supported</span></span>  |
|<span data-ttu-id="94b20-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94b20-119">Application</span></span> |<span data-ttu-id="94b20-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b20-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="94b20-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94b20-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="94b20-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94b20-122">Request headers</span></span>
| <span data-ttu-id="94b20-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94b20-123">Header</span></span>       | <span data-ttu-id="94b20-124">値</span><span class="sxs-lookup"><span data-stu-id="94b20-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94b20-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="94b20-125">Authorization</span></span>  | <span data-ttu-id="94b20-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94b20-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94b20-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="94b20-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="94b20-129">応答</span><span class="sxs-lookup"><span data-stu-id="94b20-129">Response</span></span>
<span data-ttu-id="94b20-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="94b20-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94b20-132">例</span><span class="sxs-lookup"><span data-stu-id="94b20-132">Example</span></span>
<span data-ttu-id="94b20-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="94b20-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94b20-134">要求</span><span class="sxs-lookup"><span data-stu-id="94b20-134">Request</span></span>
<span data-ttu-id="94b20-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94b20-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="94b20-136">応答</span><span class="sxs-lookup"><span data-stu-id="94b20-136">Response</span></span>
<span data-ttu-id="94b20-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94b20-137">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->