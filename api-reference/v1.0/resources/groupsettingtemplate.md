---
title: groupSettingTemplate リソースの種類
description: グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**Groupsettingtemplates**に基づいてグループ設定を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d0624be1511b542da08e76ed5f9c51e60fe58a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029282"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="ad3a6-107">groupSettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad3a6-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="ad3a6-108">グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-108">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="ad3a6-109">使用可能な**Groupsettingtemplates**に基づいて[グループ設定](groupsetting.md)を作成し、既定の既定値から変更された値を作成できます。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-109">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="ad3a6-110">グループ設定テンプレートを作成、更新、または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-110">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="ad3a6-111">これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-111">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="ad3a6-112">現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-112">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="ad3a6-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad3a6-113">Methods</span></span>

| <span data-ttu-id="ad3a6-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad3a6-114">Method</span></span> | <span data-ttu-id="ad3a6-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ad3a6-115">Return Type</span></span> | <span data-ttu-id="ad3a6-116">説明</span><span class="sxs-lookup"><span data-stu-id="ad3a6-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad3a6-117">GroupSettingTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="ad3a6-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="ad3a6-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="ad3a6-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="ad3a6-119">システム定義のいずれかの groupSettingTemplate オブジェクトの特定のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="ad3a6-120">GroupSettingTemplate の一覧表示</span><span class="sxs-lookup"><span data-stu-id="ad3a6-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="ad3a6-121">GroupSettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="ad3a6-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="ad3a6-122">システム定義のすべての groupSettingTemplate オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad3a6-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad3a6-123">Properties</span></span>

| <span data-ttu-id="ad3a6-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad3a6-124">Property</span></span> | <span data-ttu-id="ad3a6-125">型</span><span class="sxs-lookup"><span data-stu-id="ad3a6-125">Type</span></span> | <span data-ttu-id="ad3a6-126">説明</span><span class="sxs-lookup"><span data-stu-id="ad3a6-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ad3a6-127">description</span><span class="sxs-lookup"><span data-stu-id="ad3a6-127">description</span></span>|<span data-ttu-id="ad3a6-128">String</span><span class="sxs-lookup"><span data-stu-id="ad3a6-128">String</span></span>| <span data-ttu-id="ad3a6-129">テンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-129">Description of the template.</span></span> |
|<span data-ttu-id="ad3a6-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ad3a6-130">displayName</span></span>|<span data-ttu-id="ad3a6-131">String</span><span class="sxs-lookup"><span data-stu-id="ad3a6-131">String</span></span>| <span data-ttu-id="ad3a6-132">テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-132">Display name of the template.</span></span> |
|<span data-ttu-id="ad3a6-133">id</span><span class="sxs-lookup"><span data-stu-id="ad3a6-133">id</span></span>|<span data-ttu-id="ad3a6-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ad3a6-134">String</span></span>| <span data-ttu-id="ad3a6-135">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-135">Unique identifier for the template.</span></span> <span data-ttu-id="ad3a6-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-136">Read-only.</span></span>|
|<span data-ttu-id="ad3a6-137">values</span><span class="sxs-lookup"><span data-stu-id="ad3a6-137">values</span></span>|<span data-ttu-id="ad3a6-138">[Settingtemplatevalue](settingtemplatevalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ad3a6-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="ad3a6-139">このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ad3a6-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad3a6-140">Relationships</span></span>

<span data-ttu-id="ad3a6-141">なし。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad3a6-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad3a6-142">JSON representation</span></span>

<span data-ttu-id="ad3a6-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad3a6-143">Here is a JSON representation of the resource.</span></span>

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
