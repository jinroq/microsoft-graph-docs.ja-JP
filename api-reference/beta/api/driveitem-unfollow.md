---
author: chackman
ms.author: chackman
title: ドライブ項目のフォローを取り消します
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a42f740b3ea6f706529a5353e9cbb846bb7a4e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945952"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="bca05-102">ドライブ項目のフォローを取り消します</span><span class="sxs-lookup"><span data-stu-id="bca05-102">Unfollow drive item</span></span>

> <span data-ttu-id="bca05-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bca05-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bca05-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bca05-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bca05-105">[DriveItem](../resources/driveitem.md)のフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="bca05-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="bca05-106">**注:** 以下の項目には、[以下の項目](driveitem-follow.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bca05-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bca05-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bca05-107">Permissions</span></span>

<span data-ttu-id="bca05-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bca05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca05-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bca05-110">Permission type</span></span>      | <span data-ttu-id="bca05-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bca05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bca05-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bca05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bca05-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca05-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bca05-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bca05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bca05-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bca05-115">Not supported.</span></span>    |
|<span data-ttu-id="bca05-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bca05-116">Application</span></span> | <span data-ttu-id="bca05-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca05-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bca05-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bca05-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="bca05-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="bca05-119">Request body</span></span>

<span data-ttu-id="bca05-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="bca05-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="bca05-121">応答</span><span class="sxs-lookup"><span data-stu-id="bca05-121">Response</span></span>

<span data-ttu-id="bca05-122">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="bca05-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="bca05-123">例</span><span class="sxs-lookup"><span data-stu-id="bca05-123">Example</span></span>

<span data-ttu-id="bca05-124">次の使用例で識別される項目を unfollows `{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="bca05-124">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!-- {
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow"
} -->
