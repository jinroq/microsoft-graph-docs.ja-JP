---
title: チームのクローンを作成する
description: チームのコピーを作成します。 この操作では、対応するグループのコピーも作成されます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ed4880d80bd94febc4d12deb04ca10a4cb7dad3
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396738"
---
# <a name="clone-a-team"></a><span data-ttu-id="75069-104">チームのクローンを作成する</span><span class="sxs-lookup"><span data-stu-id="75069-104">Clone a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75069-105">[チーム](../resources/team.md)のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="75069-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="75069-106">この操作では、対応する[グループ](../resources/group.md)のコピーも作成されます。</span><span class="sxs-lookup"><span data-stu-id="75069-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="75069-107">チームのどの部分を複製するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="75069-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="75069-108">**アプリ**-チームにインストールされている Microsoft Teams アプリをコピーします。</span><span class="sxs-lookup"><span data-stu-id="75069-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="75069-109">\*\*\*\* チャネル–チャネル構造をコピーします (チャネル内のメッセージはコピーしません)。</span><span class="sxs-lookup"><span data-stu-id="75069-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="75069-110">**members** –グループのメンバーと所有者をコピーします。</span><span class="sxs-lookup"><span data-stu-id="75069-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="75069-111">**設定**–主要なグループ設定と共に、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="75069-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="75069-112">**タブ**–チャネル内のタブをコピーします。</span><span class="sxs-lookup"><span data-stu-id="75069-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="75069-113">タブが複製されると、それらは未構成状態になります。これは、Microsoft Teams のタブバーに表示されます。これを最初に開いたときに、構成画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="75069-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="75069-114">(タブを開くユーザーがアプリを構成するためのアクセス許可を持っていない場合は、タブがまだ構成されていないことを示すメッセージが表示されます)。</span><span class="sxs-lookup"><span data-stu-id="75069-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="75069-115">複製は、長時間実行される操作です。</span><span class="sxs-lookup"><span data-stu-id="75069-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="75069-116">POST クローンが戻ると、Location: header から返される[操作](../resources/teamsasyncoperation.md)を取得して、"実行中" または "成功" または "失敗" のどちらであるかを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="75069-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) returned by the Location: header to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="75069-117">状態が "実行中" ではない状態になるまで、この操作を続行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="75069-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="75069-118">推奨される遅延時間は、5秒です。</span><span class="sxs-lookup"><span data-stu-id="75069-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="75069-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75069-119">Permissions</span></span>

<span data-ttu-id="75069-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75069-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75069-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75069-122">Permission type</span></span>      | <span data-ttu-id="75069-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75069-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75069-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75069-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="75069-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75069-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75069-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75069-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75069-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75069-127">Not supported.</span></span>    |
|<span data-ttu-id="75069-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75069-128">Application</span></span>                            | <span data-ttu-id="75069-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75069-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75069-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75069-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="75069-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75069-131">Request headers</span></span>
| <span data-ttu-id="75069-132">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75069-132">Header</span></span>       | <span data-ttu-id="75069-133">値</span><span class="sxs-lookup"><span data-stu-id="75069-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75069-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="75069-134">Authorization</span></span>  | <span data-ttu-id="75069-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75069-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75069-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75069-137">Content-Type</span></span>  | <span data-ttu-id="75069-138">application/json</span><span class="sxs-lookup"><span data-stu-id="75069-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75069-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="75069-139">Request body</span></span>

