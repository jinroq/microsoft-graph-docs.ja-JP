---
title: groupsetting リソースの種類
description: グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570828"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="cbd97-103">groupsetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbd97-103">groupSetting resource type</span></span>

<span data-ttu-id="cbd97-104">グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="cbd97-105">グループ設定は、使用可能な[groupsettingtemplates](groupsettingtemplate.md)に基づいて作成し、既定の既定値から変更することができます。</span><span class="sxs-lookup"><span data-stu-id="cbd97-105">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="cbd97-106">これらの設定は、テナント全体レベルまたは特定のグループに対するグループの動作を管理します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-106">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="cbd97-107">テナント全体と特定のグループの両方で同じ設定が定義されている場合、グループレベル設定はテナント全体の設定より優先されます。</span><span class="sxs-lookup"><span data-stu-id="cbd97-107">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="cbd97-108">たとえば、テナント全体の設定では、グループの既存のメンバーによるゲストの招待が許可されることがありますが、個々のグループの設定を上書きして、グループのメンバーに招待されたゲストの招待を許可することはできません。</span><span class="sxs-lookup"><span data-stu-id="cbd97-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="cbd97-109">グループ設定は、Office 365 グループの動作のみを制御します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-109">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="cbd97-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbd97-110">Methods</span></span>

| <span data-ttu-id="cbd97-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbd97-111">Method</span></span> | <span data-ttu-id="cbd97-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbd97-112">Return Type</span></span> | <span data-ttu-id="cbd97-113">説明</span><span class="sxs-lookup"><span data-stu-id="cbd97-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbd97-114">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="cbd97-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="cbd97-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="cbd97-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="cbd97-116">groupsettingtemplate に基づいて設定オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-116">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="cbd97-117">POST 要求は、テンプレートで定義されているすべての設定の settingvalues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbd97-117">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="cbd97-118">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="cbd97-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="cbd97-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="cbd97-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="cbd97-120">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="cbd97-121">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cbd97-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="cbd97-122">[groupSetting](groupsetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbd97-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="cbd97-123">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="cbd97-124">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="cbd97-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="cbd97-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="cbd97-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="cbd97-126">groupsetting オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="cbd97-127">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="cbd97-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="cbd97-128">なし</span><span class="sxs-lookup"><span data-stu-id="cbd97-128">None</span></span> | <span data-ttu-id="cbd97-129">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="cbd97-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cbd97-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd97-130">Properties</span></span>

| <span data-ttu-id="cbd97-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd97-131">Property</span></span> | <span data-ttu-id="cbd97-132">型</span><span class="sxs-lookup"><span data-stu-id="cbd97-132">Type</span></span> | <span data-ttu-id="cbd97-133">説明</span><span class="sxs-lookup"><span data-stu-id="cbd97-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cbd97-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cbd97-134">displayName</span></span>|<span data-ttu-id="cbd97-135">String</span><span class="sxs-lookup"><span data-stu-id="cbd97-135">String</span></span>| <span data-ttu-id="cbd97-136">関連付けられたテンプレートに由来する、この設定グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="cbd97-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="cbd97-137">id</span><span class="sxs-lookup"><span data-stu-id="cbd97-137">id</span></span>|<span data-ttu-id="cbd97-138">String</span><span class="sxs-lookup"><span data-stu-id="cbd97-138">String</span></span>| <span data-ttu-id="cbd97-139">これらの設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="cbd97-139">Unique identifier for these settings.</span></span> <span data-ttu-id="cbd97-140">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cbd97-140">Read-only.</span></span> |
|<span data-ttu-id="cbd97-141">templateId</span><span class="sxs-lookup"><span data-stu-id="cbd97-141">templateId</span></span>|<span data-ttu-id="cbd97-142">String</span><span class="sxs-lookup"><span data-stu-id="cbd97-142">String</span></span>| <span data-ttu-id="cbd97-143">この設定のグループを作成するために使用されるテンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cbd97-143">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="cbd97-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbd97-144">Read-only.</span></span> |
|<span data-ttu-id="cbd97-145">values</span><span class="sxs-lookup"><span data-stu-id="cbd97-145">values</span></span>|<span data-ttu-id="cbd97-146">[settingvalue](settingvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cbd97-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="cbd97-147">名前と値のペアのコレクション。</span><span class="sxs-lookup"><span data-stu-id="cbd97-147">Collection of name value pairs.</span></span> <span data-ttu-id="cbd97-148">テンプレートで定義されているすべての設定が含まれていて、設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbd97-148">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbd97-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbd97-149">Relationships</span></span>

<span data-ttu-id="cbd97-150">なし。</span><span class="sxs-lookup"><span data-stu-id="cbd97-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbd97-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbd97-151">JSON representation</span></span>

<span data-ttu-id="cbd97-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbd97-152">Here is a JSON representation of the resource.</span></span>

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
