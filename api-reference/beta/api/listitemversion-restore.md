---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 旧バージョンの SharePoint リスト アイテムを復元する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ede28ecb2ee743748af7ab70cc64e0ae8ec38528
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338722"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="0cf00-102">旧バージョンのリスト アイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="0cf00-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cf00-103">旧バージョンのリスト アイテムを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="0cf00-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="0cf00-104">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、アイテムの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="0cf00-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf00-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0cf00-105">Permissions</span></span>

<span data-ttu-id="0cf00-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cf00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="0cf00-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cf00-108">Permission type</span></span>             |         <span data-ttu-id="0cf00-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cf00-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="0cf00-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cf00-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cf00-111">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0cf00-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="0cf00-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cf00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cf00-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="0cf00-113">n/a</span></span>                                                          |
| <span data-ttu-id="0cf00-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cf00-114">Application</span></span>                            | <span data-ttu-id="0cf00-115">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0cf00-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cf00-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cf00-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="0cf00-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cf00-117">Request body</span></span>

<span data-ttu-id="0cf00-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="0cf00-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="0cf00-119">例</span><span class="sxs-lookup"><span data-stu-id="0cf00-119">Example</span></span>

<span data-ttu-id="0cf00-120">この例では、`{item-id}` と `{version-id}` で識別されるリスト アイテムのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="0cf00-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="0cf00-121">応答</span><span class="sxs-lookup"><span data-stu-id="0cf00-121">Response</span></span>

<span data-ttu-id="0cf00-122">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="0cf00-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
