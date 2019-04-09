---
title: devicemanagementtemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf144ed30a017dc1f3ae84fc481568adc0d0d09
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522518"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="5363b-103">devicemanagementtemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5363b-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="5363b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5363b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5363b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5363b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5363b-106">デバイス設定の定義済みコレクションを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="5363b-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="5363b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5363b-107">Methods</span></span>
|<span data-ttu-id="5363b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5363b-108">Method</span></span>|<span data-ttu-id="5363b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5363b-109">Return Type</span></span>|<span data-ttu-id="5363b-110">説明</span><span class="sxs-lookup"><span data-stu-id="5363b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5363b-111">devicemanagementtemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5363b-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="5363b-112">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5363b-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="5363b-113">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5363b-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="5363b-114">devicemanagementtemplate の取得</span><span class="sxs-lookup"><span data-stu-id="5363b-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="5363b-115">devicemanagementtemplate</span><span class="sxs-lookup"><span data-stu-id="5363b-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5363b-116">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5363b-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5363b-117">devicemanagementtemplate の作成</span><span class="sxs-lookup"><span data-stu-id="5363b-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="5363b-118">devicemanagementtemplate</span><span class="sxs-lookup"><span data-stu-id="5363b-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5363b-119">新しい[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5363b-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5363b-120">devicemanagementtemplate の削除</span><span class="sxs-lookup"><span data-stu-id="5363b-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="5363b-121">なし</span><span class="sxs-lookup"><span data-stu-id="5363b-121">None</span></span>|<span data-ttu-id="5363b-122">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5363b-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="5363b-123">devicemanagementtemplate の更新</span><span class="sxs-lookup"><span data-stu-id="5363b-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="5363b-124">devicemanagementtemplate</span><span class="sxs-lookup"><span data-stu-id="5363b-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="5363b-125">[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5363b-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="5363b-126">createInstance アクション</span><span class="sxs-lookup"><span data-stu-id="5363b-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="5363b-127">devicemanagementintent</span><span class="sxs-lookup"><span data-stu-id="5363b-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="5363b-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5363b-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5363b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5363b-129">Properties</span></span>
|<span data-ttu-id="5363b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5363b-130">Property</span></span>|<span data-ttu-id="5363b-131">型</span><span class="sxs-lookup"><span data-stu-id="5363b-131">Type</span></span>|<span data-ttu-id="5363b-132">説明</span><span class="sxs-lookup"><span data-stu-id="5363b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5363b-133">id</span><span class="sxs-lookup"><span data-stu-id="5363b-133">id</span></span>|<span data-ttu-id="5363b-134">文字列</span><span class="sxs-lookup"><span data-stu-id="5363b-134">String</span></span>|<span data-ttu-id="5363b-135">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="5363b-135">The template ID</span></span>|
|<span data-ttu-id="5363b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5363b-136">displayName</span></span>|<span data-ttu-id="5363b-137">String</span><span class="sxs-lookup"><span data-stu-id="5363b-137">String</span></span>|<span data-ttu-id="5363b-138">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="5363b-138">The template's display name</span></span>|
|<span data-ttu-id="5363b-139">説明</span><span class="sxs-lookup"><span data-stu-id="5363b-139">description</span></span>|<span data-ttu-id="5363b-140">String</span><span class="sxs-lookup"><span data-stu-id="5363b-140">String</span></span>|<span data-ttu-id="5363b-141">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="5363b-141">The template's description</span></span>|

## <a name="relationships"></a><span data-ttu-id="5363b-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5363b-142">Relationships</span></span>
|<span data-ttu-id="5363b-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5363b-143">Relationship</span></span>|<span data-ttu-id="5363b-144">型</span><span class="sxs-lookup"><span data-stu-id="5363b-144">Type</span></span>|<span data-ttu-id="5363b-145">説明</span><span class="sxs-lookup"><span data-stu-id="5363b-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5363b-146">settings</span><span class="sxs-lookup"><span data-stu-id="5363b-146">settings</span></span>|<span data-ttu-id="5363b-147">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5363b-147">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="5363b-148">このテンプレートに含まれるすべての設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="5363b-148">Collection of all settings this template has</span></span>|
|<span data-ttu-id="5363b-149">categories</span><span class="sxs-lookup"><span data-stu-id="5363b-149">categories</span></span>|<span data-ttu-id="5363b-150">[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5363b-150">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="5363b-151">テンプレート内のカテゴリ設定のコレクション</span><span class="sxs-lookup"><span data-stu-id="5363b-151">Collection of setting categories within the template</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5363b-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5363b-152">JSON Representation</span></span>
<span data-ttu-id="5363b-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5363b-153">Here is a JSON representation of the resource.</span></span>
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
  "description": "String"
}
```







