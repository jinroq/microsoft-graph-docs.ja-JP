---
title: groupSettingTemplate リソースの種類
description: グループ設定テンプレートは、テナントが使用できるシステム定義の設定を表します。グループ設定は、使用可能な **groupSettingTemplates** に基づいて作成することができ、値は事前設定された既定値から変更することができます。グループ設定テンプレートの作成、更新、削除はできません。これらの設定は、テナント全体の設定または特定のグループ設定を表すことができます。現時点では、利用可能なテンプレートは Office 365 グループのみに適用され、そこでユーザーがグループを作成したり、組織外からゲストをグループのメンバーに招待できるかどうかなどの設定をすることができます。
ms.openlocfilehash: 3c4111b2727e79e048778063b259611795733de4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023768"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="b3e41-107">groupSettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3e41-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="b3e41-p102">グループ設定テンプレートは、テナントが使用できるシステム定義の設定を表します。[グループ設定](groupsetting.md)は、使用可能な **groupSettingTemplates** に基づいて作成することができ、値は事前設定された既定値から変更することができます。グループ設定テンプレートの作成、更新、削除はできません。これらの設定は、テナント全体の設定または特定のグループ設定を表すことができます。現時点では、利用可能なテンプレートは Office 365 グループのみに適用され、そこでユーザーがグループを作成したり、組織外からゲストをグループのメンバーに招待できるかどうかなどの設定をすることができます。</span><span class="sxs-lookup"><span data-stu-id="b3e41-p102">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="b3e41-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3e41-113">Methods</span></span>

| <span data-ttu-id="b3e41-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3e41-114">Method</span></span> | <span data-ttu-id="b3e41-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b3e41-115">Return Type</span></span> | <span data-ttu-id="b3e41-116">説明</span><span class="sxs-lookup"><span data-stu-id="b3e41-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3e41-117">groupSettingTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="b3e41-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="b3e41-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b3e41-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="b3e41-119">システムで定義された groupSettingTemplate オブジェクトの特定のプロパティを読み込みます。</span><span class="sxs-lookup"><span data-stu-id="b3e41-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="b3e41-120">groupSettingTemplate のリスト</span><span class="sxs-lookup"><span data-stu-id="b3e41-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="b3e41-121">GroupSettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="b3e41-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="b3e41-122">システムで定義された groupSettingTemplate オブジェクトをすべて一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b3e41-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3e41-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3e41-123">Properties</span></span>

| <span data-ttu-id="b3e41-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3e41-124">Property</span></span> | <span data-ttu-id="b3e41-125">型</span><span class="sxs-lookup"><span data-stu-id="b3e41-125">Type</span></span> | <span data-ttu-id="b3e41-126">説明</span><span class="sxs-lookup"><span data-stu-id="b3e41-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b3e41-127">説明</span><span class="sxs-lookup"><span data-stu-id="b3e41-127">description</span></span>|<span data-ttu-id="b3e41-128">文字列</span><span class="sxs-lookup"><span data-stu-id="b3e41-128">String</span></span>| <span data-ttu-id="b3e41-129">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="b3e41-129">Description of the template.</span></span> |
|<span data-ttu-id="b3e41-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b3e41-130">displayName</span></span>|<span data-ttu-id="b3e41-131">文字列</span><span class="sxs-lookup"><span data-stu-id="b3e41-131">String</span></span>| <span data-ttu-id="b3e41-132">テンプレートの表示名です。</span><span class="sxs-lookup"><span data-stu-id="b3e41-132">Display name of the template.</span></span> |
|<span data-ttu-id="b3e41-133">id</span><span class="sxs-lookup"><span data-stu-id="b3e41-133">id</span></span>|<span data-ttu-id="b3e41-134">文字列</span><span class="sxs-lookup"><span data-stu-id="b3e41-134">String</span></span>| <span data-ttu-id="b3e41-p103">テンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3e41-p103">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="b3e41-137">値</span><span class="sxs-lookup"><span data-stu-id="b3e41-137">values</span></span>|<span data-ttu-id="b3e41-138">[settingTemplateValue](settingtemplatevalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b3e41-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="b3e41-139">このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b3e41-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b3e41-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3e41-140">Relationships</span></span>

<span data-ttu-id="b3e41-141">なし。</span><span class="sxs-lookup"><span data-stu-id="b3e41-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b3e41-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3e41-142">JSON representation</span></span>

<span data-ttu-id="b3e41-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3e41-143">Here is a JSON representation of the resource.</span></span>

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