---
title: チームのクローンを作成します。
description: チームのコピーを作成します。 この操作では、対応するグループのコピーも作成します。
author: nkramer
ms.openlocfilehash: 21671ccbe440a57f6d745f9587c09b4432e25c35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321834"
---
# <a name="clone-a-team"></a><span data-ttu-id="672eb-104">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="672eb-104">Clone a team</span></span>



<span data-ttu-id="672eb-105">[チーム](../resources/team.md)のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="672eb-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="672eb-106">この操作では、対応する[グループ](../resources/group.md)のコピーも作成します。</span><span class="sxs-lookup"><span data-stu-id="672eb-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="672eb-107">クローンを作成するチームのどの部分を指定できます。</span><span class="sxs-lookup"><span data-stu-id="672eb-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="672eb-108">**アプリケーション**・ チームにインストールされているアプリケーションをマイクロソフト チームのコピーです。</span><span class="sxs-lookup"><span data-stu-id="672eb-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="672eb-109">**チャネル**は、チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。</span><span class="sxs-lookup"><span data-stu-id="672eb-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="672eb-110">**メンバー** -メンバーをコピーし、グループの所有者です。</span><span class="sxs-lookup"><span data-stu-id="672eb-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="672eb-111">**設定**– は、キーのグループの設定と、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="672eb-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="672eb-112">**タブ**– は、チャネル内のタブにコピーします。</span><span class="sxs-lookup"><span data-stu-id="672eb-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="672eb-113">タブがクローン化されると、未構成の状態に移動する:、マイクロソフト チームのタブ バーに表示され、構成] 画面で移動します] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="672eb-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="672eb-114">(タブを開いた人がアプリケーションを構成するのにはアクセス許可を持たない場合が表示されるタブが構成されていないことを説明するメッセージです。)</span><span class="sxs-lookup"><span data-stu-id="672eb-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="672eb-115">クローン作成は、時間のかかる操作です。</span><span class="sxs-lookup"><span data-stu-id="672eb-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="672eb-116">投稿クローンが返されるは、「実行中」または「成功」または「失敗」を表示する[操作](../resources/teamsasyncoperation.md)を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="672eb-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="672eb-117">ステータスが「動作していない」まで取得を続行してください。</span><span class="sxs-lookup"><span data-stu-id="672eb-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="672eb-118">取得の推奨される間隔は、5 秒間です。</span><span class="sxs-lookup"><span data-stu-id="672eb-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="672eb-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="672eb-119">Permissions</span></span>

<span data-ttu-id="672eb-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="672eb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672eb-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="672eb-122">Permission type</span></span>      | <span data-ttu-id="672eb-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="672eb-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="672eb-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="672eb-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="672eb-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672eb-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="672eb-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="672eb-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="672eb-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="672eb-127">Not supported.</span></span>    |
|<span data-ttu-id="672eb-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="672eb-128">Application</span></span>                            | <span data-ttu-id="672eb-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672eb-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="672eb-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="672eb-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="672eb-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="672eb-131">Request headers</span></span>
| <span data-ttu-id="672eb-132">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="672eb-132">Header</span></span>       | <span data-ttu-id="672eb-133">値</span><span class="sxs-lookup"><span data-stu-id="672eb-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="672eb-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="672eb-134">Authorization</span></span>  | <span data-ttu-id="672eb-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="672eb-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="672eb-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="672eb-137">Content-Type</span></span>  | <span data-ttu-id="672eb-138">application/json</span><span class="sxs-lookup"><span data-stu-id="672eb-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="672eb-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="672eb-139">Request body</span></span>

