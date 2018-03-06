# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="b82ed-101">Microsoft Graph でのグループの操作</span><span class="sxs-lookup"><span data-stu-id="b82ed-101">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="b82ed-102">グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有している[ユーザー](user.md)その他のプリンシパルの集合です。</span><span class="sxs-lookup"><span data-stu-id="b82ed-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="b82ed-103">Microsoft Graph では、シナリオに従って、さまざまな種類のグループとグループ機能を作成および管理するために使用できる API を提供します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="b82ed-104">Microsoft Graph でのすべてのグループ関連の操作には、管理者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="b82ed-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="b82ed-105">**注**:グループは、職場または学校のアカウントでのみ作成できます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="b82ed-106">個人用 Microsoft アカウントはグループをサポートしません。</span><span class="sxs-lookup"><span data-stu-id="b82ed-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="b82ed-107">種類</span><span class="sxs-lookup"><span data-stu-id="b82ed-107">Type</span></span>              | <span data-ttu-id="b82ed-108">使用例</span><span class="sxs-lookup"><span data-stu-id="b82ed-108">Use case</span></span> | <span data-ttu-id="b82ed-109">groupType</span><span class="sxs-lookup"><span data-stu-id="b82ed-109">groupType</span></span> | <span data-ttu-id="b82ed-110">メールが有効</span><span class="sxs-lookup"><span data-stu-id="b82ed-110">mail-enabled</span></span> | <span data-ttu-id="b82ed-111">セキュリティが有効</span><span class="sxs-lookup"><span data-stu-id="b82ed-111">security-enabled</span></span> | <span data-ttu-id="b82ed-112">API 経由で作成できますか?</span><span class="sxs-lookup"><span data-stu-id="b82ed-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="b82ed-113">Office 365 グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="b82ed-114">共有の Microsoft オンライン リソースを持つユーザーのコラボレーションを容易にします。</span><span class="sxs-lookup"><span data-stu-id="b82ed-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="b82ed-115">はい</span><span class="sxs-lookup"><span data-stu-id="b82ed-115">Yes</span></span> |
| [<span data-ttu-id="b82ed-116">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-116">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="b82ed-117">ユーザーのアプリ内リソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-117">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="b82ed-118">はい</span><span class="sxs-lookup"><span data-stu-id="b82ed-118">Yes</span></span> |
| [<span data-ttu-id="b82ed-119">メールが有効なセキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-119">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="b82ed-120">共有グループ メールボックスにより、アプリ内リソースへのユーザー アクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-120">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="b82ed-121">なし</span><span class="sxs-lookup"><span data-stu-id="b82ed-121">No</span></span> |
| <span data-ttu-id="b82ed-122">配布グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-122">Distribution groups</span></span> | <span data-ttu-id="b82ed-123">グループのメンバーにメールを配布します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-123">Distributing mail to the members of the group.</span></span> <span data-ttu-id="b82ed-124">豊富なリソース セットを提供するため Office 365 グループを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b82ed-124">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="b82ed-125">なし</span><span class="sxs-lookup"><span data-stu-id="b82ed-125">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="b82ed-126">Office 365 グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-126">Office 365 groups</span></span>
<span data-ttu-id="b82ed-127">Office 365 グループのパワーは、共同作業の性質にあり、プロジェクトまたはチームで共同作業するユーザーに最適です。</span><span class="sxs-lookup"><span data-stu-id="b82ed-127">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="b82ed-128">それは、以下を含む、グループのメンバーが共有するリソースとともに作成されます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-128">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="b82ed-129">Outlook 会話</span><span class="sxs-lookup"><span data-stu-id="b82ed-129">Outlook conversations</span></span>
- <span data-ttu-id="b82ed-130">Outlook カレンダー</span><span class="sxs-lookup"><span data-stu-id="b82ed-130">Outlook calendar</span></span>
- <span data-ttu-id="b82ed-131">SharePoint ファイル</span><span class="sxs-lookup"><span data-stu-id="b82ed-131">SharePoint files</span></span>
- <span data-ttu-id="b82ed-132">OneNote ノートブック</span><span class="sxs-lookup"><span data-stu-id="b82ed-132">OneNote notebook</span></span>
- <span data-ttu-id="b82ed-133">SharePoint チーム サイト</span><span class="sxs-lookup"><span data-stu-id="b82ed-133">SharePoint team site</span></span>
- <span data-ttu-id="b82ed-134">Planner の計画</span><span class="sxs-lookup"><span data-stu-id="b82ed-134">Planner plans</span></span>
- <span data-ttu-id="b82ed-135">Intune デバイス管理</span><span class="sxs-lookup"><span data-stu-id="b82ed-135">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="b82ed-136">Outlook 内のグループ例</span><span class="sxs-lookup"><span data-stu-id="b82ed-136">Group in Outlook example</span></span>

<span data-ttu-id="b82ed-137">Outlook 内にあるグループの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-137">The following is a JSON representation of groups in Outlook.</span></span> 

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```
<span data-ttu-id="b82ed-138">Office 365 グループと管理者の操作性の詳細については、「[Office 365 グループの概要](https://support.office.com/ja-JP/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b82ed-138">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/ja-JP/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="b82ed-139">セキュリティ グループとメールが有効なセキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-139">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="b82ed-140">セキュリティ グループは、リソースへのユーザー アクセスを制御するためのものです。</span><span class="sxs-lookup"><span data-stu-id="b82ed-140">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="b82ed-141">ユーザーがセキュリティ グループのメンバーであるかどうかを確認することで、そのユーザーがアプリ内のいくつかのセキュア リソースにアクセスしようとしているときに、アプリが承認を判断することができます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-141">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="b82ed-142">セキュリティ グループには、ユーザーおよび他のセキュリティ グループをメンバーとして含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-142">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="b82ed-143">メールが有効なセキュリティ グループは、セキュリティ グループと同じ方法で使用されますが、グループの共有メールボックス機能が追加されています。</span><span class="sxs-lookup"><span data-stu-id="b82ed-143">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="b82ed-144">API では、メールが有効なセキュリティ グループを作成することはできませんが、他のグループ操作は動作します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-144">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span>  <span data-ttu-id="b82ed-145">メールが有効なセキュリティ グループは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b82ed-145">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="b82ed-146">詳細については、「[メールが有効なセキュリティ グループの管理](https://technet.microsoft.com/ja-JP/library/bb123521%28v=exchg.160%29.aspx)」の Exchange 記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b82ed-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/ja-JP/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="b82ed-147">セキュリティ グループの例</span><span class="sxs-lookup"><span data-stu-id="b82ed-147">Security group example</span></span>

<span data-ttu-id="b82ed-148">セキュリティ グループの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-148">The following is a JSON representation of a security group.</span></span> 

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```
## <a name="dynamic-membership"></a><span data-ttu-id="b82ed-149">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="b82ed-149">Dynamic membership</span></span> 

<span data-ttu-id="b82ed-150">すべての種類のグループには、ユーザーのプロパティに基づいてグループから自動的にメンバーを追加または削除する動的メンバーシップ ルールを付けることができます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="b82ed-151">たとえば、"マーケティング従業員グループ" には、部署プロパティを "マーケティング" に設定したすべてのユーザーが含まれます。これにより、新たなマーケティング従業員は自動的にグループに追加され、部署を脱退する従業員は自動的にグループから削除されます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="b82ed-152">このルールは、グループの作成中に `"membershipRule": 'user.department -eq "Marketing"'` として "membershipRule" フィールドに指定できます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="b82ed-153">GroupType には `"DynamicMembership"` も含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="b82ed-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="b82ed-154">次の要求では、マーケティング従業員用の新しい Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

<span data-ttu-id="b82ed-155">membershipRule の数式化の詳細については、「[Azure Active Directory で動的グループ メンバーシップの属性ベースのルールを作成する](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b82ed-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="b82ed-156">**注**: 動的メンバーシップ ルールには、[Azure Active Directory Premium P1](https://azure.microsoft.com/ja-JP/pricing/details/active-directory/) 以上の階層のライセンスを持つテナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="b82ed-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/ja-JP/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="b82ed-157">その他の種類のグループ</span><span class="sxs-lookup"><span data-stu-id="b82ed-157">Other types of groups</span></span>

<span data-ttu-id="b82ed-158">Yammer の Office 365 グループは、Yammer への投稿によりユーザーのコラボレーションを容易にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="b82ed-159">この種類のグループは、読み取りの要求で返すことができますが、その投稿に API でアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b82ed-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="b82ed-160">Yammer 投稿とスレッド フィードがグループで有効になると、既定の Office 365 グループ会話が無効になります。</span><span class="sxs-lookup"><span data-stu-id="b82ed-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="b82ed-161">詳細については、「[Yammer 開発者向け API ドキュメント](https://developer.yammer.com/docs)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b82ed-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="b82ed-162">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="b82ed-162">Common use cases</span></span>

<span data-ttu-id="b82ed-163">Microsoft Graph を使用して、次の一般的な操作を実行することができます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="b82ed-164">**ユース ケース**</span><span class="sxs-lookup"><span data-stu-id="b82ed-164">**Use cases**</span></span>  | <span data-ttu-id="b82ed-165">**REST リソース**</span><span class="sxs-lookup"><span data-stu-id="b82ed-165">**REST resources**</span></span> | <span data-ttu-id="b82ed-166">**関連項目**</span><span class="sxs-lookup"><span data-stu-id="b82ed-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b82ed-167">**グループ オブジェクトおよびメソッド**</span><span class="sxs-lookup"><span data-stu-id="b82ed-167">**Group object and methods**</span></span> | | |
| <span data-ttu-id="b82ed-168">新しいグループの作成、既存グループの取得、グループでのプロパティの更新、グループの削除を行います。</span><span class="sxs-lookup"><span data-stu-id="b82ed-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="b82ed-169">現在、API を使用して、セキュリティ グループと Outlook 内グループのみを作成できます。</span><span class="sxs-lookup"><span data-stu-id="b82ed-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="b82ed-170">group</span><span class="sxs-lookup"><span data-stu-id="b82ed-170">group</span></span>](group.md) | [<span data-ttu-id="b82ed-171">新しいグループを作成する</span><span class="sxs-lookup"><span data-stu-id="b82ed-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="b82ed-172">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b82ed-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="b82ed-173">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="b82ed-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="b82ed-174">グループを削除する</span><span class="sxs-lookup"><span data-stu-id="b82ed-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="b82ed-175">**グループ メンバーシップ メソッド**</span><span class="sxs-lookup"><span data-stu-id="b82ed-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="b82ed-176">グループのメンバーを一覧表示し、メンバーを追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="b82ed-177">user</span><span class="sxs-lookup"><span data-stu-id="b82ed-177">user</span></span>](user.md) <br/> [<span data-ttu-id="b82ed-178">group</span><span class="sxs-lookup"><span data-stu-id="b82ed-178">group</span></span>](group.md)| [<span data-ttu-id="b82ed-179">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b82ed-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="b82ed-180">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="b82ed-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="b82ed-181">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="b82ed-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="b82ed-182">ユーザーがグループのメンバーであるかどうかを判別し、ユーザーがメンバーであるすべてのグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="b82ed-183">user</span><span class="sxs-lookup"><span data-stu-id="b82ed-183">user</span></span>](user.md) <br/> [<span data-ttu-id="b82ed-184">group</span><span class="sxs-lookup"><span data-stu-id="b82ed-184">group</span></span>](group.md)| [<span data-ttu-id="b82ed-185">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="b82ed-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="b82ed-186">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="b82ed-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="b82ed-187">グループの所有者を一覧表示し、所有者を追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="b82ed-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="b82ed-188">user</span><span class="sxs-lookup"><span data-stu-id="b82ed-188">user</span></span>](user.md) <br/> [<span data-ttu-id="b82ed-189">group</span><span class="sxs-lookup"><span data-stu-id="b82ed-189">group</span></span>](group.md)| [<span data-ttu-id="b82ed-190">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b82ed-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="b82ed-191">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="b82ed-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="b82ed-192">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="b82ed-192">Remove member</span></span>](../api/group_delete_members.md)|
