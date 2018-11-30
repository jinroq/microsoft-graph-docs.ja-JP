---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint サイトのサブサイトを一覧表示する
ms.openlocfilehash: 2f35e891afc3cbeaf0504c3dd8008bafb23ecd52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069648"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="cc1fb-102">サブサイトを列挙する</span><span class="sxs-lookup"><span data-stu-id="cc1fb-102">Enumerate subsites</span></span>

> <span data-ttu-id="cc1fb-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc1fb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc1fb-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc1fb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc1fb-105">[サイト][] に定義されているサブサイトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc1fb-105">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="cc1fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc1fb-107">Permissions</span></span>

<span data-ttu-id="cc1fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc1fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc1fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc1fb-110">Permission type</span></span>      | <span data-ttu-id="cc1fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc1fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc1fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc1fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc1fb-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc1fb-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc1fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc1fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc1fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc1fb-115">Not supported.</span></span>    |
|<span data-ttu-id="cc1fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc1fb-116">Application</span></span> | <span data-ttu-id="cc1fb-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc1fb-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc1fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc1fb-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="cc1fb-119">応答</span><span class="sxs-lookup"><span data-stu-id="cc1fb-119">Response</span></span>

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
