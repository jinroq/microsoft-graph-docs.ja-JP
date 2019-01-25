---
title: AccessReview を削除します。
description: Azure AD のレビュー機能にアクセス、accessReview オブジェクトを削除します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527774"
---
# <a name="delete-accessreview"></a><span data-ttu-id="2badf-103">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="2badf-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2badf-104">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2badf-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2badf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2badf-105">Permissions</span></span>
<span data-ttu-id="2badf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2badf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2badf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2badf-108">Permission type</span></span>                        | <span data-ttu-id="2badf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2badf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2badf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2badf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2badf-111">AccessReview.ReadWrite.All と、デバッギングを削除する呼び出しの完全なシナリオを ProgramControl.ReadWrite.All する必要があり、</span><span class="sxs-lookup"><span data-stu-id="2badf-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="2badf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2badf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2badf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2badf-113">Not supported.</span></span> |
|<span data-ttu-id="2badf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2badf-114">Application</span></span>                            | <span data-ttu-id="2badf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2badf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2badf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2badf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="2badf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2badf-117">Request headers</span></span>
| <span data-ttu-id="2badf-118">名前</span><span class="sxs-lookup"><span data-stu-id="2badf-118">Name</span></span>         | <span data-ttu-id="2badf-119">型</span><span class="sxs-lookup"><span data-stu-id="2badf-119">Type</span></span>        | <span data-ttu-id="2badf-120">説明</span><span class="sxs-lookup"><span data-stu-id="2badf-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2badf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2badf-121">Authorization</span></span> | <span data-ttu-id="2badf-122">string</span><span class="sxs-lookup"><span data-stu-id="2badf-122">string</span></span> | <span data-ttu-id="2badf-123">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="2badf-123">Bearer \{token\}.</span></span> <span data-ttu-id="2badf-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="2badf-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2badf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2badf-125">Request body</span></span>
<span data-ttu-id="2badf-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2badf-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2badf-127">応答</span><span class="sxs-lookup"><span data-stu-id="2badf-127">Response</span></span>
<span data-ttu-id="2badf-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2badf-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2badf-130">例</span><span class="sxs-lookup"><span data-stu-id="2badf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2badf-131">要求</span><span class="sxs-lookup"><span data-stu-id="2badf-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="2badf-132">応答</span><span class="sxs-lookup"><span data-stu-id="2badf-132">Response</span></span>
><span data-ttu-id="2badf-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2badf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
