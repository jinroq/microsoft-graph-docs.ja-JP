---
title: deviceManagementSettingCategory リソースの種類
description: 設定カテゴリを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c87774cf0aa8a5e3a4cb65b10566323b2c7749
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943390"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="a1270-103">deviceManagementSettingCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1270-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="a1270-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1270-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1270-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1270-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1270-106">設定カテゴリを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="a1270-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="a1270-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1270-107">Methods</span></span>
|<span data-ttu-id="a1270-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1270-108">Method</span></span>|<span data-ttu-id="a1270-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1270-109">Return Type</span></span>|<span data-ttu-id="a1270-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1270-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1270-111">DeviceManagementSettingCategories を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a1270-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="a1270-112">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1270-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="a1270-113">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a1270-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="a1270-114">DeviceManagementSettingCategory の取得</span><span class="sxs-lookup"><span data-stu-id="a1270-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="a1270-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="a1270-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="a1270-116">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1270-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="a1270-117">DeviceManagementSettingCategory の作成</span><span class="sxs-lookup"><span data-stu-id="a1270-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="a1270-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="a1270-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="a1270-119">新しい[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1270-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="a1270-120">DeviceManagementSettingCategory の削除</span><span class="sxs-lookup"><span data-stu-id="a1270-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="a1270-121">None</span><span class="sxs-lookup"><span data-stu-id="a1270-121">None</span></span>|<span data-ttu-id="a1270-122">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1270-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="a1270-123">DeviceManagementSettingCategory の更新</span><span class="sxs-lookup"><span data-stu-id="a1270-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="a1270-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="a1270-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="a1270-125">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1270-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1270-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1270-126">Properties</span></span>
|<span data-ttu-id="a1270-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1270-127">Property</span></span>|<span data-ttu-id="a1270-128">種類</span><span class="sxs-lookup"><span data-stu-id="a1270-128">Type</span></span>|<span data-ttu-id="a1270-129">説明</span><span class="sxs-lookup"><span data-stu-id="a1270-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1270-130">id</span><span class="sxs-lookup"><span data-stu-id="a1270-130">id</span></span>|<span data-ttu-id="a1270-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a1270-131">String</span></span>|<span data-ttu-id="a1270-132">カテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="a1270-132">The category ID</span></span>|
|<span data-ttu-id="a1270-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a1270-133">displayName</span></span>|<span data-ttu-id="a1270-134">String</span><span class="sxs-lookup"><span data-stu-id="a1270-134">String</span></span>|<span data-ttu-id="a1270-135">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="a1270-135">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1270-136">関係</span><span class="sxs-lookup"><span data-stu-id="a1270-136">Relationships</span></span>
|<span data-ttu-id="a1270-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1270-137">Relationship</span></span>|<span data-ttu-id="a1270-138">型</span><span class="sxs-lookup"><span data-stu-id="a1270-138">Type</span></span>|<span data-ttu-id="a1270-139">説明</span><span class="sxs-lookup"><span data-stu-id="a1270-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1270-140">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="a1270-140">settingDefinitions</span></span>|<span data-ttu-id="a1270-141">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1270-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="a1270-142">このカテゴリに含まれる設定の定義は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a1270-142">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1270-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1270-143">JSON Representation</span></span>
<span data-ttu-id="a1270-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1270-144">Here is a JSON representation of the resource.</span></span>
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




