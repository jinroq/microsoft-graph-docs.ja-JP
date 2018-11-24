# <a name="clone-a-team"></a><span data-ttu-id="02f2d-101">チームのクローンを作成します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-101">Clone a team</span></span>



<span data-ttu-id="02f2d-102">[チーム](../resources/team.md)のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-102">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="02f2d-103">この操作では、対応する[グループ](../resources/group.md)のコピーも作成します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-103">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="02f2d-104">クローンを作成するチームのどの部分を指定できます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-104">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="02f2d-105">**アプリケーション**・ チームにインストールされているアプリケーションをマイクロソフト チームのコピーです。</span><span class="sxs-lookup"><span data-stu-id="02f2d-105">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="02f2d-106">**チャネル**は、チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-106">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="02f2d-107">**メンバー** -メンバーをコピーし、グループの所有者です。</span><span class="sxs-lookup"><span data-stu-id="02f2d-107">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="02f2d-108">**設定**– は、キーのグループの設定と、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-108">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="02f2d-109">**タブ**– は、チャネル内のタブにコピーします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-109">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="02f2d-110">タブがクローン化されると、未構成の状態に移動する:、マイクロソフト チームのタブ バーに表示され、構成] 画面で移動します] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-110">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="02f2d-111">(タブを開いた人がアプリケーションを構成するのにはアクセス許可を持たない場合が表示されるタブが構成されていないことを説明するメッセージです。)</span><span class="sxs-lookup"><span data-stu-id="02f2d-111">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="02f2d-112">クローン作成は、時間のかかる操作です。</span><span class="sxs-lookup"><span data-stu-id="02f2d-112">Cloning is a long-running operation.</span></span>
<span data-ttu-id="02f2d-113">投稿クローンが返されるは、「実行中」または「成功」または「失敗」を表示する[操作](../resources/teamsasyncoperation.md)を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02f2d-113">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="02f2d-114">ステータスが「動作していない」まで取得を続行してください。</span><span class="sxs-lookup"><span data-stu-id="02f2d-114">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="02f2d-115">取得の推奨される間隔は、5 秒間です。</span><span class="sxs-lookup"><span data-stu-id="02f2d-115">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="02f2d-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02f2d-116">Permissions</span></span>

<span data-ttu-id="02f2d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02f2d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02f2d-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02f2d-119">Permission type</span></span>      | <span data-ttu-id="02f2d-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02f2d-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02f2d-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02f2d-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="02f2d-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f2d-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02f2d-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02f2d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02f2d-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f2d-124">Not supported.</span></span>    |
|<span data-ttu-id="02f2d-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02f2d-125">Application</span></span>                            | <span data-ttu-id="02f2d-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f2d-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02f2d-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02f2d-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="02f2d-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f2d-128">Request headers</span></span>
| <span data-ttu-id="02f2d-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f2d-129">Header</span></span>       | <span data-ttu-id="02f2d-130">値</span><span class="sxs-lookup"><span data-stu-id="02f2d-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02f2d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f2d-131">Authorization</span></span>  | <span data-ttu-id="02f2d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02f2d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02f2d-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02f2d-134">Content-Type</span></span>  | <span data-ttu-id="02f2d-135">application/json</span><span class="sxs-lookup"><span data-stu-id="02f2d-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02f2d-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="02f2d-136">Request body</span></span>

