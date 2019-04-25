---
title: チャネルからタブを削除する
description: 'チーム内の指定されたチャネルからタブを削除 (固定解除) します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a5cb2334c250c63d0644c8fab3f97d35c481a515
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521777"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="48090-103">チャネルからタブを削除する</span><span class="sxs-lookup"><span data-stu-id="48090-103">Delete tab from channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48090-104">[チーム](../resources/team.md)内の指定された[チャネル](../resources/channel.md)からタブを削除 (固定解除) します。</span><span class="sxs-lookup"><span data-stu-id="48090-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="48090-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48090-105">Permissions</span></span>
<span data-ttu-id="48090-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48090-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48090-108">Permission type</span></span>      | <span data-ttu-id="48090-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48090-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48090-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48090-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48090-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48090-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48090-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48090-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48090-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48090-113">Not supported.</span></span>    |
|<span data-ttu-id="48090-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48090-114">Application</span></span> | <span data-ttu-id="48090-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48090-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="48090-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="48090-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="48090-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="48090-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="48090-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48090-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="48090-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48090-119">Request headers</span></span>
| <span data-ttu-id="48090-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48090-120">Header</span></span>       | <span data-ttu-id="48090-121">値</span><span class="sxs-lookup"><span data-stu-id="48090-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48090-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48090-122">Authorization</span></span>  | <span data-ttu-id="48090-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48090-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48090-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="48090-125">Request body</span></span>
<span data-ttu-id="48090-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="48090-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48090-127">応答</span><span class="sxs-lookup"><span data-stu-id="48090-127">Response</span></span>

<span data-ttu-id="48090-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="48090-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48090-130">例</span><span class="sxs-lookup"><span data-stu-id="48090-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="48090-131">要求</span><span class="sxs-lookup"><span data-stu-id="48090-131">Request</span></span>
<span data-ttu-id="48090-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48090-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="48090-133">応答</span><span class="sxs-lookup"><span data-stu-id="48090-133">Response</span></span>
<span data-ttu-id="48090-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48090-134">The following is an example of the response.</span></span> <span data-ttu-id="48090-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="48090-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="48090-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="48090-136">All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
