---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2168cc2449092249ec07f17831c38b5be15d7676
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971691"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="a6532-103">androidManagedStoreAppConfigurationSchemaItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6532-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="a6532-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6532-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6532-106">Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。</span><span class="sxs-lookup"><span data-stu-id="a6532-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="a6532-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6532-107">Properties</span></span>
|<span data-ttu-id="a6532-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6532-108">Property</span></span>|<span data-ttu-id="a6532-109">型</span><span class="sxs-lookup"><span data-stu-id="a6532-109">Type</span></span>|<span data-ttu-id="a6532-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6532-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6532-111">index</span><span class="sxs-lookup"><span data-stu-id="a6532-111">index</span></span>|<span data-ttu-id="a6532-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a6532-112">Int32</span></span>|<span data-ttu-id="a6532-113">入れ子になったスキーマアイテムを維持するためにアプリケーションで使用する一意のインデックス</span><span class="sxs-lookup"><span data-stu-id="a6532-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="a6532-114">parentIndex</span><span class="sxs-lookup"><span data-stu-id="a6532-114">parentIndex</span></span>|<span data-ttu-id="a6532-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a6532-115">Int32</span></span>|<span data-ttu-id="a6532-116">入れ子になったスキーマアイテムを追跡するための親スキーマアイテムのインデックス</span><span class="sxs-lookup"><span data-stu-id="a6532-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="a6532-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="a6532-117">schemaItemKey</span></span>|<span data-ttu-id="a6532-118">String</span><span class="sxs-lookup"><span data-stu-id="a6532-118">String</span></span>|<span data-ttu-id="a6532-119">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="a6532-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="a6532-120">displayName</span><span class="sxs-lookup"><span data-stu-id="a6532-120">displayName</span></span>|<span data-ttu-id="a6532-121">String</span><span class="sxs-lookup"><span data-stu-id="a6532-121">String</span></span>|<span data-ttu-id="a6532-122">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="a6532-122">Human readable name</span></span>|
|<span data-ttu-id="a6532-123">description</span><span class="sxs-lookup"><span data-stu-id="a6532-123">description</span></span>|<span data-ttu-id="a6532-124">String</span><span class="sxs-lookup"><span data-stu-id="a6532-124">String</span></span>|<span data-ttu-id="a6532-125">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="a6532-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="a6532-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="a6532-126">defaultBoolValue</span></span>|<span data-ttu-id="a6532-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6532-127">Boolean</span></span>|<span data-ttu-id="a6532-128">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a6532-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a6532-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="a6532-129">defaultIntValue</span></span>|<span data-ttu-id="a6532-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a6532-130">Int32</span></span>|<span data-ttu-id="a6532-131">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a6532-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a6532-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="a6532-132">defaultStringValue</span></span>|<span data-ttu-id="a6532-133">String</span><span class="sxs-lookup"><span data-stu-id="a6532-133">String</span></span>|<span data-ttu-id="a6532-134">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a6532-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a6532-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="a6532-135">defaultStringArrayValue</span></span>|<span data-ttu-id="a6532-136">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6532-136">String collection</span></span>|<span data-ttu-id="a6532-137">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a6532-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a6532-138">dataType</span><span class="sxs-lookup"><span data-stu-id="a6532-138">dataType</span></span>|[<span data-ttu-id="a6532-139">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="a6532-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="a6532-140">このアイテムが記述する値の種類。</span><span class="sxs-lookup"><span data-stu-id="a6532-140">The type of value this item describes.</span></span> <span data-ttu-id="a6532-141">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="a6532-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="a6532-142">selections</span><span class="sxs-lookup"><span data-stu-id="a6532-142">selections</span></span>|<span data-ttu-id="a6532-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6532-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a6532-144">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="a6532-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6532-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6532-145">Relationships</span></span>
<span data-ttu-id="a6532-146">なし</span><span class="sxs-lookup"><span data-stu-id="a6532-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6532-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6532-147">JSON Representation</span></span>
<span data-ttu-id="a6532-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6532-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```





