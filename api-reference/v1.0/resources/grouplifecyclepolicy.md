# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="3ec76-101">groupLifecyclePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="3ec76-101">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="3ec76-102">Office 365 グループのライフサイクル ポリシーを表します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-102">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="3ec76-103">グループのライフサイクル ポリシーにより、管理者はグループに対して有効期限を設定できます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-103">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="3ec76-104">たとえば、180 日後にグループの有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-104">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="3ec76-105">グループの有効期限に達すると、グループの所有者は、管理者が定義した時間間隔内でグループを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ec76-105">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="3ec76-106">更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-106">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="3ec76-107">たとえば、グループの新しい有効期限は、更新後 180 日です。</span><span class="sxs-lookup"><span data-stu-id="3ec76-107">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="3ec76-108">グループが更新されない場合、グループの有効期限が切れ、削除されます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-108">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="3ec76-109">グループは、削除から 30 日以内に復元できます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-109">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="3ec76-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ec76-110">Methods</span></span>

| <span data-ttu-id="3ec76-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ec76-111">Method</span></span> | <span data-ttu-id="3ec76-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ec76-112">Return Type</span></span> | <span data-ttu-id="3ec76-113">説明</span><span class="sxs-lookup"><span data-stu-id="3ec76-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ec76-114">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-114">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_get.md) | [<span data-ttu-id="3ec76-115">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-115">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="3ec76-116">groupLifecyclePolicy オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3ec76-116">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="3ec76-117">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="3ec76-117">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy_list.md) | <span data-ttu-id="3ec76-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3ec76-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="3ec76-119">すべての groupLifecyclePolicies を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-119">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="3ec76-120">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-120">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_update.md) | [<span data-ttu-id="3ec76-121">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-121">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="3ec76-122">groupLifecyclePolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-122">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="3ec76-123">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-123">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_delete.md) | <span data-ttu-id="3ec76-124">なし</span><span class="sxs-lookup"><span data-stu-id="3ec76-124">None</span></span> | <span data-ttu-id="3ec76-125">groupLifecyclePolicy オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-125">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="3ec76-126">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-126">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_addgroup.md)|<span data-ttu-id="3ec76-127">なし</span><span class="sxs-lookup"><span data-stu-id="3ec76-127">None</span></span>| <span data-ttu-id="3ec76-128">ライフ サイクル ポリシーにグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-128">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="3ec76-129">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec76-129">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_removegroup.md)|<span data-ttu-id="3ec76-130">なし</span><span class="sxs-lookup"><span data-stu-id="3ec76-130">None</span></span>| <span data-ttu-id="3ec76-131">ライフ サイクル ポリシーからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="3ec76-131">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ec76-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ec76-132">Properties</span></span>

| <span data-ttu-id="3ec76-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ec76-133">Property</span></span> | <span data-ttu-id="3ec76-134">タイプ</span><span class="sxs-lookup"><span data-stu-id="3ec76-134">Type</span></span> | <span data-ttu-id="3ec76-135">説明</span><span class="sxs-lookup"><span data-stu-id="3ec76-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3ec76-136">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="3ec76-136">alternateNotificationEmails</span></span>|<span data-ttu-id="3ec76-137">String</span><span class="sxs-lookup"><span data-stu-id="3ec76-137">String</span></span>| <span data-ttu-id="3ec76-138">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="3ec76-138">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="3ec76-139">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-139">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="3ec76-140">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="3ec76-140">groupLifetimeInDays</span></span>|<span data-ttu-id="3ec76-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec76-141">Int32</span></span>| <span data-ttu-id="3ec76-142">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="3ec76-142">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="3ec76-143">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="3ec76-143">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="3ec76-144">ID</span><span class="sxs-lookup"><span data-stu-id="3ec76-144">id</span></span>|<span data-ttu-id="3ec76-145">Guid</span><span class="sxs-lookup"><span data-stu-id="3ec76-145">Guid</span></span>| <span data-ttu-id="3ec76-146">ポリシーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="3ec76-146">A unique identifier for a policy.</span></span> <span data-ttu-id="3ec76-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3ec76-147">Read-only.</span></span>|
|<span data-ttu-id="3ec76-148">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="3ec76-148">managedGroupTypes</span></span>|<span data-ttu-id="3ec76-149">String</span><span class="sxs-lookup"><span data-stu-id="3ec76-149">String</span></span>| <span data-ttu-id="3ec76-150">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="3ec76-150">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="3ec76-151">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="3ec76-151">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3ec76-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ec76-152">Relationships</span></span>

<span data-ttu-id="3ec76-153">なし。</span><span class="sxs-lookup"><span data-stu-id="3ec76-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ec76-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ec76-154">JSON representation</span></span>

<span data-ttu-id="3ec76-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ec76-155">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->