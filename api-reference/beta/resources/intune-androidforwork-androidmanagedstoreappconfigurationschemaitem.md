---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 39f7bb07e28875ec2d0280eb02a9d3c90b5a82e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366211"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="9928d-103">androidManagedStoreAppConfigurationSchemaItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9928d-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="9928d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9928d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9928d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9928d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9928d-106">Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。</span><span class="sxs-lookup"><span data-stu-id="9928d-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="9928d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9928d-107">Properties</span></span>
|<span data-ttu-id="9928d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9928d-108">Property</span></span>|<span data-ttu-id="9928d-109">型</span><span class="sxs-lookup"><span data-stu-id="9928d-109">Type</span></span>|<span data-ttu-id="9928d-110">説明</span><span class="sxs-lookup"><span data-stu-id="9928d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9928d-111">index</span><span class="sxs-lookup"><span data-stu-id="9928d-111">index</span></span>|<span data-ttu-id="9928d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9928d-112">Int32</span></span>|<span data-ttu-id="9928d-113">入れ子になったスキーマアイテムを維持するためにアプリケーションで使用する一意のインデックス</span><span class="sxs-lookup"><span data-stu-id="9928d-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="9928d-114">parentIndex</span><span class="sxs-lookup"><span data-stu-id="9928d-114">parentIndex</span></span>|<span data-ttu-id="9928d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9928d-115">Int32</span></span>|<span data-ttu-id="9928d-116">入れ子になったスキーマアイテムを追跡するための親スキーマアイテムのインデックス</span><span class="sxs-lookup"><span data-stu-id="9928d-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="9928d-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="9928d-117">schemaItemKey</span></span>|<span data-ttu-id="9928d-118">String</span><span class="sxs-lookup"><span data-stu-id="9928d-118">String</span></span>|<span data-ttu-id="9928d-119">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="9928d-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="9928d-120">displayName</span><span class="sxs-lookup"><span data-stu-id="9928d-120">displayName</span></span>|<span data-ttu-id="9928d-121">String</span><span class="sxs-lookup"><span data-stu-id="9928d-121">String</span></span>|<span data-ttu-id="9928d-122">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="9928d-122">Human readable name</span></span>|
|<span data-ttu-id="9928d-123">description</span><span class="sxs-lookup"><span data-stu-id="9928d-123">description</span></span>|<span data-ttu-id="9928d-124">String</span><span class="sxs-lookup"><span data-stu-id="9928d-124">String</span></span>|<span data-ttu-id="9928d-125">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="9928d-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="9928d-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="9928d-126">defaultBoolValue</span></span>|<span data-ttu-id="9928d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="9928d-127">Boolean</span></span>|<span data-ttu-id="9928d-128">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9928d-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9928d-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="9928d-129">defaultIntValue</span></span>|<span data-ttu-id="9928d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9928d-130">Int32</span></span>|<span data-ttu-id="9928d-131">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9928d-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9928d-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="9928d-132">defaultStringValue</span></span>|<span data-ttu-id="9928d-133">String</span><span class="sxs-lookup"><span data-stu-id="9928d-133">String</span></span>|<span data-ttu-id="9928d-134">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9928d-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9928d-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="9928d-135">defaultStringArrayValue</span></span>|<span data-ttu-id="9928d-136">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9928d-136">String collection</span></span>|<span data-ttu-id="9928d-137">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9928d-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9928d-138">dataType</span><span class="sxs-lookup"><span data-stu-id="9928d-138">dataType</span></span>|[<span data-ttu-id="9928d-139">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="9928d-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="9928d-140">このアイテムが記述する値の種類。</span><span class="sxs-lookup"><span data-stu-id="9928d-140">The type of value this item describes.</span></span> <span data-ttu-id="9928d-141">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="9928d-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="9928d-142">selections</span><span class="sxs-lookup"><span data-stu-id="9928d-142">selections</span></span>|<span data-ttu-id="9928d-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9928d-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9928d-144">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="9928d-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9928d-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9928d-145">Relationships</span></span>
<span data-ttu-id="9928d-146">なし</span><span class="sxs-lookup"><span data-stu-id="9928d-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9928d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9928d-147">JSON Representation</span></span>
<span data-ttu-id="9928d-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9928d-148">Here is a JSON representation of the resource.</span></span>
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



