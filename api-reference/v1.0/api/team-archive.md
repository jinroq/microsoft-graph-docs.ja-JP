---
title: チームのアーカイブ
description: '指定されたチームをアーカイブします。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 5a364fe025688bf082de187940e40acdee22d6a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882853"
---
# <a name="archive-team"></a><span data-ttu-id="55465-103">チームのアーカイブ</span><span class="sxs-lookup"><span data-stu-id="55465-103">Archive team</span></span>



<span data-ttu-id="55465-104">指定された[チーム](../resources/team.md)をアーカイブします。</span><span class="sxs-lookup"><span data-stu-id="55465-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="55465-105">チームがアーカイブされると、ユーザーが不要になった送信、チーム内のすべてのチャネルのメッセージのようにチームの名前、説明、またはその他の設定を編集またはチームに一般にほとんどの変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="55465-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="55465-106">チームのメンバーシップの変更を続行できるようにします。</span><span class="sxs-lookup"><span data-stu-id="55465-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="55465-107">アーカイブは、非同期操作です。</span><span class="sxs-lookup"><span data-stu-id="55465-107">Archiving is an async operation.</span></span> <span data-ttu-id="55465-108">チームは、非同期操作が完了すると正常に、この API からの応答の後に発生する可能性がありますが、アーカイブされます。</span><span class="sxs-lookup"><span data-stu-id="55465-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="55465-109">チームをアーカイブするには、チームや[グループ](../resources/group.md)に所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="55465-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="55465-110">アーカイブ済みの状態からチームを復元するには、 [unarchive](team-unarchive.md)に API を使用します。</span><span class="sxs-lookup"><span data-stu-id="55465-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55465-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55465-111">Permissions</span></span>
<span data-ttu-id="55465-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55465-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55465-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55465-114">Permission type</span></span>      | <span data-ttu-id="55465-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55465-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55465-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55465-116">Delegated (work or school account)</span></span> | <span data-ttu-id="55465-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55465-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="55465-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55465-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55465-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55465-119">Not supported.</span></span>    |
|<span data-ttu-id="55465-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55465-120">Application</span></span> | <span data-ttu-id="55465-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55465-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="55465-122">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="55465-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="55465-123">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="55465-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="55465-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55465-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="55465-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55465-125">Request headers</span></span>
| <span data-ttu-id="55465-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55465-126">Header</span></span>       | <span data-ttu-id="55465-127">値</span><span class="sxs-lookup"><span data-stu-id="55465-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55465-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="55465-128">Authorization</span></span>  | <span data-ttu-id="55465-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55465-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55465-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="55465-131">Request body</span></span>
<span data-ttu-id="55465-132">要求にすることがあります _(オプション)_ が含まれます、 `shouldSetSpoSiteReadOnlyForMembers` 、JSON 内のパラメーターの本文、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="55465-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="55465-133">この省略可能なパラメーターでは、チーム メンバーのアクセス権をチームに関連付けられている Sharepoint Online サイトで読み取り専用に設定するかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="55465-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="55465-134">False に設定するか、本文を省略することに、この手順をスキップしてされます。</span><span class="sxs-lookup"><span data-stu-id="55465-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="55465-135">応答</span><span class="sxs-lookup"><span data-stu-id="55465-135">Response</span></span>

<span data-ttu-id="55465-136">かどうかアーカイブが正常に開始しました、このメソッドが返されます、`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="55465-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="55465-137">応答が含まれても、`Location`ヘッダーで、チームのアーカイブを処理するために作成された[teamsAsyncOperation](../resources/teamsasyncoperation.md)の場所が含まれています。</span><span class="sxs-lookup"><span data-stu-id="55465-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="55465-138">この場所に GET 要求を行うことによって、アーカイブ ・ オペレーションのステータスを確認します。</span><span class="sxs-lookup"><span data-stu-id="55465-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="55465-139">例</span><span class="sxs-lookup"><span data-stu-id="55465-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="55465-140">要求</span><span class="sxs-lookup"><span data-stu-id="55465-140">Request</span></span>
<span data-ttu-id="55465-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55465-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="55465-142">応答</span><span class="sxs-lookup"><span data-stu-id="55465-142">Response</span></span>
<span data-ttu-id="55465-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55465-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
