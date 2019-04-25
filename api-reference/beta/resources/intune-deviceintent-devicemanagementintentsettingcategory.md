---
title: devicemanagementintentsettingcategory リソースの種類
description: 意図の設定カテゴリを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1551d4d4217b03380feef46d07d9f0cc5dac4064
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550701"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a><span data-ttu-id="e1845-103">devicemanagementintentsettingcategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1845-103">deviceManagementIntentSettingCategory resource type</span></span>

> <span data-ttu-id="e1845-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1845-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1845-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1845-106">意図の設定カテゴリを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="e1845-106">Entity representing an intent setting category</span></span>


<span data-ttu-id="e1845-107">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e1845-107">Inherits from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e1845-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1845-108">Methods</span></span>
|<span data-ttu-id="e1845-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1845-109">Method</span></span>|<span data-ttu-id="e1845-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1845-110">Return Type</span></span>|<span data-ttu-id="e1845-111">説明</span><span class="sxs-lookup"><span data-stu-id="e1845-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1845-112">devicemanagementintentsettingcategories のリスト</span><span class="sxs-lookup"><span data-stu-id="e1845-112">List deviceManagementIntentSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|<span data-ttu-id="e1845-113">[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1845-113">[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) collection</span></span>|<span data-ttu-id="e1845-114">[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e1845-114">List properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="e1845-115">devicemanagementintentsettingcategory の取得</span><span class="sxs-lookup"><span data-stu-id="e1845-115">Get deviceManagementIntentSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[<span data-ttu-id="e1845-116">deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e1845-116">deviceManagementIntentSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|<span data-ttu-id="e1845-117">[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1845-117">Read properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="e1845-118">devicemanagementintentsettingcategory の作成</span><span class="sxs-lookup"><span data-stu-id="e1845-118">Create deviceManagementIntentSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[<span data-ttu-id="e1845-119">deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e1845-119">deviceManagementIntentSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|<span data-ttu-id="e1845-120">新しい[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1845-120">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="e1845-121">devicemanagementintentsettingcategory の削除</span><span class="sxs-lookup"><span data-stu-id="e1845-121">Delete deviceManagementIntentSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|<span data-ttu-id="e1845-122">なし</span><span class="sxs-lookup"><span data-stu-id="e1845-122">None</span></span>|<span data-ttu-id="e1845-123">[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e1845-123">Deletes a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>|
|[<span data-ttu-id="e1845-124">devicemanagementintentsettingcategory の更新</span><span class="sxs-lookup"><span data-stu-id="e1845-124">Update deviceManagementIntentSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[<span data-ttu-id="e1845-125">deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e1845-125">deviceManagementIntentSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|<span data-ttu-id="e1845-126">[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e1845-126">Update the properties of a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1845-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1845-127">Properties</span></span>
|<span data-ttu-id="e1845-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1845-128">Property</span></span>|<span data-ttu-id="e1845-129">型</span><span class="sxs-lookup"><span data-stu-id="e1845-129">Type</span></span>|<span data-ttu-id="e1845-130">説明</span><span class="sxs-lookup"><span data-stu-id="e1845-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1845-131">id</span><span class="sxs-lookup"><span data-stu-id="e1845-131">id</span></span>|<span data-ttu-id="e1845-132">String</span><span class="sxs-lookup"><span data-stu-id="e1845-132">String</span></span>|<span data-ttu-id="e1845-133">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="e1845-133">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="e1845-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e1845-134">displayName</span></span>|<span data-ttu-id="e1845-135">String</span><span class="sxs-lookup"><span data-stu-id="e1845-135">String</span></span>|<span data-ttu-id="e1845-136">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名</span><span class="sxs-lookup"><span data-stu-id="e1845-136">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1845-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1845-137">Relationships</span></span>
|<span data-ttu-id="e1845-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1845-138">Relationship</span></span>|<span data-ttu-id="e1845-139">型</span><span class="sxs-lookup"><span data-stu-id="e1845-139">Type</span></span>|<span data-ttu-id="e1845-140">説明</span><span class="sxs-lookup"><span data-stu-id="e1845-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1845-141">settingdefinitions</span><span class="sxs-lookup"><span data-stu-id="e1845-141">settingDefinitions</span></span>|<span data-ttu-id="e1845-142">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1845-142">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="e1845-143">このカテゴリには、 [devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承する設定定義が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e1845-143">The setting definitions this category contains Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="e1845-144">settings</span><span class="sxs-lookup"><span data-stu-id="e1845-144">settings</span></span>|<span data-ttu-id="e1845-145">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1845-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="e1845-146">このカテゴリに含まれる設定</span><span class="sxs-lookup"><span data-stu-id="e1845-146">The settings this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1845-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1845-147">JSON Representation</span></span>
<span data-ttu-id="e1845-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1845-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```





