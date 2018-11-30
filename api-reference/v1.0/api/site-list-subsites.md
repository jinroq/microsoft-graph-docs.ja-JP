---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint サイトのサブサイトを一覧表示する
ms.openlocfilehash: a26c2f592c11760b822c80a7e37749823a5172aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021300"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="2dcbb-102">サブサイトを列挙する</span><span class="sxs-lookup"><span data-stu-id="2dcbb-102">Enumerate subsites</span></span>

<span data-ttu-id="2dcbb-103">[サイト][] に定義されているサブサイトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2dcbb-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2dcbb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2dcbb-105">Permissions</span></span>

<span data-ttu-id="2dcbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dcbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dcbb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2dcbb-108">Permission type</span></span>      | <span data-ttu-id="2dcbb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2dcbb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dcbb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2dcbb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2dcbb-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dcbb-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dcbb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2dcbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dcbb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dcbb-113">Not supported.</span></span>    |
|<span data-ttu-id="2dcbb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2dcbb-114">Application</span></span> | <span data-ttu-id="2dcbb-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dcbb-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dcbb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2dcbb-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="2dcbb-117">応答</span><span class="sxs-lookup"><span data-stu-id="2dcbb-117">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
