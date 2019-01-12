---
title: チームのクローンを作成します。
description: チームのコピーを作成します。 この操作では、対応するグループのコピーも作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4fb3769db0df6d2fc30d995098daee19b49e83b7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958342"
---
# <a name="clone-a-team"></a><span data-ttu-id="13da0-104">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="13da0-104">Clone a team</span></span>

> <span data-ttu-id="13da0-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13da0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13da0-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13da0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13da0-107">[チーム](../resources/team.md)のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="13da0-107">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="13da0-108">この操作では、対応する[グループ](../resources/group.md)のコピーも作成します。</span><span class="sxs-lookup"><span data-stu-id="13da0-108">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="13da0-109">クローンを作成するチームのどの部分を指定できます。</span><span class="sxs-lookup"><span data-stu-id="13da0-109">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="13da0-110">**アプリケーション**・ チームにインストールされているアプリケーションをマイクロソフト チームのコピーです。</span><span class="sxs-lookup"><span data-stu-id="13da0-110">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="13da0-111">**チャネル**は、チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。</span><span class="sxs-lookup"><span data-stu-id="13da0-111">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="13da0-112">**メンバー** -メンバーをコピーし、グループの所有者です。</span><span class="sxs-lookup"><span data-stu-id="13da0-112">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="13da0-113">**設定**– は、キーのグループの設定と、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="13da0-113">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="13da0-114">**タブ**– は、チャネル内のタブにコピーします。</span><span class="sxs-lookup"><span data-stu-id="13da0-114">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="13da0-115">タブがクローン化されると、未構成の状態に移動する:、マイクロソフト チームのタブ バーに表示され、構成] 画面で移動します] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="13da0-115">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="13da0-116">(タブを開いた人がアプリケーションを構成するのにはアクセス許可を持たない場合が表示されるタブが構成されていないことを説明するメッセージです。)</span><span class="sxs-lookup"><span data-stu-id="13da0-116">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="13da0-117">クローン作成は、時間のかかる操作です。</span><span class="sxs-lookup"><span data-stu-id="13da0-117">Cloning is a long-running operation.</span></span>
<span data-ttu-id="13da0-118">投稿クローンが返されるは、「実行中」または「成功」または「失敗」を表示する[操作](../resources/teamsasyncoperation.md)を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="13da0-118">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="13da0-119">ステータスが「動作していない」まで取得を続行してください。</span><span class="sxs-lookup"><span data-stu-id="13da0-119">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="13da0-120">取得の推奨される間隔は、5 秒間です。</span><span class="sxs-lookup"><span data-stu-id="13da0-120">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="13da0-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13da0-121">Permissions</span></span>

<span data-ttu-id="13da0-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13da0-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13da0-124">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13da0-124">Permission type</span></span>      | <span data-ttu-id="13da0-125">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13da0-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13da0-126">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13da0-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="13da0-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13da0-127">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="13da0-128">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13da0-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13da0-129">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13da0-129">Not supported.</span></span>    |
|<span data-ttu-id="13da0-130">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13da0-130">Application</span></span>                            | <span data-ttu-id="13da0-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13da0-131">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13da0-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13da0-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="13da0-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13da0-133">Request headers</span></span>
| <span data-ttu-id="13da0-134">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13da0-134">Header</span></span>       | <span data-ttu-id="13da0-135">値</span><span class="sxs-lookup"><span data-stu-id="13da0-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13da0-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="13da0-136">Authorization</span></span>  | <span data-ttu-id="13da0-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13da0-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="13da0-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13da0-139">Content-Type</span></span>  | <span data-ttu-id="13da0-140">application/json</span><span class="sxs-lookup"><span data-stu-id="13da0-140">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13da0-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="13da0-141">Request body</span></span>

