---
title: 契約を削除します。
description: 契約オブジェクトを削除します。
localization_priority: Normal
ms.openlocfilehash: 95766f28e5456c1b4f410de65ae12dccd881727e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521321"
---
# <a name="delete-agreement"></a><span data-ttu-id="3249d-103">契約を削除します。</span><span class="sxs-lookup"><span data-stu-id="3249d-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3249d-104">[契約](../resources/agreement.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3249d-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3249d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3249d-105">Permissions</span></span>
<span data-ttu-id="3249d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3249d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3249d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3249d-108">Permission type</span></span>                        | <span data-ttu-id="3249d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3249d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3249d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3249d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3249d-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3249d-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="3249d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3249d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3249d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3249d-113">Not supported.</span></span> |
|<span data-ttu-id="3249d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3249d-114">Application</span></span>                            | <span data-ttu-id="3249d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3249d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3249d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3249d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="3249d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3249d-117">Request headers</span></span>
| <span data-ttu-id="3249d-118">名前</span><span class="sxs-lookup"><span data-stu-id="3249d-118">Name</span></span>         | <span data-ttu-id="3249d-119">型</span><span class="sxs-lookup"><span data-stu-id="3249d-119">Type</span></span>        | <span data-ttu-id="3249d-120">説明</span><span class="sxs-lookup"><span data-stu-id="3249d-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3249d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3249d-121">Authorization</span></span> | <span data-ttu-id="3249d-122">string</span><span class="sxs-lookup"><span data-stu-id="3249d-122">string</span></span> | <span data-ttu-id="3249d-123">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="3249d-123">Bearer \{token\}.</span></span> <span data-ttu-id="3249d-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="3249d-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3249d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3249d-125">Request body</span></span>
<span data-ttu-id="3249d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3249d-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3249d-127">応答</span><span class="sxs-lookup"><span data-stu-id="3249d-127">Response</span></span>
<span data-ttu-id="3249d-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3249d-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3249d-130">例</span><span class="sxs-lookup"><span data-stu-id="3249d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3249d-131">要求</span><span class="sxs-lookup"><span data-stu-id="3249d-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="3249d-132">応答</span><span class="sxs-lookup"><span data-stu-id="3249d-132">Response</span></span>
><span data-ttu-id="3249d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3249d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