| <span data-ttu-id="02f2d-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02f2d-137">Property</span></span>     | <span data-ttu-id="02f2d-138">型</span><span class="sxs-lookup"><span data-stu-id="02f2d-138">Type</span></span>   |<span data-ttu-id="02f2d-139">説明</span><span class="sxs-lookup"><span data-stu-id="02f2d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f2d-140">分類</span><span class="sxs-lookup"><span data-stu-id="02f2d-140">classification</span></span>|<span data-ttu-id="02f2d-141">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="02f2d-141">String (optional)</span></span>|<span data-ttu-id="02f2d-142">(低、中、または高のビジネス ・ インパクト) などのグループの分類について説明します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-142">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="02f2d-143">分類を指定しない場合、分類は、元のチームまたはグループからコピーされます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-143">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="02f2d-144">description</span><span class="sxs-lookup"><span data-stu-id="02f2d-144">description</span></span>|<span data-ttu-id="02f2d-145">文字列 (省略可能)</span><span class="sxs-lookup"><span data-stu-id="02f2d-145">String (optional)</span></span>|<span data-ttu-id="02f2d-146">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="02f2d-146">An optional description for the group.</span></span> <span data-ttu-id="02f2d-147">このプロパティを指定しない場合、空白のままにします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-147">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="02f2d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="02f2d-148">displayName</span></span>|<span data-ttu-id="02f2d-149">文字列</span><span class="sxs-lookup"><span data-stu-id="02f2d-149">String</span></span>|<span data-ttu-id="02f2d-p108">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-p108">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="02f2d-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="02f2d-153">mailNickname</span></span>|<span data-ttu-id="02f2d-154">文字列</span><span class="sxs-lookup"><span data-stu-id="02f2d-154">String</span></span>|<span data-ttu-id="02f2d-155">グループ、組織内で一意の電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="02f2d-155">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="02f2d-156">グループが作成されるとき、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02f2d-156">This property must be specified when a group is created.</span></span> <span data-ttu-id="02f2d-157">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02f2d-157">Supports $filter.</span></span> <span data-ttu-id="02f2d-158">このプロパティが指定されていない場合に、表示名から計算されます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-158">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="02f2d-159">既知の問題: 現在、このプロパティは無視されます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-159">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="02f2d-160">partsToClone</span><span class="sxs-lookup"><span data-stu-id="02f2d-160">partsToClone</span></span>| [<span data-ttu-id="02f2d-161">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="02f2d-161">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="02f2d-162">クローンを作成する部品のコンマで区切られたリスト。</span><span class="sxs-lookup"><span data-stu-id="02f2d-162">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="02f2d-163">法的な部分は、「アプリケーション、タブ、設定、チャネル、メンバー"です。</span><span class="sxs-lookup"><span data-stu-id="02f2d-163">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="02f2d-164">visibility</span><span class="sxs-lookup"><span data-stu-id="02f2d-164">visibility</span></span>|<span data-ttu-id="02f2d-165">[teamVisibilityType](../resources/teamVisibilityType.md)(省略可能)</span><span class="sxs-lookup"><span data-stu-id="02f2d-165">[teamVisibilityType](../resources/teamVisibilityType.md) (optional)</span></span>| <span data-ttu-id="02f2d-166">グループの可視性を指定します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-166">Specifies the visibility of the group.</span></span> <span data-ttu-id="02f2d-167">使用可能な値:**パブリック**、**プライベート**です。</span><span class="sxs-lookup"><span data-stu-id="02f2d-167">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="02f2d-168">可視性が指定されていない場合、元のチームまたはグループの表示と非表示がコピーされます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-168">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="02f2d-169">**EducationClass**チームは、チームのクローンが作成されている場合、可視性パラメーターは無視されます、および新しいグループの表示/非表示を HiddenMembership に設定されます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-169">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="02f2d-170">応答</span><span class="sxs-lookup"><span data-stu-id="02f2d-170">Response</span></span>

<span data-ttu-id="02f2d-171">かどうかは成功すると、このメソッドは、`202 Accepted`の場所で応答コード: ヘッダーの[処理](../resources/teamsasyncoperation.md)リソースを指します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-171">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="02f2d-172">操作が完了すると、処理リソースが送信されます作成したチームの id。</span><span class="sxs-lookup"><span data-stu-id="02f2d-172">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="02f2d-173">例</span><span class="sxs-lookup"><span data-stu-id="02f2d-173">Example</span></span>
#### <a name="request"></a><span data-ttu-id="02f2d-174">要求</span><span class="sxs-lookup"><span data-stu-id="02f2d-174">Request</span></span>
<span data-ttu-id="02f2d-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-175">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="02f2d-176">応答</span><span class="sxs-lookup"><span data-stu-id="02f2d-176">Response</span></span>
<span data-ttu-id="02f2d-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02f2d-177">The following is an example of the response.</span></span> <span data-ttu-id="02f2d-178">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="02f2d-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="02f2d-179">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="02f2d-179">All of the properties will be returned from an actual call.</span></span>
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
