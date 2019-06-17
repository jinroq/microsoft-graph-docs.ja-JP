---
title: deviceManagementTemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 438fbf37cb419145d63b8d25f9e8145005eac6cc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984416"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="14ea2-103">deviceManagementTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14ea2-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="14ea2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14ea2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14ea2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14ea2-106">デバイス設定の定義済みコレクションを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="14ea2-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="14ea2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="14ea2-107">Methods</span></span>
|<span data-ttu-id="14ea2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14ea2-108">Method</span></span>|<span data-ttu-id="14ea2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14ea2-109">Return Type</span></span>|<span data-ttu-id="14ea2-110">説明</span><span class="sxs-lookup"><span data-stu-id="14ea2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14ea2-111">DeviceManagementTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14ea2-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="14ea2-112">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="14ea2-113">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="14ea2-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="14ea2-114">DeviceManagementTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="14ea2-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="14ea2-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="14ea2-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="14ea2-116">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="14ea2-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="14ea2-117">DeviceManagementTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="14ea2-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="14ea2-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="14ea2-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="14ea2-119">新しい[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="14ea2-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="14ea2-120">DeviceManagementTemplate の削除</span><span class="sxs-lookup"><span data-stu-id="14ea2-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="14ea2-121">None</span><span class="sxs-lookup"><span data-stu-id="14ea2-121">None</span></span>|<span data-ttu-id="14ea2-122">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="14ea2-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="14ea2-123">DeviceManagementTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="14ea2-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="14ea2-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="14ea2-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="14ea2-125">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="14ea2-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="14ea2-126">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="14ea2-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="14ea2-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="14ea2-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14ea2-128">Not yet documented</span></span>|
|[<span data-ttu-id="14ea2-129">compare 関数</span><span class="sxs-lookup"><span data-stu-id="14ea2-129">compare function</span></span>](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|<span data-ttu-id="14ea2-130">[Devicemanagementsettingcomparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection</span></span>|<span data-ttu-id="14ea2-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14ea2-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="14ea2-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ea2-132">Properties</span></span>
|<span data-ttu-id="14ea2-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ea2-133">Property</span></span>|<span data-ttu-id="14ea2-134">型</span><span class="sxs-lookup"><span data-stu-id="14ea2-134">Type</span></span>|<span data-ttu-id="14ea2-135">説明</span><span class="sxs-lookup"><span data-stu-id="14ea2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ea2-136">id</span><span class="sxs-lookup"><span data-stu-id="14ea2-136">id</span></span>|<span data-ttu-id="14ea2-137">文字列</span><span class="sxs-lookup"><span data-stu-id="14ea2-137">String</span></span>|<span data-ttu-id="14ea2-138">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="14ea2-138">The template ID</span></span>|
|<span data-ttu-id="14ea2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="14ea2-139">displayName</span></span>|<span data-ttu-id="14ea2-140">String</span><span class="sxs-lookup"><span data-stu-id="14ea2-140">String</span></span>|<span data-ttu-id="14ea2-141">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="14ea2-141">The template's display name</span></span>|
|<span data-ttu-id="14ea2-142">description</span><span class="sxs-lookup"><span data-stu-id="14ea2-142">description</span></span>|<span data-ttu-id="14ea2-143">String</span><span class="sxs-lookup"><span data-stu-id="14ea2-143">String</span></span>|<span data-ttu-id="14ea2-144">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="14ea2-144">The template's description</span></span>|
|<span data-ttu-id="14ea2-145">versionInfo</span><span class="sxs-lookup"><span data-stu-id="14ea2-145">versionInfo</span></span>|<span data-ttu-id="14ea2-146">String</span><span class="sxs-lookup"><span data-stu-id="14ea2-146">String</span></span>|<span data-ttu-id="14ea2-147">テンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="14ea2-147">The template's version information</span></span>|
|<span data-ttu-id="14ea2-148">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="14ea2-148">isDeprecated</span></span>|<span data-ttu-id="14ea2-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="14ea2-149">Boolean</span></span>|<span data-ttu-id="14ea2-150">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="14ea2-150">The template is deprecated or not.</span></span> <span data-ttu-id="14ea2-151">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="14ea2-151">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="14ea2-152">intentCount</span><span class="sxs-lookup"><span data-stu-id="14ea2-152">intentCount</span></span>|<span data-ttu-id="14ea2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="14ea2-153">Int32</span></span>|<span data-ttu-id="14ea2-154">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="14ea2-154">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="14ea2-155">templateType</span><span class="sxs-lookup"><span data-stu-id="14ea2-155">templateType</span></span>|[<span data-ttu-id="14ea2-156">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="14ea2-156">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="14ea2-157">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="14ea2-157">The template's type.</span></span> <span data-ttu-id="14ea2-158">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="14ea2-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="14ea2-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="14ea2-159">publishedDateTime</span></span>|<span data-ttu-id="14ea2-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14ea2-160">DateTimeOffset</span></span>|<span data-ttu-id="14ea2-161">テンプレートが発行されたとき</span><span class="sxs-lookup"><span data-stu-id="14ea2-161">When the template was published</span></span>|

## <a name="relationships"></a><span data-ttu-id="14ea2-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14ea2-162">Relationships</span></span>
|<span data-ttu-id="14ea2-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14ea2-163">Relationship</span></span>|<span data-ttu-id="14ea2-164">型</span><span class="sxs-lookup"><span data-stu-id="14ea2-164">Type</span></span>|<span data-ttu-id="14ea2-165">説明</span><span class="sxs-lookup"><span data-stu-id="14ea2-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ea2-166">settings</span><span class="sxs-lookup"><span data-stu-id="14ea2-166">settings</span></span>|<span data-ttu-id="14ea2-167">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-167">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="14ea2-168">このテンプレートに含まれるすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-168">Collection of all settings this template has</span></span>|
|<span data-ttu-id="14ea2-169">categories</span><span class="sxs-lookup"><span data-stu-id="14ea2-169">categories</span></span>|<span data-ttu-id="14ea2-170">[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-170">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="14ea2-171">テンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-171">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="14ea2-172">migratableTo</span><span class="sxs-lookup"><span data-stu-id="14ea2-172">migratableTo</span></span>|<span data-ttu-id="14ea2-173">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-173">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="14ea2-174">このテンプレートが移行できるテンプレートのコレクション</span><span class="sxs-lookup"><span data-stu-id="14ea2-174">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14ea2-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14ea2-175">JSON Representation</span></span>
<span data-ttu-id="14ea2-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14ea2-176">Here is a JSON representation of the resource.</span></span>
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





