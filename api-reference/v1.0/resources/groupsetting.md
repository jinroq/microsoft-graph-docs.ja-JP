# <a name="groupsetting-resource-type"></a><span data-ttu-id="1047c-101">groupSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1047c-101">groupSetting resource type</span></span>

<span data-ttu-id="1047c-102">グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="1047c-102">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="1047c-p101">グループ設定は、使用可能な [groupSettingTemplates](groupSettingTemplate.md) に基づいて作成することができ、事前設定された既定値を変更することができます。これらの設定は、テナント全体のレベルまたは特定のグループのグループ基本動作を制御します。テナント全体および特定のグループの両方で同じ設定が定義されている場合、グループ レベルの設定がテナント全体の設定よりも優先されます。たとえば、テナント全体の設定では、ゲストは既存のグループのメンバーによって招待されることがありますが、個別のグループ設定を優先することができ、その場合は、グループのメンバーはゲストを招待することができません。グループ設定は、Office 365 グループの動作のみを制御します。</span><span class="sxs-lookup"><span data-stu-id="1047c-p101">Group settings can be created based on the available [groupSettingTemplates](groupSettingTemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="1047c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1047c-108">Methods</span></span>

| <span data-ttu-id="1047c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1047c-109">Method</span></span> | <span data-ttu-id="1047c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1047c-110">Return Type</span></span> | <span data-ttu-id="1047c-111">説明</span><span class="sxs-lookup"><span data-stu-id="1047c-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="1047c-112">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="1047c-112">Create setting</span></span>](../api/groupsetting_post_groupsettings.md) | [<span data-ttu-id="1047c-113">groupSetting</span><span class="sxs-lookup"><span data-stu-id="1047c-113">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="1047c-p102">groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1047c-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="1047c-116">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="1047c-116">Get setting</span></span>](../api/groupsetting_get.md) | [<span data-ttu-id="1047c-117">groupSetting</span><span class="sxs-lookup"><span data-stu-id="1047c-117">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="1047c-118">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="1047c-118">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="1047c-119">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1047c-119">List settings</span></span>](../api/groupsetting_list.md) | <span data-ttu-id="1047c-120">[groupSetting](groupsetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1047c-120">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="1047c-121">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1047c-121">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="1047c-122">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="1047c-122">Update setting</span></span>](../api/groupsetting_update.md) | [<span data-ttu-id="1047c-123">groupSetting</span><span class="sxs-lookup"><span data-stu-id="1047c-123">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="1047c-124">Groupsetting オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1047c-124">Update groupsetting object.</span></span> |
|[<span data-ttu-id="1047c-125">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="1047c-125">Delete setting</span></span>](../api/groupsetting_delete.md) | <span data-ttu-id="1047c-126">なし</span><span class="sxs-lookup"><span data-stu-id="1047c-126">None</span></span> | <span data-ttu-id="1047c-127">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1047c-127">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1047c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1047c-128">Properties</span></span>

| <span data-ttu-id="1047c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1047c-129">Property</span></span> | <span data-ttu-id="1047c-130">タイプ</span><span class="sxs-lookup"><span data-stu-id="1047c-130">Type</span></span> | <span data-ttu-id="1047c-131">説明</span><span class="sxs-lookup"><span data-stu-id="1047c-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1047c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1047c-132">displayName</span></span>|<span data-ttu-id="1047c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1047c-133">String</span></span>| <span data-ttu-id="1047c-134">関連するテンプレートに由来する設定グループの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="1047c-134">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="1047c-135">ID</span><span class="sxs-lookup"><span data-stu-id="1047c-135">id</span></span>|<span data-ttu-id="1047c-136">文字列</span><span class="sxs-lookup"><span data-stu-id="1047c-136">String</span></span>| <span data-ttu-id="1047c-p103">設定の一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1047c-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="1047c-139">templateId</span><span class="sxs-lookup"><span data-stu-id="1047c-139">templateId</span></span>|<span data-ttu-id="1047c-140">文字列</span><span class="sxs-lookup"><span data-stu-id="1047c-140">String</span></span>| <span data-ttu-id="1047c-p104">設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1047c-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="1047c-143">値</span><span class="sxs-lookup"><span data-stu-id="1047c-143">values</span></span>|<span data-ttu-id="1047c-144">[settingValue](settingvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1047c-144">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="1047c-p105">名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="1047c-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1047c-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1047c-147">Relationships</span></span>

<span data-ttu-id="1047c-148">なし。</span><span class="sxs-lookup"><span data-stu-id="1047c-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1047c-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1047c-149">JSON representation</span></span>

<span data-ttu-id="1047c-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1047c-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->