---
title: directorysettingtemplate リソースの種類
description: ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorysettingtemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543253"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="eaea2-107">directorysettingtemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eaea2-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaea2-108">ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="eaea2-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="eaea2-109">[ディレクトリの設定](directorysetting.md)は、使用可能な directorysettingtemplates に基づいて作成でき、値は事前設定の既定値から変更されます。</span><span class="sxs-lookup"><span data-stu-id="eaea2-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="eaea2-110">ディレクトリ設定テンプレートを作成、更新、または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="eaea2-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="eaea2-111">これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="eaea2-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="eaea2-112">現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eaea2-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="eaea2-113">**注**: directorysettingtemplate リソースの種類の/ベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="eaea2-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="eaea2-114">/v1.0 バージョンの名前が groupsettingtemplate に変更されました。</span><span class="sxs-lookup"><span data-stu-id="eaea2-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="eaea2-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="eaea2-115">Methods</span></span>

| <span data-ttu-id="eaea2-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="eaea2-116">Method</span></span>           | <span data-ttu-id="eaea2-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eaea2-117">Return Type</span></span>    |<span data-ttu-id="eaea2-118">説明</span><span class="sxs-lookup"><span data-stu-id="eaea2-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eaea2-119">directorysettingtemplate の取得</span><span class="sxs-lookup"><span data-stu-id="eaea2-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="eaea2-120">directorysettingtemplate</span><span class="sxs-lookup"><span data-stu-id="eaea2-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="eaea2-121">システム定義の directorysettingtemplate オブジェクトのいずれか1つの特定のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="eaea2-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="eaea2-122">directorysettingtemplate の一覧表示</span><span class="sxs-lookup"><span data-stu-id="eaea2-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="eaea2-123">directorysettingtemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="eaea2-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="eaea2-124">システム定義の directorysettingtemplate オブジェクトをすべて一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="eaea2-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="eaea2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eaea2-125">Properties</span></span>
| <span data-ttu-id="eaea2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eaea2-126">Property</span></span>     | <span data-ttu-id="eaea2-127">型</span><span class="sxs-lookup"><span data-stu-id="eaea2-127">Type</span></span>   |<span data-ttu-id="eaea2-128">説明</span><span class="sxs-lookup"><span data-stu-id="eaea2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaea2-129">description</span><span class="sxs-lookup"><span data-stu-id="eaea2-129">description</span></span>|<span data-ttu-id="eaea2-130">string</span><span class="sxs-lookup"><span data-stu-id="eaea2-130">string</span></span>|<span data-ttu-id="eaea2-131">テンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="eaea2-131">Description of the template.</span></span> <span data-ttu-id="eaea2-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eaea2-132">Read-only.</span></span>|
|<span data-ttu-id="eaea2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eaea2-133">displayName</span></span>|<span data-ttu-id="eaea2-134">string</span><span class="sxs-lookup"><span data-stu-id="eaea2-134">string</span></span>|<span data-ttu-id="eaea2-135">テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="eaea2-135">Display name of the template.</span></span> <span data-ttu-id="eaea2-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="eaea2-136">Read-only.</span></span> |
|<span data-ttu-id="eaea2-137">id</span><span class="sxs-lookup"><span data-stu-id="eaea2-137">id</span></span>|<span data-ttu-id="eaea2-138">string</span><span class="sxs-lookup"><span data-stu-id="eaea2-138">string</span></span>| <span data-ttu-id="eaea2-139">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="eaea2-139">Unique identifier for the template.</span></span> <span data-ttu-id="eaea2-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eaea2-140">Read-only.</span></span>|
|<span data-ttu-id="eaea2-141">values</span><span class="sxs-lookup"><span data-stu-id="eaea2-141">values</span></span>|<span data-ttu-id="eaea2-142">[settingtemplatevalue](settingtemplatevalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="eaea2-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="eaea2-143">このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingtemplatevalues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="eaea2-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="eaea2-144">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="eaea2-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eaea2-145">関係</span><span class="sxs-lookup"><span data-stu-id="eaea2-145">Relationships</span></span>
<span data-ttu-id="eaea2-146">なし</span><span class="sxs-lookup"><span data-stu-id="eaea2-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="eaea2-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eaea2-147">JSON representation</span></span>

<span data-ttu-id="eaea2-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eaea2-148">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
