---
title: groupsettingtemplate リソースの種類
description: グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**groupsettingtemplates**に基づいてグループ設定を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570793"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="41f8f-107">groupsettingtemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41f8f-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="41f8f-108">グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="41f8f-108">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="41f8f-109">使用可能な**groupsettingtemplates**に基づいて[グループ設定](groupsetting.md)を作成し、既定の既定値から変更された値を作成できます。</span><span class="sxs-lookup"><span data-stu-id="41f8f-109">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="41f8f-110">グループ設定テンプレートを作成、更新、または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="41f8f-110">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="41f8f-111">これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="41f8f-111">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="41f8f-112">現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="41f8f-112">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="41f8f-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="41f8f-113">Methods</span></span>

| <span data-ttu-id="41f8f-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="41f8f-114">Method</span></span> | <span data-ttu-id="41f8f-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41f8f-115">Return Type</span></span> | <span data-ttu-id="41f8f-116">説明</span><span class="sxs-lookup"><span data-stu-id="41f8f-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="41f8f-117">groupsettingtemplate の取得</span><span class="sxs-lookup"><span data-stu-id="41f8f-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="41f8f-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="41f8f-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="41f8f-119">システム定義のいずれかの groupsettingtemplate オブジェクトの特定のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="41f8f-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="41f8f-120">groupsettingtemplate の一覧表示</span><span class="sxs-lookup"><span data-stu-id="41f8f-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="41f8f-121">groupsettingtemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="41f8f-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="41f8f-122">システム定義のすべての groupsettingtemplate オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="41f8f-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="41f8f-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41f8f-123">Properties</span></span>

| <span data-ttu-id="41f8f-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41f8f-124">Property</span></span> | <span data-ttu-id="41f8f-125">型</span><span class="sxs-lookup"><span data-stu-id="41f8f-125">Type</span></span> | <span data-ttu-id="41f8f-126">説明</span><span class="sxs-lookup"><span data-stu-id="41f8f-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="41f8f-127">description</span><span class="sxs-lookup"><span data-stu-id="41f8f-127">description</span></span>|<span data-ttu-id="41f8f-128">String</span><span class="sxs-lookup"><span data-stu-id="41f8f-128">String</span></span>| <span data-ttu-id="41f8f-129">テンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="41f8f-129">Description of the template.</span></span> |
|<span data-ttu-id="41f8f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="41f8f-130">displayName</span></span>|<span data-ttu-id="41f8f-131">String</span><span class="sxs-lookup"><span data-stu-id="41f8f-131">String</span></span>| <span data-ttu-id="41f8f-132">テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="41f8f-132">Display name of the template.</span></span> |
|<span data-ttu-id="41f8f-133">id</span><span class="sxs-lookup"><span data-stu-id="41f8f-133">id</span></span>|<span data-ttu-id="41f8f-134">String</span><span class="sxs-lookup"><span data-stu-id="41f8f-134">String</span></span>| <span data-ttu-id="41f8f-135">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="41f8f-135">Unique identifier for the template.</span></span> <span data-ttu-id="41f8f-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41f8f-136">Read-only.</span></span>|
|<span data-ttu-id="41f8f-137">values</span><span class="sxs-lookup"><span data-stu-id="41f8f-137">values</span></span>|<span data-ttu-id="41f8f-138">[settingtemplatevalue](settingtemplatevalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41f8f-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="41f8f-139">このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingtemplatevalues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="41f8f-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="41f8f-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41f8f-140">Relationships</span></span>

<span data-ttu-id="41f8f-141">なし。</span><span class="sxs-lookup"><span data-stu-id="41f8f-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="41f8f-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41f8f-142">JSON representation</span></span>

<span data-ttu-id="41f8f-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41f8f-143">Here is a JSON representation of the resource.</span></span>

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
