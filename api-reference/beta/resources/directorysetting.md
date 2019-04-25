---
title: directorysetting リソースの種類
description: ディレクトリの設定は、使用可能な directorysettingtemplates に基づいて作成し、既定の既定値から変更することができます。 これらの設定は、テナント全体レベルまたは特定のエンティティレベルで、エンティティまたは機能の動作を制御できます。 テナント全体と特定のエンティティレベルの両方で同じ設定が定義されている場合、特定のエンティティレベルの設定はテナント全体の設定から除外されることがあります。  たとえば、テナント全体の設定では、ゲストがグループの既存のメンバーに招待されることが許可されますが、特定のグループの設定はオプトアウトされ、グループのメンバーによるゲストの招待が許可されない場合があります。 現在、システムで定義されている設定は、Office グループの動作のみを制御します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535240"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="bd1a0-107">directorysetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd1a0-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd1a0-108">ディレクトリの設定は、使用可能な[directorysettingtemplates](directorysettingtemplate.md)に基づいて作成し、既定の既定値から変更することができます。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="bd1a0-109">これらの設定は、テナント全体レベルまたは特定のエンティティレベルで、エンティティまたは機能の動作を制御できます。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="bd1a0-110">テナント全体と特定のエンティティレベルの両方で同じ設定が定義されている場合、特定のエンティティレベルの設定はテナント全体の設定から除外されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="bd1a0-111">たとえば、テナント全体の設定では、ゲストがグループの既存のメンバーに招待されることが許可されますが、特定のグループの設定はオプトアウトされ、グループのメンバーによるゲストの招待が許可されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="bd1a0-112">現在、システムで定義されている設定は、Office グループの動作のみを制御します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="bd1a0-113">**注**: directorysetting リソースの種類の/ベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="bd1a0-114">/v1.0 のバージョンが groupsetting に変更されました。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="bd1a0-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd1a0-115">Methods</span></span>

| <span data-ttu-id="bd1a0-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd1a0-116">Method</span></span>           | <span data-ttu-id="bd1a0-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bd1a0-117">Return Type</span></span>    |<span data-ttu-id="bd1a0-118">説明</span><span class="sxs-lookup"><span data-stu-id="bd1a0-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd1a0-119">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="bd1a0-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="bd1a0-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bd1a0-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bd1a0-121">directorysettingtemplate に基づいて設定オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="bd1a0-122">POST 要求は、テンプレートで定義されているすべての設定の settingvalues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="bd1a0-123">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="bd1a0-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="bd1a0-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bd1a0-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bd1a0-125">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="bd1a0-126">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bd1a0-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="bd1a0-127">[directorySetting](directorysetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd1a0-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="bd1a0-128">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="bd1a0-129">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="bd1a0-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="bd1a0-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bd1a0-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="bd1a0-131">設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-131">Update a setting object.</span></span> <span data-ttu-id="bd1a0-132">update で変更できるのは、設定値だけです。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="bd1a0-133">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="bd1a0-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="bd1a0-134">なし</span><span class="sxs-lookup"><span data-stu-id="bd1a0-134">None</span></span> |<span data-ttu-id="bd1a0-135">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd1a0-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd1a0-136">Properties</span></span>
| <span data-ttu-id="bd1a0-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd1a0-137">Property</span></span>     | <span data-ttu-id="bd1a0-138">型</span><span class="sxs-lookup"><span data-stu-id="bd1a0-138">Type</span></span>   |<span data-ttu-id="bd1a0-139">説明</span><span class="sxs-lookup"><span data-stu-id="bd1a0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd1a0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bd1a0-140">displayName</span></span>|<span data-ttu-id="bd1a0-141">string</span><span class="sxs-lookup"><span data-stu-id="bd1a0-141">string</span></span>|<span data-ttu-id="bd1a0-142">関連付けられたテンプレートに由来する、この設定グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="bd1a0-143">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-143">Read-only.</span></span>|
|<span data-ttu-id="bd1a0-144">id</span><span class="sxs-lookup"><span data-stu-id="bd1a0-144">id</span></span>|<span data-ttu-id="bd1a0-145">string</span><span class="sxs-lookup"><span data-stu-id="bd1a0-145">string</span></span>| <span data-ttu-id="bd1a0-146">これらの設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-146">Unique identifier for these settings.</span></span> <span data-ttu-id="bd1a0-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-147">Read-only.</span></span>|
|<span data-ttu-id="bd1a0-148">templateId</span><span class="sxs-lookup"><span data-stu-id="bd1a0-148">templateId</span></span>|<span data-ttu-id="bd1a0-149">string</span><span class="sxs-lookup"><span data-stu-id="bd1a0-149">string</span></span>| <span data-ttu-id="bd1a0-150">この設定のグループを作成するために使用されるテンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-150">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="bd1a0-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-151">Read-only.</span></span>|
|<span data-ttu-id="bd1a0-152">values</span><span class="sxs-lookup"><span data-stu-id="bd1a0-152">values</span></span>|<span data-ttu-id="bd1a0-153">[settingvalue](settingvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd1a0-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="bd1a0-154">名前と値のペアのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-154">Collection of name value pairs.</span></span> <span data-ttu-id="bd1a0-155">テンプレートで定義されているすべての設定が含まれていて、設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-155">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd1a0-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd1a0-156">Relationships</span></span>
<span data-ttu-id="bd1a0-157">なし</span><span class="sxs-lookup"><span data-stu-id="bd1a0-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd1a0-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd1a0-158">JSON representation</span></span>

<span data-ttu-id="bd1a0-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd1a0-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
