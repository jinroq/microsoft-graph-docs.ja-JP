---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b53fc54d4468105eaf5c14039412f03005006a66
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657876"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="2928e-107">directorySettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2928e-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2928e-108">ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="2928e-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="2928e-109">[ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates に基づいて作成でき、値は事前設定の既定値から変更されます。</span><span class="sxs-lookup"><span data-stu-id="2928e-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="2928e-110">ディレクトリ設定テンプレートを作成、更新、または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="2928e-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="2928e-111">これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="2928e-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="2928e-112">現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2928e-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="2928e-113">**注**: directorySettingTemplate リソースの種類の/ベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2928e-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="2928e-114">/V1.0 バージョンの名前が groupSettingTemplate に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2928e-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="2928e-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="2928e-115">Methods</span></span>

| <span data-ttu-id="2928e-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="2928e-116">Method</span></span>           | <span data-ttu-id="2928e-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2928e-117">Return Type</span></span>    |<span data-ttu-id="2928e-118">説明</span><span class="sxs-lookup"><span data-stu-id="2928e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2928e-119">DirectorySettingTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="2928e-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="2928e-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2928e-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="2928e-121">システム定義の directorySettingTemplate オブジェクトのいずれか1つの特定のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2928e-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="2928e-122">DirectorySettingTemplate の一覧表示</span><span class="sxs-lookup"><span data-stu-id="2928e-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="2928e-123">DirectorySettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="2928e-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="2928e-124">システム定義の directorySettingTemplate オブジェクトをすべて一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2928e-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="2928e-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2928e-125">Properties</span></span>
| <span data-ttu-id="2928e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2928e-126">Property</span></span>     | <span data-ttu-id="2928e-127">型</span><span class="sxs-lookup"><span data-stu-id="2928e-127">Type</span></span>   |<span data-ttu-id="2928e-128">説明</span><span class="sxs-lookup"><span data-stu-id="2928e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2928e-129">description</span><span class="sxs-lookup"><span data-stu-id="2928e-129">description</span></span>|<span data-ttu-id="2928e-130">string</span><span class="sxs-lookup"><span data-stu-id="2928e-130">string</span></span>|<span data-ttu-id="2928e-131">テンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="2928e-131">Description of the template.</span></span> <span data-ttu-id="2928e-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2928e-132">Read-only.</span></span>|
|<span data-ttu-id="2928e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2928e-133">displayName</span></span>|<span data-ttu-id="2928e-134">string</span><span class="sxs-lookup"><span data-stu-id="2928e-134">string</span></span>|<span data-ttu-id="2928e-135">テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="2928e-135">Display name of the template.</span></span> <span data-ttu-id="2928e-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2928e-136">Read-only.</span></span> |
|<span data-ttu-id="2928e-137">id</span><span class="sxs-lookup"><span data-stu-id="2928e-137">id</span></span>|<span data-ttu-id="2928e-138">string</span><span class="sxs-lookup"><span data-stu-id="2928e-138">string</span></span>| <span data-ttu-id="2928e-139">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2928e-139">Unique identifier for the template.</span></span> <span data-ttu-id="2928e-140">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2928e-140">Read-only.</span></span>|
|<span data-ttu-id="2928e-141">values</span><span class="sxs-lookup"><span data-stu-id="2928e-141">values</span></span>|<span data-ttu-id="2928e-142">[Settingtemplatevalue](settingtemplatevalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2928e-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="2928e-143">このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2928e-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="2928e-144">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2928e-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2928e-145">関係</span><span class="sxs-lookup"><span data-stu-id="2928e-145">Relationships</span></span>
<span data-ttu-id="2928e-146">なし</span><span class="sxs-lookup"><span data-stu-id="2928e-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2928e-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2928e-147">JSON representation</span></span>

<span data-ttu-id="2928e-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2928e-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
