---
author: JeremyKelley
description: サイト に定義されているサブサイトのコレクションを取得します。
ms.date: 09/10/2017
title: SharePoint サイトのサブサイトを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0a0a3d9b932778734e64a01f2f3370ac7435aa3c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363747"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="35625-103">サブサイトを列挙する</span><span class="sxs-lookup"><span data-stu-id="35625-103">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35625-104">[サイト][] に定義されているサブサイトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="35625-104">Get a collection of subsites defined for a [site][].</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="35625-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35625-106">Permissions</span></span>

<span data-ttu-id="35625-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35625-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35625-109">Permission type</span></span>      | <span data-ttu-id="35625-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35625-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35625-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35625-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35625-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35625-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="35625-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35625-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35625-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35625-114">Not supported.</span></span>    |
|<span data-ttu-id="35625-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35625-115">Application</span></span> | <span data-ttu-id="35625-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35625-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35625-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35625-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="35625-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="35625-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35625-119">C#</span><span class="sxs-lookup"><span data-stu-id="35625-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35625-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35625-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35625-121">目的-C</span><span class="sxs-lookup"><span data-stu-id="35625-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35625-122">Java</span><span class="sxs-lookup"><span data-stu-id="35625-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="35625-123">応答</span><span class="sxs-lookup"><span data-stu-id="35625-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
}
-->
