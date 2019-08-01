---
title: チャネルからタブを削除する
description: 'チーム内の指定されたチャネルからタブを削除 (固定解除) します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3dbba4b8996a86e8ff71d0dd115b0a00362e103f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027210"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="c7605-103">チャネルからタブを削除する</span><span class="sxs-lookup"><span data-stu-id="c7605-103">Delete tab from channel</span></span>



<span data-ttu-id="c7605-104">[チーム](../resources/team.md)内の指定された[チャネル](../resources/channel.md)からタブを削除 (固定解除) します。</span><span class="sxs-lookup"><span data-stu-id="c7605-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c7605-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7605-105">Permissions</span></span>
<span data-ttu-id="c7605-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7605-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7605-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7605-108">Permission type</span></span>      | <span data-ttu-id="c7605-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7605-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7605-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7605-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7605-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7605-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7605-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7605-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7605-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7605-113">Not supported.</span></span>    |
|<span data-ttu-id="c7605-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7605-114">Application</span></span> | <span data-ttu-id="c7605-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7605-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="c7605-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c7605-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c7605-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c7605-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7605-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7605-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7605-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7605-119">Request headers</span></span>
| <span data-ttu-id="c7605-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7605-120">Header</span></span>       | <span data-ttu-id="c7605-121">値</span><span class="sxs-lookup"><span data-stu-id="c7605-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7605-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7605-122">Authorization</span></span>  | <span data-ttu-id="c7605-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c7605-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7605-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7605-125">Request body</span></span>
<span data-ttu-id="c7605-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c7605-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7605-127">応答</span><span class="sxs-lookup"><span data-stu-id="c7605-127">Response</span></span>

<span data-ttu-id="c7605-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c7605-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7605-130">例</span><span class="sxs-lookup"><span data-stu-id="c7605-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c7605-131">要求</span><span class="sxs-lookup"><span data-stu-id="c7605-131">Request</span></span>
<span data-ttu-id="c7605-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7605-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="c7605-133">応答</span><span class="sxs-lookup"><span data-stu-id="c7605-133">Response</span></span>
<span data-ttu-id="c7605-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7605-134">The following is an example of the response.</span></span> <span data-ttu-id="c7605-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c7605-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c7605-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c7605-136">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
