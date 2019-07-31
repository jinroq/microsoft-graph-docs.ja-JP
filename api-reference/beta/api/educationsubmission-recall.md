---
title: 'educationSubmission: 呼び戻し'
description: '学生が提出を希望していることを示します。 この操作は、学生のみが行うことができます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37d34685aabe00bff82de453e68a8ebba36aa3a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955081"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="7df2b-104">educationSubmission: 呼び戻し</span><span class="sxs-lookup"><span data-stu-id="7df2b-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7df2b-105">学生が提出を希望していることを示します。</span><span class="sxs-lookup"><span data-stu-id="7df2b-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="7df2b-106">この操作は、学生のみが行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7df2b-106">This action can only be done by a student.</span></span> <span data-ttu-id="7df2b-107">送信の状態は "送信済み" から "作業" に変更されます。</span><span class="sxs-lookup"><span data-stu-id="7df2b-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="7df2b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7df2b-108">Permissions</span></span>

<span data-ttu-id="7df2b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7df2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7df2b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7df2b-111">Permission type</span></span>                        | <span data-ttu-id="7df2b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7df2b-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="7df2b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7df2b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7df2b-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="7df2b-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7df2b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7df2b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7df2b-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="7df2b-116">Not supported</span></span>                                           |
| <span data-ttu-id="7df2b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7df2b-117">Application</span></span>                            | <span data-ttu-id="7df2b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7df2b-118">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="7df2b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7df2b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a><span data-ttu-id="7df2b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7df2b-120">Request headers</span></span>

| <span data-ttu-id="7df2b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7df2b-121">Header</span></span>        | <span data-ttu-id="7df2b-122">値</span><span class="sxs-lookup"><span data-stu-id="7df2b-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7df2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7df2b-123">Authorization</span></span> | <span data-ttu-id="7df2b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7df2b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7df2b-126">応答</span><span class="sxs-lookup"><span data-stu-id="7df2b-126">Response</span></span>

<span data-ttu-id="7df2b-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7df2b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7df2b-129">例</span><span class="sxs-lookup"><span data-stu-id="7df2b-129">Example</span></span>

<span data-ttu-id="7df2b-130">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7df2b-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7df2b-131">要求</span><span class="sxs-lookup"><span data-stu-id="7df2b-131">Request</span></span>

<span data-ttu-id="7df2b-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7df2b-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="7df2b-133">応答</span><span class="sxs-lookup"><span data-stu-id="7df2b-133">Response</span></span>

<span data-ttu-id="7df2b-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7df2b-134">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
