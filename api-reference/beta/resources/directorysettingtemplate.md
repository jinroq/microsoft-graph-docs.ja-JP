---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516659"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="841b7-107">directorySettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="841b7-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="841b7-108">ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="841b7-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="841b7-109">[ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。</span><span class="sxs-lookup"><span data-stu-id="841b7-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="841b7-110">ディレクトリ設定のテンプレートを作成、更新または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="841b7-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="841b7-111">これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="841b7-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="841b7-112">現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="841b7-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="841b7-113">**注**: directorySettingTemplate リソースの種類の/beta バージョンは、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="841b7-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="841b7-114">/V1.0 のバージョンは groupSettingTemplate に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="841b7-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="841b7-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="841b7-115">Methods</span></span>

| <span data-ttu-id="841b7-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="841b7-116">Method</span></span>           | <span data-ttu-id="841b7-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="841b7-117">Return Type</span></span>    |<span data-ttu-id="841b7-118">説明</span><span class="sxs-lookup"><span data-stu-id="841b7-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="841b7-119">DirectorySettingTemplate を取得します。</span><span class="sxs-lookup"><span data-stu-id="841b7-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="841b7-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="841b7-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="841b7-121">システム定義の directorySettingTemplate オブジェクトの 1 つの特定のプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="841b7-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="841b7-122">リスト directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="841b7-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="841b7-123">DirectorySettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="841b7-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="841b7-124">すべてのシステム定義の directorySettingTemplate オブジェクトの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="841b7-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="841b7-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="841b7-125">Properties</span></span>
| <span data-ttu-id="841b7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="841b7-126">Property</span></span>     | <span data-ttu-id="841b7-127">型</span><span class="sxs-lookup"><span data-stu-id="841b7-127">Type</span></span>   |<span data-ttu-id="841b7-128">説明</span><span class="sxs-lookup"><span data-stu-id="841b7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="841b7-129">説明</span><span class="sxs-lookup"><span data-stu-id="841b7-129">description</span></span>|<span data-ttu-id="841b7-130">string</span><span class="sxs-lookup"><span data-stu-id="841b7-130">string</span></span>|<span data-ttu-id="841b7-131">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="841b7-131">Description of the template.</span></span> <span data-ttu-id="841b7-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="841b7-132">Read-only.</span></span>|
|<span data-ttu-id="841b7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="841b7-133">displayName</span></span>|<span data-ttu-id="841b7-134">string</span><span class="sxs-lookup"><span data-stu-id="841b7-134">string</span></span>|<span data-ttu-id="841b7-135">テンプレートの表示名です。</span><span class="sxs-lookup"><span data-stu-id="841b7-135">Display name of the template.</span></span> <span data-ttu-id="841b7-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="841b7-136">Read-only.</span></span> |
|<span data-ttu-id="841b7-137">id</span><span class="sxs-lookup"><span data-stu-id="841b7-137">id</span></span>|<span data-ttu-id="841b7-138">文字列</span><span class="sxs-lookup"><span data-stu-id="841b7-138">string</span></span>| <span data-ttu-id="841b7-p106">テンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="841b7-p106">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="841b7-141">値</span><span class="sxs-lookup"><span data-stu-id="841b7-141">values</span></span>|<span data-ttu-id="841b7-142">[settingTemplateValue](settingtemplatevalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="841b7-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="841b7-143">このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="841b7-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="841b7-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="841b7-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="841b7-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="841b7-145">Relationships</span></span>
<span data-ttu-id="841b7-146">なし</span><span class="sxs-lookup"><span data-stu-id="841b7-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="841b7-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="841b7-147">JSON representation</span></span>

<span data-ttu-id="841b7-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="841b7-148">Here is a JSON representation of the resource.</span></span>

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
