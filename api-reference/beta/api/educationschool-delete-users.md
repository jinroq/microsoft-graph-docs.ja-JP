---
title: educationSchool から educationUser を削除する
description: 学校からユーザーを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2a09a56feb648e435ed83109c2d092ce9ada7927
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955195"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="b02e5-103">educationSchool から educationUser を削除する</span><span class="sxs-lookup"><span data-stu-id="b02e5-103">Remove educationUser from an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b02e5-104">学校からユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="b02e5-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b02e5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b02e5-105">Permissions</span></span>

<span data-ttu-id="b02e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b02e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b02e5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b02e5-108">Permission type</span></span>                        | <span data-ttu-id="b02e5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b02e5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b02e5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b02e5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b02e5-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b02e5-111">Not supported.</span></span>                              |
| <span data-ttu-id="b02e5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b02e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b02e5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b02e5-113">Not supported.</span></span>                              |
| <span data-ttu-id="b02e5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b02e5-114">Application</span></span>                            | <span data-ttu-id="b02e5-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b02e5-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="b02e5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b02e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b02e5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b02e5-117">Request headers</span></span>

| <span data-ttu-id="b02e5-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b02e5-118">Header</span></span>        | <span data-ttu-id="b02e5-119">値</span><span class="sxs-lookup"><span data-stu-id="b02e5-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b02e5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b02e5-120">Authorization</span></span> | <span data-ttu-id="b02e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b02e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b02e5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b02e5-123">Request body</span></span>

<span data-ttu-id="b02e5-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b02e5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b02e5-125">応答</span><span class="sxs-lookup"><span data-stu-id="b02e5-125">Response</span></span>

<span data-ttu-id="b02e5-126">成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="b02e5-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b02e5-127">例</span><span class="sxs-lookup"><span data-stu-id="b02e5-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b02e5-128">要求</span><span class="sxs-lookup"><span data-stu-id="b02e5-128">Request</span></span>

<span data-ttu-id="b02e5-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b02e5-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="b02e5-130">応答</span><span class="sxs-lookup"><span data-stu-id="b02e5-130">Response</span></span>

<span data-ttu-id="b02e5-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b02e5-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
