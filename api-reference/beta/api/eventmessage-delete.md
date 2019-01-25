---
title: eventMessage の削除
description: eventMessage を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f1f58adff84326397b6b3f4bc340fcbf79d94cb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509729"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="eed8a-103">eventMessage の削除</span><span class="sxs-lookup"><span data-stu-id="eed8a-103">Delete eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eed8a-104">eventMessage を削除します。</span><span class="sxs-lookup"><span data-stu-id="eed8a-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="eed8a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eed8a-105">Permissions</span></span>
<span data-ttu-id="eed8a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eed8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed8a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eed8a-108">Permission type</span></span>      | <span data-ttu-id="eed8a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eed8a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eed8a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eed8a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eed8a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eed8a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eed8a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eed8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eed8a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eed8a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eed8a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eed8a-114">Application</span></span> | <span data-ttu-id="eed8a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eed8a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eed8a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eed8a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eed8a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eed8a-117">Request headers</span></span>
| <span data-ttu-id="eed8a-118">名前</span><span class="sxs-lookup"><span data-stu-id="eed8a-118">Name</span></span>       | <span data-ttu-id="eed8a-119">型</span><span class="sxs-lookup"><span data-stu-id="eed8a-119">Type</span></span> | <span data-ttu-id="eed8a-120">説明</span><span class="sxs-lookup"><span data-stu-id="eed8a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eed8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eed8a-121">Authorization</span></span>  | <span data-ttu-id="eed8a-122">string</span><span class="sxs-lookup"><span data-stu-id="eed8a-122">string</span></span>  | <span data-ttu-id="eed8a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eed8a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eed8a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eed8a-125">Request body</span></span>
<span data-ttu-id="eed8a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eed8a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eed8a-127">応答</span><span class="sxs-lookup"><span data-stu-id="eed8a-127">Response</span></span>

<span data-ttu-id="eed8a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="eed8a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed8a-130">例</span><span class="sxs-lookup"><span data-stu-id="eed8a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eed8a-131">要求</span><span class="sxs-lookup"><span data-stu-id="eed8a-131">Request</span></span>
<span data-ttu-id="eed8a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eed8a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="eed8a-133">応答</span><span class="sxs-lookup"><span data-stu-id="eed8a-133">Response</span></span>
<span data-ttu-id="eed8a-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eed8a-134">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
