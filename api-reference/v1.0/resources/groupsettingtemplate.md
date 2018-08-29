# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="14f76-101">groupSettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14f76-101">groupSettingTemplate resource type</span></span>

<span data-ttu-id="14f76-p101">グループ設定テンプレートは、テナントが使用できるシステム定義の設定を表します。[グループ設定](groupsetting.md)は、使用可能な **groupSettingTemplates** に基づいて作成することができ、値は事前設定された既定値から変更することができます。グループ設定テンプレートの作成、更新、削除はできません。これらの設定は、テナント全体の設定または特定のグループ設定を表すことができます。現時点では、利用可能なテンプレートは Office 365 グループのみに適用され、そこでユーザーがグループを作成したり、組織外からゲストをグループのメンバーに招待できるかどうかなどの設定をすることができます。</span><span class="sxs-lookup"><span data-stu-id="14f76-p101">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="14f76-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="14f76-107">Methods</span></span>

| <span data-ttu-id="14f76-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14f76-108">Method</span></span> | <span data-ttu-id="14f76-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14f76-109">Return Type</span></span> | <span data-ttu-id="14f76-110">説明</span><span class="sxs-lookup"><span data-stu-id="14f76-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="14f76-111">groupSettingTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="14f76-111">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate_get.md) | [<span data-ttu-id="14f76-112">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="14f76-112">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="14f76-113">システムで定義された groupSettingTemplate オブジェクトの特定のプロパティを読み込みます。</span><span class="sxs-lookup"><span data-stu-id="14f76-113">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="14f76-114">groupSettingTemplate のリスト</span><span class="sxs-lookup"><span data-stu-id="14f76-114">List groupSettingTemplate</span></span>](../api/groupsettingtemplate_list.md) | [<span data-ttu-id="14f76-115">GroupSettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="14f76-115">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="14f76-116">システムで定義された groupSettingTemplate オブジェクトをすべて一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14f76-116">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="14f76-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14f76-117">Properties</span></span>

| <span data-ttu-id="14f76-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14f76-118">Property</span></span> | <span data-ttu-id="14f76-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="14f76-119">Type</span></span> | <span data-ttu-id="14f76-120">説明</span><span class="sxs-lookup"><span data-stu-id="14f76-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="14f76-121">説明</span><span class="sxs-lookup"><span data-stu-id="14f76-121">description</span></span>|<span data-ttu-id="14f76-122">文字列</span><span class="sxs-lookup"><span data-stu-id="14f76-122">String</span></span>| <span data-ttu-id="14f76-123">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="14f76-123">Description of the template.</span></span> |
|<span data-ttu-id="14f76-124">displayName</span><span class="sxs-lookup"><span data-stu-id="14f76-124">displayName</span></span>|<span data-ttu-id="14f76-125">文字列</span><span class="sxs-lookup"><span data-stu-id="14f76-125">String</span></span>| <span data-ttu-id="14f76-126">テンプレートの表示名です。</span><span class="sxs-lookup"><span data-stu-id="14f76-126">Display name of the template.</span></span> |
|<span data-ttu-id="14f76-127">ID</span><span class="sxs-lookup"><span data-stu-id="14f76-127">id</span></span>|<span data-ttu-id="14f76-128">文字列</span><span class="sxs-lookup"><span data-stu-id="14f76-128">String</span></span>| <span data-ttu-id="14f76-p102">テンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="14f76-p102">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="14f76-131">値</span><span class="sxs-lookup"><span data-stu-id="14f76-131">values</span></span>|<span data-ttu-id="14f76-132">[settingTemplateValue](settingtemplatevalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14f76-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="14f76-133">このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="14f76-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="14f76-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14f76-134">Relationships</span></span>

<span data-ttu-id="14f76-135">なし。</span><span class="sxs-lookup"><span data-stu-id="14f76-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="14f76-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14f76-136">JSON representation</span></span>

<span data-ttu-id="14f76-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14f76-137">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->