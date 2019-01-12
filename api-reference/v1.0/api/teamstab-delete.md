---
title: チャネルからタブを削除します。
description: '削除 (固定解除)、チーム内で指定されたチャネルのタブです。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 672077e4b1ac383ca6e6bb415ff25639fb03dc08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917434"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="764e7-103">チャネルからタブを削除します。</span><span class="sxs-lookup"><span data-stu-id="764e7-103">Delete tab from channel</span></span>



<span data-ttu-id="764e7-104">削除 (固定解除)[チーム](../resources/team.md)内で指定された[チャネル](../resources/channel.md)のタブです。</span><span class="sxs-lookup"><span data-stu-id="764e7-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="764e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="764e7-105">Permissions</span></span>
<span data-ttu-id="764e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="764e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="764e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="764e7-108">Permission type</span></span>      | <span data-ttu-id="764e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="764e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="764e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="764e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="764e7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="764e7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="764e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="764e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="764e7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="764e7-113">Not supported.</span></span>    |
|<span data-ttu-id="764e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="764e7-114">Application</span></span> | <span data-ttu-id="764e7-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="764e7-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="764e7-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="764e7-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="764e7-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="764e7-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="764e7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="764e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="764e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="764e7-119">Request headers</span></span>
| <span data-ttu-id="764e7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="764e7-120">Header</span></span>       | <span data-ttu-id="764e7-121">値</span><span class="sxs-lookup"><span data-stu-id="764e7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="764e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="764e7-122">Authorization</span></span>  | <span data-ttu-id="764e7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="764e7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="764e7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="764e7-125">Request body</span></span>
<span data-ttu-id="764e7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="764e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="764e7-127">応答</span><span class="sxs-lookup"><span data-stu-id="764e7-127">Response</span></span>

<span data-ttu-id="764e7-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="764e7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="764e7-130">例</span><span class="sxs-lookup"><span data-stu-id="764e7-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="764e7-131">要求</span><span class="sxs-lookup"><span data-stu-id="764e7-131">Request</span></span>
<span data-ttu-id="764e7-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="764e7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="764e7-133">応答</span><span class="sxs-lookup"><span data-stu-id="764e7-133">Response</span></span>
<span data-ttu-id="764e7-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="764e7-134">The following is an example of the response.</span></span> <span data-ttu-id="764e7-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="764e7-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="764e7-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="764e7-136">All of the properties will be returned from an actual call.</span></span>
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
