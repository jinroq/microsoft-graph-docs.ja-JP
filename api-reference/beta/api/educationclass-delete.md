---
title: educationClass を削除する
description: クラスを削除します。 クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: a7d5f376bd6d70229d8058084946fd474a692212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508161"
---
# <a name="delete-educationclass"></a><span data-ttu-id="bbb98-104">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="bbb98-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbb98-105">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="bbb98-105">Delete a class.</span></span> <span data-ttu-id="bbb98-106">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="bbb98-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb98-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bbb98-107">Permissions</span></span>
<span data-ttu-id="bbb98-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbb98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb98-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbb98-110">Permission type</span></span>      | <span data-ttu-id="bbb98-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbb98-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbb98-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbb98-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="bbb98-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbb98-113">Not supported.</span></span>  |
|<span data-ttu-id="bbb98-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbb98-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bbb98-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbb98-115">Not supported.</span></span>  |
|<span data-ttu-id="bbb98-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbb98-116">Application</span></span> | <span data-ttu-id="bbb98-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb98-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bbb98-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbb98-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bbb98-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbb98-119">Request headers</span></span>
| <span data-ttu-id="bbb98-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbb98-120">Header</span></span>       | <span data-ttu-id="bbb98-121">値</span><span class="sxs-lookup"><span data-stu-id="bbb98-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbb98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbb98-122">Authorization</span></span>  | <span data-ttu-id="bbb98-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bbb98-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbb98-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbb98-125">Request body</span></span>
<span data-ttu-id="bbb98-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bbb98-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bbb98-127">応答</span><span class="sxs-lookup"><span data-stu-id="bbb98-127">Response</span></span>
<span data-ttu-id="bbb98-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bbb98-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb98-130">例</span><span class="sxs-lookup"><span data-stu-id="bbb98-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbb98-131">要求</span><span class="sxs-lookup"><span data-stu-id="bbb98-131">Request</span></span>
<span data-ttu-id="bbb98-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbb98-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="bbb98-133">応答</span><span class="sxs-lookup"><span data-stu-id="bbb98-133">Response</span></span>
<span data-ttu-id="bbb98-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbb98-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
