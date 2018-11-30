---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。
ms.openlocfilehash: fa4906aa58805e6d1a027973f61b5d68ed47f2c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066775"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="324b0-107">directorySettingTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="324b0-107">directorySettingTemplate resource type</span></span>

> <span data-ttu-id="324b0-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="324b0-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="324b0-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="324b0-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="324b0-110">ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="324b0-110">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="324b0-111">[ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。</span><span class="sxs-lookup"><span data-stu-id="324b0-111">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="324b0-112">ディレクトリ設定のテンプレートを作成、更新または削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="324b0-112">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="324b0-113">これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="324b0-113">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="324b0-114">現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="324b0-114">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="324b0-115">**注**: directorySettingTemplate リソースの種類の/beta バージョンは、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="324b0-115">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="324b0-116">/V1.0 のバージョンは groupSettingTemplate に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="324b0-116">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="324b0-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="324b0-117">Methods</span></span>

| <span data-ttu-id="324b0-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="324b0-118">Method</span></span>           | <span data-ttu-id="324b0-119">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="324b0-119">Return Type</span></span>    |<span data-ttu-id="324b0-120">説明</span><span class="sxs-lookup"><span data-stu-id="324b0-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="324b0-121">DirectorySettingTemplate を取得します。</span><span class="sxs-lookup"><span data-stu-id="324b0-121">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="324b0-122">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="324b0-122">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="324b0-123">システム定義の directorySettingTemplate オブジェクトの 1 つの特定のプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="324b0-123">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="324b0-124">リスト directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="324b0-124">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="324b0-125">DirectorySettingTemplate のコレクション</span><span class="sxs-lookup"><span data-stu-id="324b0-125">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="324b0-126">すべてのシステム定義の directorySettingTemplate オブジェクトの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="324b0-126">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="324b0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="324b0-127">Properties</span></span>
| <span data-ttu-id="324b0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="324b0-128">Property</span></span>     | <span data-ttu-id="324b0-129">型</span><span class="sxs-lookup"><span data-stu-id="324b0-129">Type</span></span>   |<span data-ttu-id="324b0-130">説明</span><span class="sxs-lookup"><span data-stu-id="324b0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="324b0-131">description</span><span class="sxs-lookup"><span data-stu-id="324b0-131">description</span></span>|<span data-ttu-id="324b0-132">文字列</span><span class="sxs-lookup"><span data-stu-id="324b0-132">string</span></span>|<span data-ttu-id="324b0-133">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="324b0-133">Description of the template.</span></span> <span data-ttu-id="324b0-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="324b0-134">Read-only.</span></span>|
|<span data-ttu-id="324b0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="324b0-135">displayName</span></span>|<span data-ttu-id="324b0-136">string</span><span class="sxs-lookup"><span data-stu-id="324b0-136">string</span></span>|<span data-ttu-id="324b0-137">テンプレートの表示名です。</span><span class="sxs-lookup"><span data-stu-id="324b0-137">Display name of the template.</span></span> <span data-ttu-id="324b0-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="324b0-138">Read-only.</span></span> |
|<span data-ttu-id="324b0-139">ID</span><span class="sxs-lookup"><span data-stu-id="324b0-139">id</span></span>|<span data-ttu-id="324b0-140">文字列</span><span class="sxs-lookup"><span data-stu-id="324b0-140">string</span></span>| <span data-ttu-id="324b0-p107">テンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="324b0-p107">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="324b0-143">値</span><span class="sxs-lookup"><span data-stu-id="324b0-143">values</span></span>|<span data-ttu-id="324b0-144">[settingTemplateValue](settingtemplatevalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="324b0-144">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="324b0-145">このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="324b0-145">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="324b0-146">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="324b0-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="324b0-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="324b0-147">Relationships</span></span>
<span data-ttu-id="324b0-148">なし</span><span class="sxs-lookup"><span data-stu-id="324b0-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="324b0-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="324b0-149">JSON representation</span></span>

<span data-ttu-id="324b0-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="324b0-150">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->