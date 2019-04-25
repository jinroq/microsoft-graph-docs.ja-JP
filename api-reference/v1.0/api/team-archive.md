---
title: チームをアーカイブする
description: '指定されたチームをアーカイブします。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 28c1ea9d96d55587f95af85c9aba50a43fe08d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520250"
---
# <a name="archive-team"></a><span data-ttu-id="96874-103">チームをアーカイブする</span><span class="sxs-lookup"><span data-stu-id="96874-103">Archive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96874-104">指定された[チーム](../resources/team.md)をアーカイブします。</span><span class="sxs-lookup"><span data-stu-id="96874-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="96874-105">チームをアーカイブすると、ユーザーはチームのチャネルでメッセージを送信したり、いいねしたり、チームの名前、説明、またはその他の設定、通常、チームへの変更がほとんどできなくなります。</span><span class="sxs-lookup"><span data-stu-id="96874-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="96874-106">チームへのメンバーシップの変更はそのまま許可されます。</span><span class="sxs-lookup"><span data-stu-id="96874-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="96874-107">アーカイブは非同期操作です。</span><span class="sxs-lookup"><span data-stu-id="96874-107">Archiving is an async operation.</span></span> <span data-ttu-id="96874-108">非同期操作が正常に完了すると、チームがアーカイブされます。この API の応答に続いて発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="96874-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="96874-109">チームをアーカイブできるのは、チームと[グループ](../resources/group.md)が所有者の場合です。</span><span class="sxs-lookup"><span data-stu-id="96874-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="96874-110">アーカイブした状態からチームを復元するには、API を使用して[アーカイブを解除](team-unarchive.md)します。</span><span class="sxs-lookup"><span data-stu-id="96874-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96874-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96874-111">Permissions</span></span>
<span data-ttu-id="96874-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96874-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96874-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96874-114">Permission type</span></span>      | <span data-ttu-id="96874-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96874-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96874-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96874-116">Delegated (work or school account)</span></span> | <span data-ttu-id="96874-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96874-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96874-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96874-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96874-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96874-119">Not supported.</span></span>    |
|<span data-ttu-id="96874-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96874-120">Application</span></span> | <span data-ttu-id="96874-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96874-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="96874-122">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="96874-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="96874-123">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="96874-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="96874-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96874-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="96874-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96874-125">Request headers</span></span>
| <span data-ttu-id="96874-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96874-126">Header</span></span>       | <span data-ttu-id="96874-127">値</span><span class="sxs-lookup"><span data-stu-id="96874-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96874-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="96874-128">Authorization</span></span>  | <span data-ttu-id="96874-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96874-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96874-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="96874-131">Request body</span></span>
<span data-ttu-id="96874-132">次のように、リクエストでは_オプションで_ JSON の本文に`shouldSetSpoSiteReadOnlyForMembers`パラメーターを入力できます。</span><span class="sxs-lookup"><span data-stu-id="96874-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="96874-133">このオプションのパラメーターは、チーム メンバーのアクセス許可を、チームに関連付けられている Sharepoint Online サイトで読み取り専用に設定するかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="96874-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="96874-134">False に設定したり、本文を完全に省略したりすると、この手順がスキップされます。</span><span class="sxs-lookup"><span data-stu-id="96874-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="96874-135">応答</span><span class="sxs-lookup"><span data-stu-id="96874-135">Response</span></span>

<span data-ttu-id="96874-136">アーカイブが正常に開始された場合、このメソッドは`202 Accepted`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="96874-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="96874-137">応答には、チームのアーカイブを処理するのに作成された [teamsAsyncOperation](../resources/teamsasyncoperation.md) の場所を含む`Location`ヘッダーも含まれます。</span><span class="sxs-lookup"><span data-stu-id="96874-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="96874-138">この場所に GET 要求を作成して、アーカイブ操作の状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="96874-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="96874-139">例</span><span class="sxs-lookup"><span data-stu-id="96874-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96874-140">要求</span><span class="sxs-lookup"><span data-stu-id="96874-140">Request</span></span>
<span data-ttu-id="96874-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96874-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="96874-142">応答</span><span class="sxs-lookup"><span data-stu-id="96874-142">Response</span></span>
<span data-ttu-id="96874-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96874-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
