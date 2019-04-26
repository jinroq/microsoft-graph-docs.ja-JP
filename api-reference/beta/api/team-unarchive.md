---
title: チームを展開する
description: アーカイブされたチームを復元します。 これにより、ユーザーがメッセージを送信したり、チームを編集したりできるようになります。テナントとチームの設定によって abiding ます。 Teams は、アーカイブ API を使用してアーカイブされます。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3af0f2b0434e1883a95210eaf46129921fd176cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335229"
---
# <a name="unarchive-team"></a><span data-ttu-id="c8b9a-105">チームを展開する</span><span class="sxs-lookup"><span data-stu-id="c8b9a-105">Unarchive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8b9a-106">アーカイブされた[チーム](../resources/team.md)を復元します。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="c8b9a-107">これにより、ユーザーがメッセージを送信したり、チームを編集したりできるようになります。テナントとチームの設定によって abiding ます。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="c8b9a-108">Teams は、[アーカイブ](team-archive.md)API を使用してアーカイブされます。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="c8b9a-109">アーカイブの取り消しは、非同期操作です。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="c8b9a-110">非同期操作が正常に完了すると、この API からの応答によって発生する可能性があるチームが unarchived れます。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8b9a-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8b9a-111">Permissions</span></span>
<span data-ttu-id="c8b9a-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8b9a-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8b9a-114">Permission type</span></span>      | <span data-ttu-id="c8b9a-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8b9a-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c8b9a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8b9a-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c8b9a-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8b9a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-119">Not supported.</span></span>    |
|<span data-ttu-id="c8b9a-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8b9a-120">Application</span></span> | <span data-ttu-id="c8b9a-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8b9a-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c8b9a-122">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c8b9a-123">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c8b9a-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8b9a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="c8b9a-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8b9a-125">Request headers</span></span>
| <span data-ttu-id="c8b9a-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8b9a-126">Header</span></span>       | <span data-ttu-id="c8b9a-127">値</span><span class="sxs-lookup"><span data-stu-id="c8b9a-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8b9a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8b9a-128">Authorization</span></span>  | <span data-ttu-id="c8b9a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8b9a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8b9a-131">Request body</span></span>
<span data-ttu-id="c8b9a-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8b9a-133">応答</span><span class="sxs-lookup"><span data-stu-id="c8b9a-133">Response</span></span>

<span data-ttu-id="c8b9a-134">アーカイブが正常に開始されなかった場合、 `202 Accepted`このメソッドは応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c8b9a-135">応答には、チームの`Location`アーカイブを処理するために作成された[teamsAsyncOperation](../resources/teamsasyncoperation.md)の場所を含むヘッダーも含まれます。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="c8b9a-136">この場所に GET 要求を行うことによって、未アーカイブ操作の状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="c8b9a-137">例</span><span class="sxs-lookup"><span data-stu-id="c8b9a-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c8b9a-138">要求</span><span class="sxs-lookup"><span data-stu-id="c8b9a-138">Request</span></span>
<span data-ttu-id="c8b9a-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="c8b9a-140">応答</span><span class="sxs-lookup"><span data-stu-id="c8b9a-140">Response</span></span>
<span data-ttu-id="c8b9a-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8b9a-141">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