| <span data-ttu-id="672eb-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="672eb-140">Property</span></span>     | <span data-ttu-id="672eb-141">種類</span><span class="sxs-lookup"><span data-stu-id="672eb-141">Type</span></span>   |<span data-ttu-id="672eb-142">説明</span><span class="sxs-lookup"><span data-stu-id="672eb-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="672eb-143">分類</span><span class="sxs-lookup"><span data-stu-id="672eb-143">classification</span></span>|<span data-ttu-id="672eb-144">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="672eb-144">String (optional)</span></span>|<span data-ttu-id="672eb-145">(低、中、または高のビジネス ・ インパクト) などのグループの分類について説明します。</span><span class="sxs-lookup"><span data-stu-id="672eb-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="672eb-146">分類を指定しない場合、分類は、元のチームまたはグループからコピーされます。</span><span class="sxs-lookup"><span data-stu-id="672eb-146">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="672eb-147">description</span><span class="sxs-lookup"><span data-stu-id="672eb-147">description</span></span>|<span data-ttu-id="672eb-148">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="672eb-148">String (optional)</span></span>|<span data-ttu-id="672eb-149">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="672eb-149">An optional description for the group.</span></span> <span data-ttu-id="672eb-150">このプロパティを指定しない場合、空白のままにします。</span><span class="sxs-lookup"><span data-stu-id="672eb-150">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="672eb-151">displayName</span><span class="sxs-lookup"><span data-stu-id="672eb-151">displayName</span></span>|<span data-ttu-id="672eb-152">String</span><span class="sxs-lookup"><span data-stu-id="672eb-152">String</span></span>|<span data-ttu-id="672eb-p109">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="672eb-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="672eb-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="672eb-156">mailNickname</span></span>|<span data-ttu-id="672eb-157">String</span><span class="sxs-lookup"><span data-stu-id="672eb-157">String</span></span>|<span data-ttu-id="672eb-158">グループ、組織内で一意の電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="672eb-158">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="672eb-159">グループが作成されるとき、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="672eb-159">This property must be specified when a group is created.</span></span> <span data-ttu-id="672eb-160">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="672eb-160">Supports $filter.</span></span> <span data-ttu-id="672eb-161">このプロパティが指定されていない場合に、表示名から計算されます。</span><span class="sxs-lookup"><span data-stu-id="672eb-161">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="672eb-162">既知の問題: 現在、このプロパティは無視されます。</span><span class="sxs-lookup"><span data-stu-id="672eb-162">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="672eb-163">partsToClone</span><span class="sxs-lookup"><span data-stu-id="672eb-163">partsToClone</span></span>| [<span data-ttu-id="672eb-164">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="672eb-164">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="672eb-165">クローンを作成する部品のコンマで区切られたリスト。</span><span class="sxs-lookup"><span data-stu-id="672eb-165">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="672eb-166">法的な部分は、「アプリケーション、タブ、設定、チャネル、メンバー"です。</span><span class="sxs-lookup"><span data-stu-id="672eb-166">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="672eb-167">visibility</span><span class="sxs-lookup"><span data-stu-id="672eb-167">visibility</span></span>|<span data-ttu-id="672eb-168">[teamVisibilityType](../resources/teamvisibilitytype.md)(省略可能)</span><span class="sxs-lookup"><span data-stu-id="672eb-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="672eb-169">グループの可視性を指定します。</span><span class="sxs-lookup"><span data-stu-id="672eb-169">Specifies the visibility of the group.</span></span> <span data-ttu-id="672eb-170">使用可能な値:**パブリック**、**プライベート**です。</span><span class="sxs-lookup"><span data-stu-id="672eb-170">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="672eb-171">可視性が指定されていない場合、元のチームまたはグループの表示と非表示がコピーされます。</span><span class="sxs-lookup"><span data-stu-id="672eb-171">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="672eb-172">**EducationClass**チームは、チームのクローンが作成されている場合、可視性パラメーターは無視されます、および新しいグループの表示/非表示を HiddenMembership に設定されます。</span><span class="sxs-lookup"><span data-stu-id="672eb-172">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="672eb-173">応答</span><span class="sxs-lookup"><span data-stu-id="672eb-173">Response</span></span>

<span data-ttu-id="672eb-174">かどうかは成功すると、このメソッドは、`202 Accepted`の場所で応答コード: ヘッダーの[処理](../resources/teamsasyncoperation.md)リソースを指します。</span><span class="sxs-lookup"><span data-stu-id="672eb-174">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="672eb-175">操作が完了すると、処理リソースが送信されます作成したチームの id。</span><span class="sxs-lookup"><span data-stu-id="672eb-175">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="672eb-176">例</span><span class="sxs-lookup"><span data-stu-id="672eb-176">Example</span></span>
#### <a name="request"></a><span data-ttu-id="672eb-177">要求</span><span class="sxs-lookup"><span data-stu-id="672eb-177">Request</span></span>
<span data-ttu-id="672eb-178">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="672eb-178">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="672eb-179">応答</span><span class="sxs-lookup"><span data-stu-id="672eb-179">Response</span></span>
<span data-ttu-id="672eb-180">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="672eb-180">The following is an example of the response.</span></span> <span data-ttu-id="672eb-181">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="672eb-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="672eb-182">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="672eb-182">All of the properties will be returned from an actual call.</span></span>
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
