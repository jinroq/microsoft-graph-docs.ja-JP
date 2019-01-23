---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398920"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="d0433-103">androidManagedStoreAppConfigurationSchemaItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0433-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="d0433-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0433-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0433-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0433-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0433-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0433-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0433-107">Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。</span><span class="sxs-lookup"><span data-stu-id="d0433-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="d0433-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0433-108">Properties</span></span>
|<span data-ttu-id="d0433-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0433-109">Property</span></span>|<span data-ttu-id="d0433-110">型</span><span class="sxs-lookup"><span data-stu-id="d0433-110">Type</span></span>|<span data-ttu-id="d0433-111">説明</span><span class="sxs-lookup"><span data-stu-id="d0433-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0433-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="d0433-112">schemaItemKey</span></span>|<span data-ttu-id="d0433-113">String</span><span class="sxs-lookup"><span data-stu-id="d0433-113">String</span></span>|<span data-ttu-id="d0433-114">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="d0433-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="d0433-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d0433-115">displayName</span></span>|<span data-ttu-id="d0433-116">String</span><span class="sxs-lookup"><span data-stu-id="d0433-116">String</span></span>|<span data-ttu-id="d0433-117">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="d0433-117">Human readable name</span></span>|
|<span data-ttu-id="d0433-118">説明</span><span class="sxs-lookup"><span data-stu-id="d0433-118">description</span></span>|<span data-ttu-id="d0433-119">String</span><span class="sxs-lookup"><span data-stu-id="d0433-119">String</span></span>|<span data-ttu-id="d0433-120">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="d0433-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="d0433-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="d0433-121">defaultBoolValue</span></span>|<span data-ttu-id="d0433-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0433-122">Boolean</span></span>|<span data-ttu-id="d0433-123">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="d0433-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d0433-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="d0433-124">defaultIntValue</span></span>|<span data-ttu-id="d0433-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d0433-125">Int32</span></span>|<span data-ttu-id="d0433-126">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="d0433-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d0433-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="d0433-127">defaultStringValue</span></span>|<span data-ttu-id="d0433-128">String</span><span class="sxs-lookup"><span data-stu-id="d0433-128">String</span></span>|<span data-ttu-id="d0433-129">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="d0433-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d0433-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="d0433-130">defaultStringArrayValue</span></span>|<span data-ttu-id="d0433-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d0433-131">String collection</span></span>|<span data-ttu-id="d0433-132">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="d0433-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d0433-133">dataType</span><span class="sxs-lookup"><span data-stu-id="d0433-133">dataType</span></span>|[<span data-ttu-id="d0433-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="d0433-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="d0433-135">この項目を記述する値の型。</span><span class="sxs-lookup"><span data-stu-id="d0433-135">The type of value this item describes.</span></span> <span data-ttu-id="d0433-136">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="d0433-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="d0433-137">selections</span><span class="sxs-lookup"><span data-stu-id="d0433-137">selections</span></span>|<span data-ttu-id="d0433-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d0433-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d0433-139">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="d0433-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0433-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0433-140">Relationships</span></span>
<span data-ttu-id="d0433-141">なし</span><span class="sxs-lookup"><span data-stu-id="d0433-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0433-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0433-142">JSON Representation</span></span>
<span data-ttu-id="d0433-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0433-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