| <span data-ttu-id="13da0-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13da0-142">Property</span></span>     | <span data-ttu-id="13da0-143">種類</span><span class="sxs-lookup"><span data-stu-id="13da0-143">Type</span></span>   |<span data-ttu-id="13da0-144">説明</span><span class="sxs-lookup"><span data-stu-id="13da0-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13da0-145">分類</span><span class="sxs-lookup"><span data-stu-id="13da0-145">classification</span></span>|<span data-ttu-id="13da0-146">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="13da0-146">String (optional)</span></span>|<span data-ttu-id="13da0-147">(低、中、または高のビジネス ・ インパクト) などのグループの分類について説明します。</span><span class="sxs-lookup"><span data-stu-id="13da0-147">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="13da0-148">このプロパティの有効値は、[テンプレートの定義](../resources/directorysettingtemplate.md)に基づいて、ClassificationList の[設定](../resources/directorysetting.md)値を作成することによって定義されます。</span><span class="sxs-lookup"><span data-stu-id="13da0-148">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="13da0-149">分類を指定しない場合、分類は、元のチームまたはグループからコピーされます。</span><span class="sxs-lookup"><span data-stu-id="13da0-149">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="13da0-150">description</span><span class="sxs-lookup"><span data-stu-id="13da0-150">description</span></span>|<span data-ttu-id="13da0-151">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="13da0-151">String (optional)</span></span>|<span data-ttu-id="13da0-152">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="13da0-152">An optional description for the group.</span></span> <span data-ttu-id="13da0-153">このプロパティを指定しない場合、空白のままにします。</span><span class="sxs-lookup"><span data-stu-id="13da0-153">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="13da0-154">displayName</span><span class="sxs-lookup"><span data-stu-id="13da0-154">displayName</span></span>|<span data-ttu-id="13da0-155">String</span><span class="sxs-lookup"><span data-stu-id="13da0-155">String</span></span>|<span data-ttu-id="13da0-p110">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="13da0-p110">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="13da0-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="13da0-159">mailNickname</span></span>|<span data-ttu-id="13da0-160">String</span><span class="sxs-lookup"><span data-stu-id="13da0-160">String</span></span>|<span data-ttu-id="13da0-161">グループ、組織内で一意の電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="13da0-161">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="13da0-162">グループが作成されるとき、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="13da0-162">This property must be specified when a group is created.</span></span> <span data-ttu-id="13da0-163">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="13da0-163">Supports $filter.</span></span> <span data-ttu-id="13da0-164">このプロパティが指定されていない場合に、表示名から計算されます。</span><span class="sxs-lookup"><span data-stu-id="13da0-164">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="13da0-165">既知の問題: 現在、このプロパティは無視されます。</span><span class="sxs-lookup"><span data-stu-id="13da0-165">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="13da0-166">partsToClone</span><span class="sxs-lookup"><span data-stu-id="13da0-166">partsToClone</span></span>| [<span data-ttu-id="13da0-167">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="13da0-167">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="13da0-168">クローンを作成する部品のコンマで区切られたリスト。</span><span class="sxs-lookup"><span data-stu-id="13da0-168">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="13da0-169">法的な部分は、「アプリケーション、タブ、設定、チャネル、メンバー"です。</span><span class="sxs-lookup"><span data-stu-id="13da0-169">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="13da0-170">visibility</span><span class="sxs-lookup"><span data-stu-id="13da0-170">visibility</span></span>|<span data-ttu-id="13da0-171">[teamVisibilityType](../resources/teamvisibilitytype.md)(省略可能)</span><span class="sxs-lookup"><span data-stu-id="13da0-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="13da0-172">グループの可視性を指定します。</span><span class="sxs-lookup"><span data-stu-id="13da0-172">Specifies the visibility of the group.</span></span> <span data-ttu-id="13da0-173">使用可能な値:**パブリック**、**プライベート**です。</span><span class="sxs-lookup"><span data-stu-id="13da0-173">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="13da0-174">可視性が指定されていない場合、元のチームまたはグループの表示と非表示がコピーされます。</span><span class="sxs-lookup"><span data-stu-id="13da0-174">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="13da0-175">**EducationClass**チームは、チームのクローンが作成されている場合、可視性パラメーターは無視されます、および新しいグループの表示/非表示を HiddenMembership に設定されます。</span><span class="sxs-lookup"><span data-stu-id="13da0-175">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="13da0-176">応答</span><span class="sxs-lookup"><span data-stu-id="13da0-176">Response</span></span>

<span data-ttu-id="13da0-177">かどうかは成功すると、このメソッドは、`202 Accepted`の場所で応答コード: ヘッダーの[処理](../resources/teamsasyncoperation.md)リソースを指します。</span><span class="sxs-lookup"><span data-stu-id="13da0-177">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="13da0-178">操作が完了すると、処理リソースが送信されます作成したチームの id。</span><span class="sxs-lookup"><span data-stu-id="13da0-178">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="13da0-179">例</span><span class="sxs-lookup"><span data-stu-id="13da0-179">Example</span></span>
#### <a name="request"></a><span data-ttu-id="13da0-180">要求</span><span class="sxs-lookup"><span data-stu-id="13da0-180">Request</span></span>
<span data-ttu-id="13da0-181">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13da0-181">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a><span data-ttu-id="13da0-182">応答</span><span class="sxs-lookup"><span data-stu-id="13da0-182">Response</span></span>
<span data-ttu-id="13da0-183">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13da0-183">The following is an example of the response.</span></span> <span data-ttu-id="13da0-184">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="13da0-184">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13da0-185">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13da0-185">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
