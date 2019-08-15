---
title: EducationRubric の削除
description: EducationRubric オブジェクトを削除します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: aae747b530e5109fbf56048b34be4b6a418f019c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416220"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="fd0e3-103">EducationRubric の削除</span><span class="sxs-lookup"><span data-stu-id="fd0e3-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd0e3-104">[EducationRubric](../resources/educationrubric.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd0e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd0e3-105">Permissions</span></span>

<span data-ttu-id="fd0e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd0e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd0e3-108">Permission type</span></span>                        | <span data-ttu-id="fd0e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd0e3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fd0e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd0e3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd0e3-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="fd0e3-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="fd0e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd0e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd0e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-113">Not supported.</span></span> |
| <span data-ttu-id="fd0e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd0e3-114">Application</span></span>                            | <span data-ttu-id="fd0e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd0e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd0e3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fd0e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd0e3-117">Request headers</span></span>

| <span data-ttu-id="fd0e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="fd0e3-118">Name</span></span>          | <span data-ttu-id="fd0e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="fd0e3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fd0e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd0e3-120">Authorization</span></span> | <span data-ttu-id="fd0e3-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="fd0e3-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd0e3-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd0e3-122">Request body</span></span>

<span data-ttu-id="fd0e3-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd0e3-124">応答</span><span class="sxs-lookup"><span data-stu-id="fd0e3-124">Response</span></span>

<span data-ttu-id="fd0e3-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd0e3-127">例</span><span class="sxs-lookup"><span data-stu-id="fd0e3-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd0e3-128">要求</span><span class="sxs-lookup"><span data-stu-id="fd0e3-128">Request</span></span>

<span data-ttu-id="fd0e3-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```

### <a name="response"></a><span data-ttu-id="fd0e3-130">応答</span><span class="sxs-lookup"><span data-stu-id="fd0e3-130">Response</span></span>

<span data-ttu-id="fd0e3-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd0e3-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
