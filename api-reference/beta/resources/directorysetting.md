---
title: directorySetting リソースの種類
description: ディレクトリの設定は、使用可能な directorySettingTemplates を基に作成し、事前に設定された既定値から変更できます。 これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。 テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。  たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。 現在定義されているシステムの設定は Office グループの動作を制御するだけ。
localization_priority: Normal
ms.openlocfilehash: 2687df732896abfb8ecf3b0651682228b84fa17b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810139"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="84c2a-107">directorySetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84c2a-107">directorySetting resource type</span></span>

> <span data-ttu-id="84c2a-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84c2a-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84c2a-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84c2a-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84c2a-110">ディレクトリの設定は、使用可能な[directorySettingTemplates](directorysettingtemplate.md)、に基づいて作成し、事前に設定された既定値から変更できます。</span><span class="sxs-lookup"><span data-stu-id="84c2a-110">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="84c2a-111">これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。</span><span class="sxs-lookup"><span data-stu-id="84c2a-111">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="84c2a-112">テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。</span><span class="sxs-lookup"><span data-stu-id="84c2a-112">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="84c2a-113">たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。</span><span class="sxs-lookup"><span data-stu-id="84c2a-113">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="84c2a-114">現在定義されているシステムの設定は Office グループの動作を制御するだけ。</span><span class="sxs-lookup"><span data-stu-id="84c2a-114">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="84c2a-115">**注**: directorySetting リソースの種類の/beta バージョンは、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="84c2a-115">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="84c2a-116">/V1.0 のバージョンは groupSetting に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="84c2a-116">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="84c2a-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="84c2a-117">Methods</span></span>

| <span data-ttu-id="84c2a-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="84c2a-118">Method</span></span>           | <span data-ttu-id="84c2a-119">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="84c2a-119">Return Type</span></span>    |<span data-ttu-id="84c2a-120">説明</span><span class="sxs-lookup"><span data-stu-id="84c2a-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84c2a-121">設定を作成する</span><span class="sxs-lookup"><span data-stu-id="84c2a-121">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="84c2a-122">directorySetting</span><span class="sxs-lookup"><span data-stu-id="84c2a-122">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="84c2a-123">DirectorySettingTemplate に基づいて、設定オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-123">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="84c2a-124">POST 要求は、テンプレートで定義されているすべての設定 settingValues を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="84c2a-124">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="84c2a-125">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="84c2a-125">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="84c2a-126">directorySetting</span><span class="sxs-lookup"><span data-stu-id="84c2a-126">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="84c2a-127">特定の設定オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-127">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="84c2a-128">設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="84c2a-128">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="84c2a-129">[directorySetting](directorysetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="84c2a-129">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="84c2a-130">すべての設定オブジェクトのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-130">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="84c2a-131">設定を更新する</span><span class="sxs-lookup"><span data-stu-id="84c2a-131">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="84c2a-132">directorySetting</span><span class="sxs-lookup"><span data-stu-id="84c2a-132">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="84c2a-133">設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-133">Update a setting object.</span></span> <span data-ttu-id="84c2a-134">更新プログラムでは、settingValues のみを変更できます。</span><span class="sxs-lookup"><span data-stu-id="84c2a-134">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="84c2a-135">設定を削除する</span><span class="sxs-lookup"><span data-stu-id="84c2a-135">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="84c2a-136">なし</span><span class="sxs-lookup"><span data-stu-id="84c2a-136">None</span></span> |<span data-ttu-id="84c2a-137">設定オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-137">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="84c2a-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84c2a-138">Properties</span></span>
| <span data-ttu-id="84c2a-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84c2a-139">Property</span></span>     | <span data-ttu-id="84c2a-140">種類</span><span class="sxs-lookup"><span data-stu-id="84c2a-140">Type</span></span>   |<span data-ttu-id="84c2a-141">説明</span><span class="sxs-lookup"><span data-stu-id="84c2a-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84c2a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="84c2a-142">displayName</span></span>|<span data-ttu-id="84c2a-143">string</span><span class="sxs-lookup"><span data-stu-id="84c2a-143">string</span></span>|<span data-ttu-id="84c2a-144">関連するテンプレートに由来する設定グループの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="84c2a-144">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="84c2a-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="84c2a-145">Read-only.</span></span>|
|<span data-ttu-id="84c2a-146">ID</span><span class="sxs-lookup"><span data-stu-id="84c2a-146">id</span></span>|<span data-ttu-id="84c2a-147">文字列</span><span class="sxs-lookup"><span data-stu-id="84c2a-147">string</span></span>| <span data-ttu-id="84c2a-p108">設定の一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="84c2a-p108">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="84c2a-150">templateId</span><span class="sxs-lookup"><span data-stu-id="84c2a-150">templateId</span></span>|<span data-ttu-id="84c2a-151">文字列</span><span class="sxs-lookup"><span data-stu-id="84c2a-151">string</span></span>| <span data-ttu-id="84c2a-p109">設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="84c2a-p109">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="84c2a-154">値</span><span class="sxs-lookup"><span data-stu-id="84c2a-154">values</span></span>|<span data-ttu-id="84c2a-155">[settingValue](settingvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84c2a-155">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="84c2a-p110">名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="84c2a-p110">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84c2a-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84c2a-158">Relationships</span></span>
<span data-ttu-id="84c2a-159">なし</span><span class="sxs-lookup"><span data-stu-id="84c2a-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="84c2a-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84c2a-160">JSON representation</span></span>

<span data-ttu-id="84c2a-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84c2a-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
