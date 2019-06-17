---
title: deviceManagementSettingCategory リソースの種類
description: 設定カテゴリを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cdf19dcfae033a6e7e17219cc9605635d25c621
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963948"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="0b7f6-103">deviceManagementSettingCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b7f6-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="0b7f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b7f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b7f6-106">設定カテゴリを表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="0b7f6-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="0b7f6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b7f6-107">Methods</span></span>
|<span data-ttu-id="0b7f6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b7f6-108">Method</span></span>|<span data-ttu-id="0b7f6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0b7f6-109">Return Type</span></span>|<span data-ttu-id="0b7f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b7f6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b7f6-111">DeviceManagementSettingCategories を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0b7f6-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="0b7f6-112">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b7f6-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="0b7f6-113">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="0b7f6-114">DeviceManagementSettingCategory の取得</span><span class="sxs-lookup"><span data-stu-id="0b7f6-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="0b7f6-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="0b7f6-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="0b7f6-116">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="0b7f6-117">DeviceManagementSettingCategory の作成</span><span class="sxs-lookup"><span data-stu-id="0b7f6-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="0b7f6-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="0b7f6-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="0b7f6-119">新しい[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="0b7f6-120">DeviceManagementSettingCategory の削除</span><span class="sxs-lookup"><span data-stu-id="0b7f6-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="0b7f6-121">None</span><span class="sxs-lookup"><span data-stu-id="0b7f6-121">None</span></span>|<span data-ttu-id="0b7f6-122">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="0b7f6-123">DeviceManagementSettingCategory の更新</span><span class="sxs-lookup"><span data-stu-id="0b7f6-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="0b7f6-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="0b7f6-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="0b7f6-125">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b7f6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b7f6-126">Properties</span></span>
|<span data-ttu-id="0b7f6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b7f6-127">Property</span></span>|<span data-ttu-id="0b7f6-128">型</span><span class="sxs-lookup"><span data-stu-id="0b7f6-128">Type</span></span>|<span data-ttu-id="0b7f6-129">説明</span><span class="sxs-lookup"><span data-stu-id="0b7f6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b7f6-130">id</span><span class="sxs-lookup"><span data-stu-id="0b7f6-130">id</span></span>|<span data-ttu-id="0b7f6-131">文字列</span><span class="sxs-lookup"><span data-stu-id="0b7f6-131">String</span></span>|<span data-ttu-id="0b7f6-132">カテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="0b7f6-132">The category ID</span></span>|
|<span data-ttu-id="0b7f6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b7f6-133">displayName</span></span>|<span data-ttu-id="0b7f6-134">String</span><span class="sxs-lookup"><span data-stu-id="0b7f6-134">String</span></span>|<span data-ttu-id="0b7f6-135">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="0b7f6-135">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b7f6-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b7f6-136">Relationships</span></span>
|<span data-ttu-id="0b7f6-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b7f6-137">Relationship</span></span>|<span data-ttu-id="0b7f6-138">型</span><span class="sxs-lookup"><span data-stu-id="0b7f6-138">Type</span></span>|<span data-ttu-id="0b7f6-139">説明</span><span class="sxs-lookup"><span data-stu-id="0b7f6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b7f6-140">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="0b7f6-140">settingDefinitions</span></span>|<span data-ttu-id="0b7f6-141">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b7f6-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="0b7f6-142">このカテゴリに含まれる設定の定義は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-142">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b7f6-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b7f6-143">JSON Representation</span></span>
<span data-ttu-id="0b7f6-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b7f6-144">Here is a JSON representation of the resource.</span></span>
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





