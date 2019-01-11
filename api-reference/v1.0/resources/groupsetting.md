---
title: groupSetting リソースの種類
description: グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4508de9c03820031e47e3457e24dc39ed14c36a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840769"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="9bfff-103">groupSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9bfff-103">groupSetting resource type</span></span>

<span data-ttu-id="9bfff-104">グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="9bfff-p101">グループ設定は、使用可能な [groupSettingTemplates](groupsettingtemplate.md) に基づいて作成することができ、事前設定された既定値を変更することができます。これらの設定は、テナント全体のレベルまたは特定のグループのグループ基本動作を制御します。テナント全体および特定のグループの両方で同じ設定が定義されている場合、グループ レベルの設定がテナント全体の設定よりも優先されます。たとえば、テナント全体の設定では、ゲストは既存のグループのメンバーによって招待されることがありますが、個別のグループ設定を優先することができ、その場合は、グループのメンバーはゲストを招待することができません。グループ設定は、Office 365 グループの動作のみを制御します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-p101">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="9bfff-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="9bfff-110">Methods</span></span>

| <span data-ttu-id="9bfff-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9bfff-111">Method</span></span> | <span data-ttu-id="9bfff-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9bfff-112">Return Type</span></span> | <span data-ttu-id="9bfff-113">説明</span><span class="sxs-lookup"><span data-stu-id="9bfff-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bfff-114">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="9bfff-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="9bfff-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="9bfff-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="9bfff-p102">groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9bfff-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="9bfff-118">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="9bfff-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="9bfff-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="9bfff-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="9bfff-120">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="9bfff-121">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9bfff-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="9bfff-122">[groupSetting](groupsetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9bfff-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="9bfff-123">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="9bfff-124">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="9bfff-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="9bfff-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="9bfff-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="9bfff-126">Groupsetting オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="9bfff-127">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="9bfff-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="9bfff-128">なし</span><span class="sxs-lookup"><span data-stu-id="9bfff-128">None</span></span> | <span data-ttu-id="9bfff-129">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9bfff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9bfff-130">Properties</span></span>

| <span data-ttu-id="9bfff-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9bfff-131">Property</span></span> | <span data-ttu-id="9bfff-132">種類</span><span class="sxs-lookup"><span data-stu-id="9bfff-132">Type</span></span> | <span data-ttu-id="9bfff-133">説明</span><span class="sxs-lookup"><span data-stu-id="9bfff-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9bfff-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9bfff-134">displayName</span></span>|<span data-ttu-id="9bfff-135">文字列</span><span class="sxs-lookup"><span data-stu-id="9bfff-135">String</span></span>| <span data-ttu-id="9bfff-136">関連するテンプレートに由来する設定グループの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="9bfff-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="9bfff-137">id</span><span class="sxs-lookup"><span data-stu-id="9bfff-137">id</span></span>|<span data-ttu-id="9bfff-138">文字列</span><span class="sxs-lookup"><span data-stu-id="9bfff-138">String</span></span>| <span data-ttu-id="9bfff-p103">設定の一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="9bfff-141">templateId</span><span class="sxs-lookup"><span data-stu-id="9bfff-141">templateId</span></span>|<span data-ttu-id="9bfff-142">文字列</span><span class="sxs-lookup"><span data-stu-id="9bfff-142">String</span></span>| <span data-ttu-id="9bfff-p104">設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="9bfff-145">値</span><span class="sxs-lookup"><span data-stu-id="9bfff-145">values</span></span>|<span data-ttu-id="9bfff-146">[settingValue](settingvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9bfff-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="9bfff-p105">名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="9bfff-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9bfff-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9bfff-149">Relationships</span></span>

<span data-ttu-id="9bfff-150">なし。</span><span class="sxs-lookup"><span data-stu-id="9bfff-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bfff-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9bfff-151">JSON representation</span></span>

<span data-ttu-id="9bfff-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9bfff-152">Here is a JSON representation of the resource.</span></span>

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
