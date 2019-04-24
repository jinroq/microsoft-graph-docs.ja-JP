---
title: directoryObject を削除する
description: directoryobject を削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63e9d4574c505158171c93fd7ac9dc51678c7d2b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455094"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="b4cc9-103">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="b4cc9-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cc9-104">directoryobject を削除します。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4cc9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4cc9-105">Permissions</span></span>
<span data-ttu-id="b4cc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b4cc9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4cc9-108">Permission type</span></span>      | <span data-ttu-id="b4cc9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4cc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4cc9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4cc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4cc9-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4cc9-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4cc9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4cc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4cc9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-113">Not supported.</span></span>    |
|<span data-ttu-id="b4cc9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4cc9-114">Application</span></span> | <span data-ttu-id="b4cc9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-115">Not supported.</span></span> |

<span data-ttu-id="b4cc9-116">**注:** ユーザー、グループ、および連絡先は、ディレクトリ オブジェクトの種類です。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="b4cc9-117">そのため、ユーザーを削除する必要がある場合は、次のアクセス許可を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="b4cc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4cc9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b4cc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4cc9-119">Request headers</span></span>
| <span data-ttu-id="b4cc9-120">名前</span><span class="sxs-lookup"><span data-stu-id="b4cc9-120">Name</span></span>       | <span data-ttu-id="b4cc9-121">型</span><span class="sxs-lookup"><span data-stu-id="b4cc9-121">Type</span></span> | <span data-ttu-id="b4cc9-122">説明</span><span class="sxs-lookup"><span data-stu-id="b4cc9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4cc9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4cc9-123">Authorization</span></span>  | <span data-ttu-id="b4cc9-124">string</span><span class="sxs-lookup"><span data-stu-id="b4cc9-124">string</span></span>  | <span data-ttu-id="b4cc9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4cc9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4cc9-127">Request body</span></span>
<span data-ttu-id="b4cc9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4cc9-129">応答</span><span class="sxs-lookup"><span data-stu-id="b4cc9-129">Response</span></span>

<span data-ttu-id="b4cc9-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4cc9-132">例</span><span class="sxs-lookup"><span data-stu-id="b4cc9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4cc9-133">要求</span><span class="sxs-lookup"><span data-stu-id="b4cc9-133">Request</span></span>
<span data-ttu-id="b4cc9-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="b4cc9-135">応答</span><span class="sxs-lookup"><span data-stu-id="b4cc9-135">Response</span></span>
<span data-ttu-id="b4cc9-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b4cc9-136">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
