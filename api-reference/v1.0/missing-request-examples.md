---
title: (me) をシングルトンとして定義します。
description: 値下げ-スキャナーを確認するのにはドキュメントに追加する必要があることは、します。
ms.openlocfilehash: 76e8cc2ed8cb481d732e1b0727107eee8d520e77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021348"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="11b54-103">ヘルパー (ドキュメントに含まれていない例)</span><span class="sxs-lookup"><span data-stu-id="11b54-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="11b54-104">これらはマークダウン スキャナーがグラフ ドキュメントを適切に処理できるようにするため、ドキュメントに追加する必要があったものです。</span><span class="sxs-lookup"><span data-stu-id="11b54-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="11b54-105">(me) をシングルトンとして定義します。</span><span class="sxs-lookup"><span data-stu-id="11b54-105">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="11b54-106">ドライブをクエリ可能な entityset として定義します。</span><span class="sxs-lookup"><span data-stu-id="11b54-106">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="11b54-107">ユーザーをクエリ可能な entityset として定義します。</span><span class="sxs-lookup"><span data-stu-id="11b54-107">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
