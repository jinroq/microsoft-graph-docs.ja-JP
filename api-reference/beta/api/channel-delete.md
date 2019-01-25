---
title: チャネルを削除します。
description: チャネルを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 734df0a79881993f4e002562e5125305b624c4c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525333"
---
# <a name="delete-channel"></a><span data-ttu-id="1113f-103">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="1113f-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1113f-104">[チャネル](../resources/channel.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1113f-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="1113f-105">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="1113f-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="1113f-106">詳細についてはの[既知の問題点のリスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1113f-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="1113f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1113f-107">Permissions</span></span>
<span data-ttu-id="1113f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1113f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1113f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1113f-110">Permission type</span></span>      | <span data-ttu-id="1113f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1113f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1113f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1113f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1113f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1113f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1113f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1113f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1113f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1113f-115">Not supported.</span></span>    |
|<span data-ttu-id="1113f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1113f-116">Application</span></span> | <span data-ttu-id="1113f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1113f-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="1113f-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1113f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1113f-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1113f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1113f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1113f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1113f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1113f-121">Request headers</span></span>
| <span data-ttu-id="1113f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1113f-122">Header</span></span>       | <span data-ttu-id="1113f-123">値</span><span class="sxs-lookup"><span data-stu-id="1113f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1113f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1113f-124">Authorization</span></span>  | <span data-ttu-id="1113f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1113f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1113f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1113f-127">Request body</span></span>
<span data-ttu-id="1113f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1113f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1113f-129">応答</span><span class="sxs-lookup"><span data-stu-id="1113f-129">Response</span></span>

<span data-ttu-id="1113f-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1113f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1113f-132">例</span><span class="sxs-lookup"><span data-stu-id="1113f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1113f-133">要求</span><span class="sxs-lookup"><span data-stu-id="1113f-133">Request</span></span>
<span data-ttu-id="1113f-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1113f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="1113f-135">応答</span><span class="sxs-lookup"><span data-stu-id="1113f-135">Response</span></span>

<span data-ttu-id="1113f-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1113f-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
