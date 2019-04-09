---
title: securityBaselineTemplate リソースの種類
description: アカウントのセキュリティベースラインテンプレート
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b572d3cc25943438f190a46fd23704a2eb6b7be3
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522343"
---
# <a name="securitybaselinetemplate-resource-type"></a><span data-ttu-id="e86a4-103">securityBaselineTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e86a4-103">securityBaselineTemplate resource type</span></span>

> <span data-ttu-id="e86a4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e86a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e86a4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e86a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e86a4-106">アカウントのセキュリティベースラインテンプレート</span><span class="sxs-lookup"><span data-stu-id="e86a4-106">The security baseline template of the account</span></span>


<span data-ttu-id="e86a4-107">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e86a4-107">Inherits from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e86a4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e86a4-108">Methods</span></span>
|<span data-ttu-id="e86a4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e86a4-109">Method</span></span>|<span data-ttu-id="e86a4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e86a4-110">Return Type</span></span>|<span data-ttu-id="e86a4-111">説明</span><span class="sxs-lookup"><span data-stu-id="e86a4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e86a4-112">リスト securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="e86a4-112">List securityBaselineTemplates</span></span>](../api/intune-deviceintent-securitybaselinetemplate-list.md)|<span data-ttu-id="e86a4-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) collection</span></span>|<span data-ttu-id="e86a4-114">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e86a4-114">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>|
|[<span data-ttu-id="e86a4-115">securityBaselineTemplate を取得する</span><span class="sxs-lookup"><span data-stu-id="e86a4-115">Get securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[<span data-ttu-id="e86a4-116">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="e86a4-116">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="e86a4-117">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e86a4-117">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="e86a4-118">securityBaselineTemplate を作成する</span><span class="sxs-lookup"><span data-stu-id="e86a4-118">Create securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[<span data-ttu-id="e86a4-119">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="e86a4-119">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="e86a4-120">新しい[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e86a4-120">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="e86a4-121">securityBaselineTemplate の削除</span><span class="sxs-lookup"><span data-stu-id="e86a4-121">Delete securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|<span data-ttu-id="e86a4-122">なし</span><span class="sxs-lookup"><span data-stu-id="e86a4-122">None</span></span>|<span data-ttu-id="e86a4-123">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e86a4-123">Deletes a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>|
|[<span data-ttu-id="e86a4-124">securityBaselineTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="e86a4-124">Update securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[<span data-ttu-id="e86a4-125">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="e86a4-125">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="e86a4-126">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e86a4-126">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e86a4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e86a4-127">Properties</span></span>
|<span data-ttu-id="e86a4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e86a4-128">Property</span></span>|<span data-ttu-id="e86a4-129">型</span><span class="sxs-lookup"><span data-stu-id="e86a4-129">Type</span></span>|<span data-ttu-id="e86a4-130">説明</span><span class="sxs-lookup"><span data-stu-id="e86a4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e86a4-131">id</span><span class="sxs-lookup"><span data-stu-id="e86a4-131">id</span></span>|<span data-ttu-id="e86a4-132">文字列</span><span class="sxs-lookup"><span data-stu-id="e86a4-132">String</span></span>|<span data-ttu-id="e86a4-133">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID</span><span class="sxs-lookup"><span data-stu-id="e86a4-133">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e86a4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e86a4-134">displayName</span></span>|<span data-ttu-id="e86a4-135">String</span><span class="sxs-lookup"><span data-stu-id="e86a4-135">String</span></span>|<span data-ttu-id="e86a4-136">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="e86a4-136">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e86a4-137">説明</span><span class="sxs-lookup"><span data-stu-id="e86a4-137">description</span></span>|<span data-ttu-id="e86a4-138">String</span><span class="sxs-lookup"><span data-stu-id="e86a4-138">String</span></span>|<span data-ttu-id="e86a4-139">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="e86a4-139">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e86a4-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e86a4-140">Relationships</span></span>
|<span data-ttu-id="e86a4-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e86a4-141">Relationship</span></span>|<span data-ttu-id="e86a4-142">型</span><span class="sxs-lookup"><span data-stu-id="e86a4-142">Type</span></span>|<span data-ttu-id="e86a4-143">説明</span><span class="sxs-lookup"><span data-stu-id="e86a4-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e86a4-144">settings</span><span class="sxs-lookup"><span data-stu-id="e86a4-144">settings</span></span>|<span data-ttu-id="e86a4-145">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="e86a4-146">このテンプレートが[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承したすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-146">Collection of all settings this template has Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e86a4-147">categories</span><span class="sxs-lookup"><span data-stu-id="e86a4-147">categories</span></span>|<span data-ttu-id="e86a4-148">[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-148">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="e86a4-149">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-149">Collection of setting categories within the template Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e86a4-150">deviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e86a4-150">deviceStateSummary</span></span>|[<span data-ttu-id="e86a4-151">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="e86a4-151">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="e86a4-152">セキュリティベースラインデバイスの状態の概要</span><span class="sxs-lookup"><span data-stu-id="e86a4-152">The security baseline device state summary</span></span>|
|<span data-ttu-id="e86a4-153">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e86a4-153">deviceStates</span></span>|<span data-ttu-id="e86a4-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e86a4-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="e86a4-155">セキュリティベースラインデバイスの状態</span><span class="sxs-lookup"><span data-stu-id="e86a4-155">The security baseline device states</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e86a4-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e86a4-156">JSON Representation</span></span>
<span data-ttu-id="e86a4-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e86a4-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```







