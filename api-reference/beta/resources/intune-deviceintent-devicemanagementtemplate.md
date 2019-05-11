---
title: deviceManagementTemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffaa90db6b47502dfd66c39538f14a3c1a52b669
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943411"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="5a014-103">deviceManagementTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a014-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="5a014-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a014-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a014-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a014-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a014-106">デバイス設定の定義済みコレクションを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="5a014-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="5a014-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a014-107">Methods</span></span>
|<span data-ttu-id="5a014-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a014-108">Method</span></span>|<span data-ttu-id="5a014-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a014-109">Return Type</span></span>|<span data-ttu-id="5a014-110">説明</span><span class="sxs-lookup"><span data-stu-id="5a014-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a014-111">DeviceManagementTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5a014-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="5a014-112">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="5a014-113">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5a014-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="5a014-114">DeviceManagementTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="5a014-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="5a014-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="5a014-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5a014-116">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a014-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5a014-117">DeviceManagementTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="5a014-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="5a014-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="5a014-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5a014-119">新しい[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a014-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5a014-120">DeviceManagementTemplate の削除</span><span class="sxs-lookup"><span data-stu-id="5a014-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="5a014-121">None</span><span class="sxs-lookup"><span data-stu-id="5a014-121">None</span></span>|<span data-ttu-id="5a014-122">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a014-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="5a014-123">DeviceManagementTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="5a014-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="5a014-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="5a014-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5a014-125">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a014-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5a014-126">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="5a014-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="5a014-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="5a014-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="5a014-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a014-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a014-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a014-129">Properties</span></span>
|<span data-ttu-id="5a014-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a014-130">Property</span></span>|<span data-ttu-id="5a014-131">種類</span><span class="sxs-lookup"><span data-stu-id="5a014-131">Type</span></span>|<span data-ttu-id="5a014-132">説明</span><span class="sxs-lookup"><span data-stu-id="5a014-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a014-133">id</span><span class="sxs-lookup"><span data-stu-id="5a014-133">id</span></span>|<span data-ttu-id="5a014-134">文字列</span><span class="sxs-lookup"><span data-stu-id="5a014-134">String</span></span>|<span data-ttu-id="5a014-135">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="5a014-135">The template ID</span></span>|
|<span data-ttu-id="5a014-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5a014-136">displayName</span></span>|<span data-ttu-id="5a014-137">String</span><span class="sxs-lookup"><span data-stu-id="5a014-137">String</span></span>|<span data-ttu-id="5a014-138">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="5a014-138">The template's display name</span></span>|
|<span data-ttu-id="5a014-139">description</span><span class="sxs-lookup"><span data-stu-id="5a014-139">description</span></span>|<span data-ttu-id="5a014-140">String</span><span class="sxs-lookup"><span data-stu-id="5a014-140">String</span></span>|<span data-ttu-id="5a014-141">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="5a014-141">The template's description</span></span>|
|<span data-ttu-id="5a014-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="5a014-142">versionInfo</span></span>|<span data-ttu-id="5a014-143">String</span><span class="sxs-lookup"><span data-stu-id="5a014-143">String</span></span>|<span data-ttu-id="5a014-144">テンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="5a014-144">The template's version information</span></span>|
|<span data-ttu-id="5a014-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="5a014-145">isDeprecated</span></span>|<span data-ttu-id="5a014-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a014-146">Boolean</span></span>|<span data-ttu-id="5a014-147">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="5a014-147">The template is deprecated or not.</span></span> <span data-ttu-id="5a014-148">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="5a014-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="5a014-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="5a014-149">intentCount</span></span>|<span data-ttu-id="5a014-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5a014-150">Int32</span></span>|<span data-ttu-id="5a014-151">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="5a014-151">Number of Intents created from this template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a014-152">関係</span><span class="sxs-lookup"><span data-stu-id="5a014-152">Relationships</span></span>
|<span data-ttu-id="5a014-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a014-153">Relationship</span></span>|<span data-ttu-id="5a014-154">型</span><span class="sxs-lookup"><span data-stu-id="5a014-154">Type</span></span>|<span data-ttu-id="5a014-155">説明</span><span class="sxs-lookup"><span data-stu-id="5a014-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a014-156">settings</span><span class="sxs-lookup"><span data-stu-id="5a014-156">settings</span></span>|<span data-ttu-id="5a014-157">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-157">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="5a014-158">このテンプレートに含まれるすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-158">Collection of all settings this template has</span></span>|
|<span data-ttu-id="5a014-159">categories</span><span class="sxs-lookup"><span data-stu-id="5a014-159">categories</span></span>|<span data-ttu-id="5a014-160">[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-160">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="5a014-161">テンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-161">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="5a014-162">migratableTo</span><span class="sxs-lookup"><span data-stu-id="5a014-162">migratableTo</span></span>|<span data-ttu-id="5a014-163">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-163">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="5a014-164">このテンプレートが移行できるテンプレートのコレクション</span><span class="sxs-lookup"><span data-stu-id="5a014-164">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a014-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a014-165">JSON Representation</span></span>
<span data-ttu-id="5a014-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a014-166">Here is a JSON representation of the resource.</span></span>
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
  "intentCount": 1024
}
```




