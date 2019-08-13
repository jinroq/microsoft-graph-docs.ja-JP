---
title: deviceManagementTemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e2c7536c61bfaf8287a0a2428e0b861e09f3a5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337623"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="ef89f-103">deviceManagementTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef89f-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="ef89f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef89f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef89f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef89f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef89f-106">デバイス設定の定義済みコレクションを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="ef89f-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="ef89f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef89f-107">Methods</span></span>
|<span data-ttu-id="ef89f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef89f-108">Method</span></span>|<span data-ttu-id="ef89f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef89f-109">Return Type</span></span>|<span data-ttu-id="ef89f-110">説明</span><span class="sxs-lookup"><span data-stu-id="ef89f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ef89f-111">DeviceManagementTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ef89f-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="ef89f-112">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="ef89f-113">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ef89f-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="ef89f-114">DeviceManagementTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="ef89f-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="ef89f-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="ef89f-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="ef89f-116">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ef89f-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="ef89f-117">DeviceManagementTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="ef89f-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="ef89f-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="ef89f-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="ef89f-119">新しい[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ef89f-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="ef89f-120">DeviceManagementTemplate の削除</span><span class="sxs-lookup"><span data-stu-id="ef89f-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="ef89f-121">None</span><span class="sxs-lookup"><span data-stu-id="ef89f-121">None</span></span>|<span data-ttu-id="ef89f-122">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ef89f-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="ef89f-123">DeviceManagementTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="ef89f-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="ef89f-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="ef89f-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="ef89f-125">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef89f-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="ef89f-126">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="ef89f-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="ef89f-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="ef89f-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef89f-128">Not yet documented</span></span>|
|[<span data-ttu-id="ef89f-129">compare 関数</span><span class="sxs-lookup"><span data-stu-id="ef89f-129">compare function</span></span>](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|<span data-ttu-id="ef89f-130">[Devicemanagementsettingcomparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection</span></span>|<span data-ttu-id="ef89f-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef89f-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ef89f-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef89f-132">Properties</span></span>
|<span data-ttu-id="ef89f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef89f-133">Property</span></span>|<span data-ttu-id="ef89f-134">型</span><span class="sxs-lookup"><span data-stu-id="ef89f-134">Type</span></span>|<span data-ttu-id="ef89f-135">説明</span><span class="sxs-lookup"><span data-stu-id="ef89f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef89f-136">id</span><span class="sxs-lookup"><span data-stu-id="ef89f-136">id</span></span>|<span data-ttu-id="ef89f-137">文字列</span><span class="sxs-lookup"><span data-stu-id="ef89f-137">String</span></span>|<span data-ttu-id="ef89f-138">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="ef89f-138">The template ID</span></span>|
|<span data-ttu-id="ef89f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ef89f-139">displayName</span></span>|<span data-ttu-id="ef89f-140">String</span><span class="sxs-lookup"><span data-stu-id="ef89f-140">String</span></span>|<span data-ttu-id="ef89f-141">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="ef89f-141">The template's display name</span></span>|
|<span data-ttu-id="ef89f-142">description</span><span class="sxs-lookup"><span data-stu-id="ef89f-142">description</span></span>|<span data-ttu-id="ef89f-143">String</span><span class="sxs-lookup"><span data-stu-id="ef89f-143">String</span></span>|<span data-ttu-id="ef89f-144">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="ef89f-144">The template's description</span></span>|
|<span data-ttu-id="ef89f-145">versionInfo</span><span class="sxs-lookup"><span data-stu-id="ef89f-145">versionInfo</span></span>|<span data-ttu-id="ef89f-146">String</span><span class="sxs-lookup"><span data-stu-id="ef89f-146">String</span></span>|<span data-ttu-id="ef89f-147">テンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="ef89f-147">The template's version information</span></span>|
|<span data-ttu-id="ef89f-148">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="ef89f-148">isDeprecated</span></span>|<span data-ttu-id="ef89f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef89f-149">Boolean</span></span>|<span data-ttu-id="ef89f-150">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="ef89f-150">The template is deprecated or not.</span></span> <span data-ttu-id="ef89f-151">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="ef89f-151">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="ef89f-152">intentCount</span><span class="sxs-lookup"><span data-stu-id="ef89f-152">intentCount</span></span>|<span data-ttu-id="ef89f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ef89f-153">Int32</span></span>|<span data-ttu-id="ef89f-154">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="ef89f-154">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="ef89f-155">templateType</span><span class="sxs-lookup"><span data-stu-id="ef89f-155">templateType</span></span>|[<span data-ttu-id="ef89f-156">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="ef89f-156">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="ef89f-157">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ef89f-157">The template's type.</span></span> <span data-ttu-id="ef89f-158">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="ef89f-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="ef89f-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef89f-159">publishedDateTime</span></span>|<span data-ttu-id="ef89f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef89f-160">DateTimeOffset</span></span>|<span data-ttu-id="ef89f-161">テンプレートが発行されたとき</span><span class="sxs-lookup"><span data-stu-id="ef89f-161">When the template was published</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef89f-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef89f-162">Relationships</span></span>
|<span data-ttu-id="ef89f-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef89f-163">Relationship</span></span>|<span data-ttu-id="ef89f-164">型</span><span class="sxs-lookup"><span data-stu-id="ef89f-164">Type</span></span>|<span data-ttu-id="ef89f-165">説明</span><span class="sxs-lookup"><span data-stu-id="ef89f-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef89f-166">settings</span><span class="sxs-lookup"><span data-stu-id="ef89f-166">settings</span></span>|<span data-ttu-id="ef89f-167">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-167">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="ef89f-168">このテンプレートに含まれるすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-168">Collection of all settings this template has</span></span>|
|<span data-ttu-id="ef89f-169">categories</span><span class="sxs-lookup"><span data-stu-id="ef89f-169">categories</span></span>|<span data-ttu-id="ef89f-170">[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-170">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="ef89f-171">テンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-171">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="ef89f-172">migratableTo</span><span class="sxs-lookup"><span data-stu-id="ef89f-172">migratableTo</span></span>|<span data-ttu-id="ef89f-173">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-173">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="ef89f-174">このテンプレートが移行できるテンプレートのコレクション</span><span class="sxs-lookup"><span data-stu-id="ef89f-174">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef89f-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef89f-175">JSON Representation</span></span>
<span data-ttu-id="ef89f-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef89f-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "publishedDateTime": "String (timestamp)"
}
```



