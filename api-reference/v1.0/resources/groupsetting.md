---
title: groupSetting リソースの種類
description: グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c85b062e955fc15f83728813427f2de5579e297e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030241"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="d2913-103">groupSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2913-103">groupSetting resource type</span></span>

<span data-ttu-id="d2913-104">グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="d2913-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="d2913-105">グループ設定は、使用可能な[Groupsettingtemplates](groupsettingtemplate.md)に基づいて作成し、既定の既定値から変更することができます。</span><span class="sxs-lookup"><span data-stu-id="d2913-105">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="d2913-106">これらの設定は、テナント全体レベルまたは特定のグループに対するグループの動作を管理します。</span><span class="sxs-lookup"><span data-stu-id="d2913-106">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="d2913-107">テナント全体と特定のグループの両方で同じ設定が定義されている場合、グループレベル設定はテナント全体の設定より優先されます。</span><span class="sxs-lookup"><span data-stu-id="d2913-107">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="d2913-108">たとえば、テナント全体の設定では、グループの既存のメンバーによるゲストの招待が許可されることがありますが、個々のグループの設定を上書きして、グループのメンバーに招待されたゲストの招待を許可することはできません。</span><span class="sxs-lookup"><span data-stu-id="d2913-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="d2913-109">グループ設定は、Office 365 グループの動作のみを制御します。</span><span class="sxs-lookup"><span data-stu-id="d2913-109">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="d2913-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2913-110">Methods</span></span>

| <span data-ttu-id="d2913-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2913-111">Method</span></span> | <span data-ttu-id="d2913-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2913-112">Return Type</span></span> | <span data-ttu-id="d2913-113">説明</span><span class="sxs-lookup"><span data-stu-id="d2913-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2913-114">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="d2913-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="d2913-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d2913-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="d2913-116">GroupSettingTemplate に基づいて設定オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2913-116">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="d2913-117">POST 要求は、テンプレートで定義されているすべての設定の settingValues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2913-117">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="d2913-118">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="d2913-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="d2913-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d2913-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="d2913-120">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="d2913-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="d2913-121">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d2913-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="d2913-122">[groupSetting](groupsetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2913-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="d2913-123">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d2913-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="d2913-124">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="d2913-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="d2913-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d2913-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="d2913-126">Groupsetting オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2913-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="d2913-127">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="d2913-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="d2913-128">なし</span><span class="sxs-lookup"><span data-stu-id="d2913-128">None</span></span> | <span data-ttu-id="d2913-129">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d2913-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2913-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2913-130">Properties</span></span>

| <span data-ttu-id="d2913-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2913-131">Property</span></span> | <span data-ttu-id="d2913-132">型</span><span class="sxs-lookup"><span data-stu-id="d2913-132">Type</span></span> | <span data-ttu-id="d2913-133">説明</span><span class="sxs-lookup"><span data-stu-id="d2913-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d2913-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d2913-134">displayName</span></span>|<span data-ttu-id="d2913-135">String</span><span class="sxs-lookup"><span data-stu-id="d2913-135">String</span></span>| <span data-ttu-id="d2913-136">関連付けられたテンプレートに由来する、この設定グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="d2913-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="d2913-137">id</span><span class="sxs-lookup"><span data-stu-id="d2913-137">id</span></span>|<span data-ttu-id="d2913-138">文字列</span><span class="sxs-lookup"><span data-stu-id="d2913-138">String</span></span>| <span data-ttu-id="d2913-139">これらの設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="d2913-139">Unique identifier for these settings.</span></span> <span data-ttu-id="d2913-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d2913-140">Read-only.</span></span> |
|<span data-ttu-id="d2913-141">templateId</span><span class="sxs-lookup"><span data-stu-id="d2913-141">templateId</span></span>|<span data-ttu-id="d2913-142">String</span><span class="sxs-lookup"><span data-stu-id="d2913-142">String</span></span>| <span data-ttu-id="d2913-143">この設定のグループを作成するために使用されるテンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d2913-143">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="d2913-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d2913-144">Read-only.</span></span> |
|<span data-ttu-id="d2913-145">values</span><span class="sxs-lookup"><span data-stu-id="d2913-145">values</span></span>|<span data-ttu-id="d2913-146">[Settingvalue](settingvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2913-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="d2913-147">名前と値のペアのコレクション。</span><span class="sxs-lookup"><span data-stu-id="d2913-147">Collection of name value pairs.</span></span> <span data-ttu-id="d2913-148">テンプレートで定義されているすべての設定が含まれていて、設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2913-148">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d2913-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2913-149">Relationships</span></span>

<span data-ttu-id="d2913-150">なし。</span><span class="sxs-lookup"><span data-stu-id="d2913-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2913-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2913-151">JSON representation</span></span>

<span data-ttu-id="d2913-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2913-152">Here is a JSON representation of the resource.</span></span>

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
