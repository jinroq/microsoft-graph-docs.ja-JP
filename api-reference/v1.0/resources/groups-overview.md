---
title: Microsoft Graph でのグループの操作
description: グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有しているユーザーその他のプリンシパルの集合です。 Microsoft Graph では、シナリオに従って、さまざまな種類のグループとグループ機能を作成および管理するために使用できる API を提供します。 Microsoft Graph でのすべてのグループ関連の操作には、管理者の同意が必要です。
author: dkershaw10
ms.openlocfilehash: f3d18fd2ebf579c878e50bfae66e3987b6ef1a84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301688"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="2a24d-105">Microsoft Graph でのグループの操作</span><span class="sxs-lookup"><span data-stu-id="2a24d-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="2a24d-106">グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有している[ユーザー](user.md)その他のプリンシパルの集合です。</span><span class="sxs-lookup"><span data-stu-id="2a24d-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="2a24d-107">Microsoft Graph では、シナリオに従って、さまざまな種類のグループとグループ機能を作成および管理するために使用できる API を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="2a24d-108">Microsoft Graph でのすべてのグループ関連の操作には、管理者の同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a24d-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="2a24d-109">**注**:グループは、職場または学校のアカウントでのみ作成できます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="2a24d-110">個人用 Microsoft アカウントはグループをサポートしません。</span><span class="sxs-lookup"><span data-stu-id="2a24d-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="2a24d-111">種類</span><span class="sxs-lookup"><span data-stu-id="2a24d-111">Type</span></span>              | <span data-ttu-id="2a24d-112">使用例</span><span class="sxs-lookup"><span data-stu-id="2a24d-112">Use case</span></span> | <span data-ttu-id="2a24d-113">groupType</span><span class="sxs-lookup"><span data-stu-id="2a24d-113">groupType</span></span> | <span data-ttu-id="2a24d-114">メールが有効</span><span class="sxs-lookup"><span data-stu-id="2a24d-114">mail-enabled</span></span> | <span data-ttu-id="2a24d-115">セキュリティが有効</span><span class="sxs-lookup"><span data-stu-id="2a24d-115">security-enabled</span></span> | <span data-ttu-id="2a24d-116">API 経由で作成できますか?</span><span class="sxs-lookup"><span data-stu-id="2a24d-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="2a24d-117">Office 365 グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="2a24d-118">共有の Microsoft オンライン リソースを持つユーザーのコラボレーションを容易にします。</span><span class="sxs-lookup"><span data-stu-id="2a24d-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="2a24d-119">はい</span><span class="sxs-lookup"><span data-stu-id="2a24d-119">Yes</span></span> |
| [<span data-ttu-id="2a24d-120">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="2a24d-121">ユーザーのアプリ内リソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="2a24d-122">はい</span><span class="sxs-lookup"><span data-stu-id="2a24d-122">Yes</span></span> |
| [<span data-ttu-id="2a24d-123">メールが有効なセキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="2a24d-124">共有グループ メールボックスにより、アプリ内リソースへのユーザー アクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="2a24d-125">なし</span><span class="sxs-lookup"><span data-stu-id="2a24d-125">No</span></span> |
| <span data-ttu-id="2a24d-126">配布グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-126">Distribution groups</span></span> | <span data-ttu-id="2a24d-127">グループのメンバーにメールを配布します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="2a24d-128">豊富なリソース セットを提供するため Office 365 グループを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2a24d-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="2a24d-129">なし</span><span class="sxs-lookup"><span data-stu-id="2a24d-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="2a24d-130">Office 365 グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-130">Office 365 groups</span></span>
<span data-ttu-id="2a24d-131">Office 365 グループのパワーは、共同作業の性質にあり、プロジェクトまたはチームで共同作業するユーザーに最適です。</span><span class="sxs-lookup"><span data-stu-id="2a24d-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="2a24d-132">それは、以下を含む、グループのメンバーが共有するリソースとともに作成されます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="2a24d-133">Outlook 会話</span><span class="sxs-lookup"><span data-stu-id="2a24d-133">Outlook conversations</span></span>
- <span data-ttu-id="2a24d-134">Outlook カレンダー</span><span class="sxs-lookup"><span data-stu-id="2a24d-134">Outlook calendar</span></span>
- <span data-ttu-id="2a24d-135">SharePoint ファイル</span><span class="sxs-lookup"><span data-stu-id="2a24d-135">SharePoint files</span></span>
- <span data-ttu-id="2a24d-136">OneNote ノートブック</span><span class="sxs-lookup"><span data-stu-id="2a24d-136">OneNote notebook</span></span>
- <span data-ttu-id="2a24d-137">SharePoint チーム サイト</span><span class="sxs-lookup"><span data-stu-id="2a24d-137">SharePoint team site</span></span>
- <span data-ttu-id="2a24d-138">Planner の計画</span><span class="sxs-lookup"><span data-stu-id="2a24d-138">Planner plans</span></span>
- <span data-ttu-id="2a24d-139">Intune デバイス管理</span><span class="sxs-lookup"><span data-stu-id="2a24d-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="2a24d-140">Outlook 内のグループ例</span><span class="sxs-lookup"><span data-stu-id="2a24d-140">Group in Outlook example</span></span>

<span data-ttu-id="2a24d-141">Outlook 内にあるグループの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="2a24d-142">Office 365 グループと管理者の操作性の詳細については、「[Office 365 グループの概要](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a24d-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="2a24d-143">セキュリティ グループとメールが有効なセキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="2a24d-144">セキュリティ グループは、リソースへのユーザー アクセスを制御するためのものです。</span><span class="sxs-lookup"><span data-stu-id="2a24d-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="2a24d-145">ユーザーがセキュリティ グループのメンバーであるかどうかを確認することで、そのユーザーがアプリ内のいくつかのセキュア リソースにアクセスしようとしているときに、アプリが承認を判断することができます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="2a24d-146">セキュリティ グループには、ユーザーおよび他のセキュリティ グループをメンバーとして含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="2a24d-147">メールが有効なセキュリティ グループは、セキュリティ グループと同じ方法で使用されますが、グループの共有メールボックス機能が追加されています。</span><span class="sxs-lookup"><span data-stu-id="2a24d-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="2a24d-148">API では、メールが有効なセキュリティ グループを作成することはできませんが、他のグループ操作は動作します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="2a24d-149">メールが有効なセキュリティ グループは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2a24d-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="2a24d-150">詳細については、「[メールが有効なセキュリティ グループの管理](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx)」の Exchange 記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a24d-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="2a24d-151">セキュリティ グループの例</span><span class="sxs-lookup"><span data-stu-id="2a24d-151">Security group example</span></span>

<span data-ttu-id="2a24d-152">セキュリティ グループの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="2a24d-153">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="2a24d-153">Dynamic membership</span></span> 

<span data-ttu-id="2a24d-154">すべての種類のグループには、ユーザーのプロパティに基づいてグループから自動的にメンバーを追加または削除する動的メンバーシップ ルールを付けることができます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="2a24d-155">たとえば、"マーケティング従業員グループ" には、部署プロパティを "マーケティング" に設定したすべてのユーザーが含まれます。これにより、新たなマーケティング従業員は自動的にグループに追加され、部署を脱退する従業員は自動的にグループから削除されます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="2a24d-156">このルールは、グループの作成中に `"membershipRule": 'user.department -eq "Marketing"'` として "membershipRule" フィールドに指定できます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="2a24d-157">GroupType には `"DynamicMembership"` も含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a24d-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="2a24d-158">次の要求では、マーケティング従業員用の新しい Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="2a24d-159">membershipRule の数式化の詳細については、「[Azure Active Directory で動的グループ メンバーシップの属性ベースのルールを作成する](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a24d-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="2a24d-160">**注**: 動的メンバーシップ ルールには、[Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) 以上の階層のライセンスを持つテナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="2a24d-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="2a24d-161">その他の種類のグループ</span><span class="sxs-lookup"><span data-stu-id="2a24d-161">Other types of groups</span></span>

<span data-ttu-id="2a24d-162">Yammer の Office 365 グループは、Yammer への投稿によりユーザーのコラボレーションを容易にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="2a24d-163">この種類のグループは、読み取りの要求で返すことができますが、その投稿に API でアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="2a24d-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="2a24d-164">Yammer 投稿とスレッド フィードがグループで有効になると、既定の Office 365 グループ会話が無効になります。</span><span class="sxs-lookup"><span data-stu-id="2a24d-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="2a24d-165">詳細については、「[Yammer 開発者向け API ドキュメント](https://developer.yammer.com/docs)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2a24d-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="2a24d-166">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="2a24d-166">Common use cases</span></span>

<span data-ttu-id="2a24d-167">Microsoft Graph を使用して、次の一般的な操作を実行することができます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-167">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="2a24d-168">**ユース ケース**</span><span class="sxs-lookup"><span data-stu-id="2a24d-168">**Use cases**</span></span>  | <span data-ttu-id="2a24d-169">**REST リソース**</span><span class="sxs-lookup"><span data-stu-id="2a24d-169">**REST resources**</span></span> | <span data-ttu-id="2a24d-170">**関連項目**</span><span class="sxs-lookup"><span data-stu-id="2a24d-170">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="2a24d-171">**グループ オブジェクトおよびメソッド**</span><span class="sxs-lookup"><span data-stu-id="2a24d-171">**Group object and methods**</span></span> | | |
| <span data-ttu-id="2a24d-172">新しいグループの作成、既存グループの取得、グループでのプロパティの更新、グループの削除を行います。</span><span class="sxs-lookup"><span data-stu-id="2a24d-172">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="2a24d-173">現在、API を使用して、セキュリティ グループと Outlook 内グループのみを作成できます。</span><span class="sxs-lookup"><span data-stu-id="2a24d-173">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="2a24d-174">group</span><span class="sxs-lookup"><span data-stu-id="2a24d-174">group</span></span>](group.md) | [<span data-ttu-id="2a24d-175">新しいグループを作成する</span><span class="sxs-lookup"><span data-stu-id="2a24d-175">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="2a24d-176">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a24d-176">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="2a24d-177">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="2a24d-177">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="2a24d-178">グループを削除する</span><span class="sxs-lookup"><span data-stu-id="2a24d-178">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="2a24d-179">**グループ メンバーシップ メソッド**</span><span class="sxs-lookup"><span data-stu-id="2a24d-179">**Group membership methods**</span></span> | | |
| <span data-ttu-id="2a24d-180">グループのメンバーを一覧表示し、メンバーを追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-180">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="2a24d-181">user</span><span class="sxs-lookup"><span data-stu-id="2a24d-181">user</span></span>](user.md) <br/> [<span data-ttu-id="2a24d-182">group</span><span class="sxs-lookup"><span data-stu-id="2a24d-182">group</span></span>](group.md)| [<span data-ttu-id="2a24d-183">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a24d-183">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="2a24d-184">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="2a24d-184">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="2a24d-185">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="2a24d-185">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="2a24d-186">ユーザーがグループのメンバーであるかどうかを判別し、ユーザーがメンバーであるすべてのグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-186">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="2a24d-187">user</span><span class="sxs-lookup"><span data-stu-id="2a24d-187">user</span></span>](user.md) <br/> [<span data-ttu-id="2a24d-188">group</span><span class="sxs-lookup"><span data-stu-id="2a24d-188">group</span></span>](group.md)| [<span data-ttu-id="2a24d-189">メンバー グループをチェックする</span><span class="sxs-lookup"><span data-stu-id="2a24d-189">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="2a24d-190">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="2a24d-190">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="2a24d-191">グループの所有者を一覧表示し、所有者を追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="2a24d-191">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="2a24d-192">user</span><span class="sxs-lookup"><span data-stu-id="2a24d-192">user</span></span>](user.md) <br/> [<span data-ttu-id="2a24d-193">group</span><span class="sxs-lookup"><span data-stu-id="2a24d-193">group</span></span>](group.md)| [<span data-ttu-id="2a24d-194">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a24d-194">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="2a24d-195">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="2a24d-195">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="2a24d-196">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="2a24d-196">Remove member</span></span>](../api/group-delete-members.md)|
