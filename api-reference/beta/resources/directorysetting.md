---
title: directorySetting リソースの種類
description: ディレクトリの設定は、使用可能な directorySettingTemplates を基に作成し、事前に設定された既定値から変更できます。 これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。 テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。  たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。 現在定義されているシステムの設定は Office グループの動作を制御するだけ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521370"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="ae425-107">directorySetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae425-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae425-108">ディレクトリの設定は、使用可能な[directorySettingTemplates](directorysettingtemplate.md)、に基づいて作成し、事前に設定された既定値から変更できます。</span><span class="sxs-lookup"><span data-stu-id="ae425-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="ae425-109">これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。</span><span class="sxs-lookup"><span data-stu-id="ae425-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="ae425-110">テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。</span><span class="sxs-lookup"><span data-stu-id="ae425-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="ae425-111">たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。</span><span class="sxs-lookup"><span data-stu-id="ae425-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="ae425-112">現在定義されているシステムの設定は Office グループの動作を制御するだけ。</span><span class="sxs-lookup"><span data-stu-id="ae425-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="ae425-113">**注**: directorySetting リソースの種類の/beta バージョンは、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae425-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="ae425-114">/V1.0 のバージョンは groupSetting に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="ae425-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="ae425-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae425-115">Methods</span></span>

| <span data-ttu-id="ae425-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae425-116">Method</span></span>           | <span data-ttu-id="ae425-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae425-117">Return Type</span></span>    |<span data-ttu-id="ae425-118">説明</span><span class="sxs-lookup"><span data-stu-id="ae425-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae425-119">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="ae425-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="ae425-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="ae425-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="ae425-121">directorySettingTemplate に基づいて、設定オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae425-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="ae425-122">POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae425-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="ae425-123">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="ae425-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="ae425-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="ae425-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="ae425-125">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="ae425-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="ae425-126">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae425-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="ae425-127">[directorySetting](directorysetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae425-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="ae425-128">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ae425-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="ae425-129">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="ae425-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="ae425-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="ae425-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="ae425-131">設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae425-131">Update a setting object.</span></span> <span data-ttu-id="ae425-132">更新プログラムでは、settingValues のみを変更できます。</span><span class="sxs-lookup"><span data-stu-id="ae425-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="ae425-133">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="ae425-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="ae425-134">なし</span><span class="sxs-lookup"><span data-stu-id="ae425-134">None</span></span> |<span data-ttu-id="ae425-135">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="ae425-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae425-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae425-136">Properties</span></span>
| <span data-ttu-id="ae425-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae425-137">Property</span></span>     | <span data-ttu-id="ae425-138">型</span><span class="sxs-lookup"><span data-stu-id="ae425-138">Type</span></span>   |<span data-ttu-id="ae425-139">説明</span><span class="sxs-lookup"><span data-stu-id="ae425-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae425-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ae425-140">displayName</span></span>|<span data-ttu-id="ae425-141">string</span><span class="sxs-lookup"><span data-stu-id="ae425-141">string</span></span>|<span data-ttu-id="ae425-142">関連するテンプレートに由来する設定グループの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="ae425-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="ae425-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae425-143">Read-only.</span></span>|
|<span data-ttu-id="ae425-144">id</span><span class="sxs-lookup"><span data-stu-id="ae425-144">id</span></span>|<span data-ttu-id="ae425-145">文字列</span><span class="sxs-lookup"><span data-stu-id="ae425-145">string</span></span>| <span data-ttu-id="ae425-p107">設定の一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae425-p107">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="ae425-148">templateId</span><span class="sxs-lookup"><span data-stu-id="ae425-148">templateId</span></span>|<span data-ttu-id="ae425-149">string</span><span class="sxs-lookup"><span data-stu-id="ae425-149">string</span></span>| <span data-ttu-id="ae425-p108">設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae425-p108">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="ae425-152">値</span><span class="sxs-lookup"><span data-stu-id="ae425-152">values</span></span>|<span data-ttu-id="ae425-153">[settingValue](settingvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae425-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="ae425-p109">名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae425-p109">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae425-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae425-156">Relationships</span></span>
<span data-ttu-id="ae425-157">None</span><span class="sxs-lookup"><span data-stu-id="ae425-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae425-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae425-158">JSON representation</span></span>

<span data-ttu-id="ae425-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae425-159">Here is a JSON representation of the resource.</span></span>

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
