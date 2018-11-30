---
author: chackman
ms.author: chackman
title: ドライブ項目のフォローを取り消します
ms.openlocfilehash: 871ea9782e62e66adeed743819a265b452e06de3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066683"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="4e26b-102">ドライブ項目のフォローを取り消します</span><span class="sxs-lookup"><span data-stu-id="4e26b-102">Unfollow drive item</span></span>

> <span data-ttu-id="4e26b-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e26b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e26b-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e26b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e26b-105">[DriveItem](../resources/driveitem.md)のフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="4e26b-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="4e26b-106">**注:** 以下の項目には、[以下の項目](driveitem-follow.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e26b-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e26b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e26b-107">Permissions</span></span>

<span data-ttu-id="4e26b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e26b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e26b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e26b-110">Permission type</span></span>      | <span data-ttu-id="4e26b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e26b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e26b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e26b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e26b-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e26b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e26b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e26b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e26b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e26b-115">Not supported.</span></span>    |
|<span data-ttu-id="4e26b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e26b-116">Application</span></span> | <span data-ttu-id="4e26b-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e26b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e26b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e26b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="4e26b-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e26b-119">Request body</span></span>

<span data-ttu-id="4e26b-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="4e26b-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="4e26b-121">応答</span><span class="sxs-lookup"><span data-stu-id="4e26b-121">Response</span></span>

<span data-ttu-id="4e26b-122">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="4e26b-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="4e26b-123">使用例</span><span class="sxs-lookup"><span data-stu-id="4e26b-123">Example</span></span>

<span data-ttu-id="4e26b-124">次の使用例で識別される項目を unfollows `{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="4e26b-124">This example unfollows an item identified by `{item-id}`.</span></span>

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
