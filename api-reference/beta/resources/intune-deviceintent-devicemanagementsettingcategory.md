---
title: devicemanagementsettingcategory リソースの種類
description: 設定カテゴリを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6af038e31135a99e473f6b14638655af073e1602
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550573"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="e182e-103">devicemanagementsettingcategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e182e-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="e182e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e182e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e182e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e182e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e182e-106">設定カテゴリを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="e182e-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="e182e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e182e-107">Methods</span></span>
|<span data-ttu-id="e182e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e182e-108">Method</span></span>|<span data-ttu-id="e182e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e182e-109">Return Type</span></span>|<span data-ttu-id="e182e-110">説明</span><span class="sxs-lookup"><span data-stu-id="e182e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e182e-111">devicemanagementsettingcategories を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e182e-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="e182e-112">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e182e-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="e182e-113">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e182e-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="e182e-114">devicemanagementsettingcategory の取得</span><span class="sxs-lookup"><span data-stu-id="e182e-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="e182e-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e182e-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="e182e-116">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e182e-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="e182e-117">devicemanagementsettingcategory の作成</span><span class="sxs-lookup"><span data-stu-id="e182e-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="e182e-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e182e-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="e182e-119">新しい[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e182e-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="e182e-120">devicemanagementsettingcategory の削除</span><span class="sxs-lookup"><span data-stu-id="e182e-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="e182e-121">なし</span><span class="sxs-lookup"><span data-stu-id="e182e-121">None</span></span>|<span data-ttu-id="e182e-122">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e182e-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="e182e-123">devicemanagementsettingcategory の更新</span><span class="sxs-lookup"><span data-stu-id="e182e-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="e182e-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="e182e-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="e182e-125">[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e182e-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e182e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e182e-126">Properties</span></span>
|<span data-ttu-id="e182e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e182e-127">Property</span></span>|<span data-ttu-id="e182e-128">型</span><span class="sxs-lookup"><span data-stu-id="e182e-128">Type</span></span>|<span data-ttu-id="e182e-129">説明</span><span class="sxs-lookup"><span data-stu-id="e182e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e182e-130">id</span><span class="sxs-lookup"><span data-stu-id="e182e-130">id</span></span>|<span data-ttu-id="e182e-131">String</span><span class="sxs-lookup"><span data-stu-id="e182e-131">String</span></span>|<span data-ttu-id="e182e-132">カテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="e182e-132">The category ID</span></span>|
|<span data-ttu-id="e182e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e182e-133">displayName</span></span>|<span data-ttu-id="e182e-134">String</span><span class="sxs-lookup"><span data-stu-id="e182e-134">String</span></span>|<span data-ttu-id="e182e-135">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="e182e-135">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="e182e-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e182e-136">Relationships</span></span>
|<span data-ttu-id="e182e-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e182e-137">Relationship</span></span>|<span data-ttu-id="e182e-138">型</span><span class="sxs-lookup"><span data-stu-id="e182e-138">Type</span></span>|<span data-ttu-id="e182e-139">説明</span><span class="sxs-lookup"><span data-stu-id="e182e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e182e-140">settingdefinitions</span><span class="sxs-lookup"><span data-stu-id="e182e-140">settingDefinitions</span></span>|<span data-ttu-id="e182e-141">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e182e-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="e182e-142">このカテゴリに含まれる設定の定義は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e182e-142">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e182e-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e182e-143">JSON Representation</span></span>
<span data-ttu-id="e182e-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e182e-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```





