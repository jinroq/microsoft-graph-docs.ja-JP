---
title: 'educationSubmission: リコール'
description: .
ms.openlocfilehash: 8df134a6d8325e5b497baada89bc0fa16d0ee9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067327"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="1276c-103">educationSubmission: リコール</span><span class="sxs-lookup"><span data-stu-id="1276c-103">educationSubmission: recall</span></span>

> <span data-ttu-id="1276c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1276c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1276c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1276c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1276c-106">受講者が提出書類を取り戻すしようとしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="1276c-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="1276c-107">このアクションは、学生によってのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="1276c-107">This action can only be done by a student.</span></span> <span data-ttu-id="1276c-108">「送信」からの提出書類のステータスを変更すると、「処理中」に戻るには。</span><span class="sxs-lookup"><span data-stu-id="1276c-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="1276c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1276c-109">Permissions</span></span>
<span data-ttu-id="1276c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1276c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1276c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1276c-112">Permission type</span></span>      | <span data-ttu-id="1276c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1276c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1276c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1276c-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="1276c-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1276c-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1276c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1276c-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1276c-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1276c-117">Not supported</span></span>  |
|<span data-ttu-id="1276c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1276c-118">Application</span></span> |<span data-ttu-id="1276c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1276c-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1276c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1276c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="1276c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1276c-121">Request headers</span></span>
| <span data-ttu-id="1276c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1276c-122">Header</span></span>       | <span data-ttu-id="1276c-123">値</span><span class="sxs-lookup"><span data-stu-id="1276c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1276c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1276c-124">Authorization</span></span>  | <span data-ttu-id="1276c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1276c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1276c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1276c-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1276c-128">応答</span><span class="sxs-lookup"><span data-stu-id="1276c-128">Response</span></span>
<span data-ttu-id="1276c-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1276c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1276c-131">例</span><span class="sxs-lookup"><span data-stu-id="1276c-131">Example</span></span>
<span data-ttu-id="1276c-132">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1276c-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1276c-133">要求</span><span class="sxs-lookup"><span data-stu-id="1276c-133">Request</span></span>
<span data-ttu-id="1276c-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1276c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="1276c-135">応答</span><span class="sxs-lookup"><span data-stu-id="1276c-135">Response</span></span>
<span data-ttu-id="1276c-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1276c-136">The following is an example of the response.</span></span>

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