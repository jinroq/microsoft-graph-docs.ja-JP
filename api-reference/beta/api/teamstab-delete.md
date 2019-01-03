---
title: チャネルからタブを削除します。
description: '削除 (固定解除)、チーム内で指定されたチャネルのタブです。 '
author: nkramer
ms.openlocfilehash: 7d8465f650d63f22625c1da2c56b3de4e065374b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349288"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="214e4-103">チャネルからタブを削除します。</span><span class="sxs-lookup"><span data-stu-id="214e4-103">Delete tab from channel</span></span>

> <span data-ttu-id="214e4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="214e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="214e4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="214e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="214e4-106">削除 (固定解除)[チーム](../resources/team.md)内で指定された[チャネル](../resources/channel.md)のタブです。</span><span class="sxs-lookup"><span data-stu-id="214e4-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="214e4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="214e4-107">Permissions</span></span>
<span data-ttu-id="214e4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="214e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214e4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="214e4-110">Permission type</span></span>      | <span data-ttu-id="214e4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="214e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214e4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="214e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="214e4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="214e4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="214e4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="214e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="214e4-115">Not supported.</span></span>    |
|<span data-ttu-id="214e4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="214e4-116">Application</span></span> | <span data-ttu-id="214e4-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="214e4-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="214e4-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="214e4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="214e4-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="214e4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="214e4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="214e4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="214e4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="214e4-121">Request headers</span></span>
| <span data-ttu-id="214e4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="214e4-122">Header</span></span>       | <span data-ttu-id="214e4-123">値</span><span class="sxs-lookup"><span data-stu-id="214e4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="214e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="214e4-124">Authorization</span></span>  | <span data-ttu-id="214e4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="214e4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="214e4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="214e4-127">Request body</span></span>
<span data-ttu-id="214e4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="214e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214e4-129">応答</span><span class="sxs-lookup"><span data-stu-id="214e4-129">Response</span></span>

<span data-ttu-id="214e4-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="214e4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="214e4-132">例</span><span class="sxs-lookup"><span data-stu-id="214e4-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="214e4-133">要求</span><span class="sxs-lookup"><span data-stu-id="214e4-133">Request</span></span>
<span data-ttu-id="214e4-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="214e4-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="214e4-135">応答</span><span class="sxs-lookup"><span data-stu-id="214e4-135">Response</span></span>
<span data-ttu-id="214e4-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="214e4-136">The following is an example of the response.</span></span> <span data-ttu-id="214e4-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="214e4-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="214e4-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="214e4-138">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->