| <span data-ttu-id="75069-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75069-140">Property</span></span>     | <span data-ttu-id="75069-141">型</span><span class="sxs-lookup"><span data-stu-id="75069-141">Type</span></span>   |<span data-ttu-id="75069-142">説明</span><span class="sxs-lookup"><span data-stu-id="75069-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75069-143">classification</span><span class="sxs-lookup"><span data-stu-id="75069-143">classification</span></span>|<span data-ttu-id="75069-144">String (省略可能)</span><span class="sxs-lookup"><span data-stu-id="75069-144">String (optional)</span></span>|<span data-ttu-id="75069-145">グループの分類 (低、中、高のビジネスへの影響など) を記述します。</span><span class="sxs-lookup"><span data-stu-id="75069-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="75069-146">このプロパティの有効な値は、[テンプレート定義](../resources/directorysettingtemplate.md)に基づいて ClassificationList[設定](../resources/directorysetting.md)値を作成することによって定義されます。</span><span class="sxs-lookup"><span data-stu-id="75069-146">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="75069-147">分類が指定されていない場合は、元のチーム/グループから分類がコピーされます。</span><span class="sxs-lookup"><span data-stu-id="75069-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="75069-148">description</span><span class="sxs-lookup"><span data-stu-id="75069-148">description</span></span>|<span data-ttu-id="75069-149">String (省略可能)</span><span class="sxs-lookup"><span data-stu-id="75069-149">String (optional)</span></span>|<span data-ttu-id="75069-150">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="75069-150">An optional description for the group.</span></span> <span data-ttu-id="75069-151">このプロパティが指定されていない場合は、空白のままになります。</span><span class="sxs-lookup"><span data-stu-id="75069-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="75069-152">displayName</span><span class="sxs-lookup"><span data-stu-id="75069-152">displayName</span></span>|<span data-ttu-id="75069-153">String</span><span class="sxs-lookup"><span data-stu-id="75069-153">String</span></span>|<span data-ttu-id="75069-p109">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="75069-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="75069-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="75069-157">mailNickname</span></span>|<span data-ttu-id="75069-158">String</span><span class="sxs-lookup"><span data-stu-id="75069-158">String</span></span>|<span data-ttu-id="75069-159">グループのメール エイリアスです (組織内で一意)。</span><span class="sxs-lookup"><span data-stu-id="75069-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="75069-160">このプロパティは、グループの作成時に指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="75069-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="75069-161">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="75069-161">Supports $filter.</span></span> <span data-ttu-id="75069-162">このプロパティが指定されていない場合は、displayName から計算されます。</span><span class="sxs-lookup"><span data-stu-id="75069-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="75069-163">既知の問題: このプロパティは現在無視されています。</span><span class="sxs-lookup"><span data-stu-id="75069-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="75069-164">partsToClone</span><span class="sxs-lookup"><span data-stu-id="75069-164">partsToClone</span></span>| [<span data-ttu-id="75069-165">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="75069-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="75069-166">クローンするパーツのコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="75069-166">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="75069-167">法的パーツとは、「アプリ、タブ、設定、チャネル、メンバー」のことです。</span><span class="sxs-lookup"><span data-stu-id="75069-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="75069-168">visibility</span><span class="sxs-lookup"><span data-stu-id="75069-168">visibility</span></span>|<span data-ttu-id="75069-169">[teamVisibilityType](../resources/teamvisibilitytype.md)オプション</span><span class="sxs-lookup"><span data-stu-id="75069-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="75069-170">グループを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="75069-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="75069-171">可能な値は、 **Private**、 **Public**です。</span><span class="sxs-lookup"><span data-stu-id="75069-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="75069-172">Visibility が指定されていない場合、表示は元のチーム/グループからコピーされます。</span><span class="sxs-lookup"><span data-stu-id="75069-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="75069-173">複製対象のチームが**educationClass**チームの場合、visibility パラメーターは無視され、新しいグループの表示が HiddenMembership に設定されます。</span><span class="sxs-lookup"><span data-stu-id="75069-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="75069-174">応答</span><span class="sxs-lookup"><span data-stu-id="75069-174">Response</span></span>

<span data-ttu-id="75069-175">成功した場合、このメソッドは`202 Accepted` 、 [operation](../resources/teamsasyncoperation.md)リソースをポイントする Location: ヘッダーを持つ応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="75069-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="75069-176">操作が完了すると、作成されたチームの id が操作リソースに通知されます。</span><span class="sxs-lookup"><span data-stu-id="75069-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="75069-177">例</span><span class="sxs-lookup"><span data-stu-id="75069-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="75069-178">要求</span><span class="sxs-lookup"><span data-stu-id="75069-178">Request</span></span>
<span data-ttu-id="75069-179">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75069-179">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="75069-180">応答</span><span class="sxs-lookup"><span data-stu-id="75069-180">Response</span></span>
<span data-ttu-id="75069-181">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75069-181">The following is an example of the response.</span></span> <span data-ttu-id="75069-182">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="75069-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="75069-183">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="75069-183">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
