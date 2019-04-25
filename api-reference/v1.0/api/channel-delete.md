---
title: チャネルを削除する
description: チャネルを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 846aa0b00fc07a0a25e3eb3aae07bcccdbd936ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565598"
---
# <a name="delete-channel"></a><span data-ttu-id="71bd4-103">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="71bd4-103">Delete channel</span></span>



<span data-ttu-id="71bd4-104">[チャネル](../resources/channel.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="71bd4-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="71bd4-105">**注**: アプリケーションのアクセス許可とこの API には、既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="71bd4-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="71bd4-106">詳細については、[既知の問題リスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71bd4-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="71bd4-107">**注**: 削除されたチャネル内のデータは、チーム所有者が削除されたチャネルを回復できるように、数週間にわたって引き続き保存されます。</span><span class="sxs-lookup"><span data-stu-id="71bd4-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="71bd4-108">その間、同じ displayName で新しいチャネルを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="71bd4-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="71bd4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71bd4-109">Permissions</span></span>
<span data-ttu-id="71bd4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71bd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bd4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71bd4-112">Permission type</span></span>      | <span data-ttu-id="71bd4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71bd4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71bd4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71bd4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="71bd4-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bd4-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="71bd4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71bd4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bd4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71bd4-117">Not supported.</span></span>    |
|<span data-ttu-id="71bd4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71bd4-118">Application</span></span> | <span data-ttu-id="71bd4-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bd4-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="71bd4-120">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="71bd4-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="71bd4-121">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="71bd4-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="71bd4-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71bd4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="71bd4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71bd4-123">Request headers</span></span>
| <span data-ttu-id="71bd4-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71bd4-124">Header</span></span>       | <span data-ttu-id="71bd4-125">値</span><span class="sxs-lookup"><span data-stu-id="71bd4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71bd4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bd4-126">Authorization</span></span>  | <span data-ttu-id="71bd4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71bd4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71bd4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="71bd4-129">Request body</span></span>
<span data-ttu-id="71bd4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71bd4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71bd4-131">応答</span><span class="sxs-lookup"><span data-stu-id="71bd4-131">Response</span></span>

<span data-ttu-id="71bd4-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="71bd4-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71bd4-134">例</span><span class="sxs-lookup"><span data-stu-id="71bd4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71bd4-135">要求</span><span class="sxs-lookup"><span data-stu-id="71bd4-135">Request</span></span>
<span data-ttu-id="71bd4-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71bd4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="71bd4-137">応答</span><span class="sxs-lookup"><span data-stu-id="71bd4-137">Response</span></span>

<span data-ttu-id="71bd4-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71bd4-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
