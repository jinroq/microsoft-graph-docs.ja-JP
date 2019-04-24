---
title: accessreview の削除
description: Azure AD access レビュー機能で、accessreview オブジェクトを削除します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456816"
---
# <a name="delete-accessreview"></a><span data-ttu-id="c810e-103">accessreview の削除</span><span class="sxs-lookup"><span data-stu-id="c810e-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c810e-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c810e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c810e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c810e-105">Permissions</span></span>
<span data-ttu-id="c810e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c810e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c810e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c810e-108">Permission type</span></span>                        | <span data-ttu-id="c810e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c810e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c810e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c810e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c810e-111">また、programcontrol を使用して完全なシナリオを実行する必要があります。また、programcontrol を削除する方法については、「プログラムを削除する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c810e-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="c810e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c810e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c810e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c810e-113">Not supported.</span></span> |
|<span data-ttu-id="c810e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c810e-114">Application</span></span>                            | <span data-ttu-id="c810e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c810e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c810e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c810e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="c810e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c810e-117">Request headers</span></span>
| <span data-ttu-id="c810e-118">名前</span><span class="sxs-lookup"><span data-stu-id="c810e-118">Name</span></span>         | <span data-ttu-id="c810e-119">型</span><span class="sxs-lookup"><span data-stu-id="c810e-119">Type</span></span>        | <span data-ttu-id="c810e-120">説明</span><span class="sxs-lookup"><span data-stu-id="c810e-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c810e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c810e-121">Authorization</span></span> | <span data-ttu-id="c810e-122">string</span><span class="sxs-lookup"><span data-stu-id="c810e-122">string</span></span> | <span data-ttu-id="c810e-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="c810e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c810e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c810e-125">Request body</span></span>
<span data-ttu-id="c810e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c810e-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c810e-127">応答</span><span class="sxs-lookup"><span data-stu-id="c810e-127">Response</span></span>
<span data-ttu-id="c810e-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c810e-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c810e-130">例</span><span class="sxs-lookup"><span data-stu-id="c810e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c810e-131">要求</span><span class="sxs-lookup"><span data-stu-id="c810e-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="c810e-132">応答</span><span class="sxs-lookup"><span data-stu-id="c810e-132">Response</span></span>
><span data-ttu-id="c810e-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c810e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
