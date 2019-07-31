---
title: androidForWorkAppConfigurationSchemaItem リソース タイプ
description: Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe1e0cb9157463741a9ba4b7e1e6e77f7b454e73
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971782"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="9b903-103">androidForWorkAppConfigurationSchemaItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="9b903-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="9b903-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b903-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b903-106">Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。</span><span class="sxs-lookup"><span data-stu-id="9b903-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="9b903-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b903-107">Properties</span></span>
|<span data-ttu-id="9b903-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b903-108">Property</span></span>|<span data-ttu-id="9b903-109">型</span><span class="sxs-lookup"><span data-stu-id="9b903-109">Type</span></span>|<span data-ttu-id="9b903-110">説明</span><span class="sxs-lookup"><span data-stu-id="9b903-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b903-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="9b903-111">schemaItemKey</span></span>|<span data-ttu-id="9b903-112">String</span><span class="sxs-lookup"><span data-stu-id="9b903-112">String</span></span>|<span data-ttu-id="9b903-113">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="9b903-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="9b903-114">displayName</span><span class="sxs-lookup"><span data-stu-id="9b903-114">displayName</span></span>|<span data-ttu-id="9b903-115">String</span><span class="sxs-lookup"><span data-stu-id="9b903-115">String</span></span>|<span data-ttu-id="9b903-116">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="9b903-116">Human readable name</span></span>|
|<span data-ttu-id="9b903-117">description</span><span class="sxs-lookup"><span data-stu-id="9b903-117">description</span></span>|<span data-ttu-id="9b903-118">String</span><span class="sxs-lookup"><span data-stu-id="9b903-118">String</span></span>|<span data-ttu-id="9b903-119">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="9b903-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="9b903-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="9b903-120">defaultBoolValue</span></span>|<span data-ttu-id="9b903-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b903-121">Boolean</span></span>|<span data-ttu-id="9b903-122">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9b903-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9b903-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="9b903-123">defaultIntValue</span></span>|<span data-ttu-id="9b903-124">Int32</span><span class="sxs-lookup"><span data-stu-id="9b903-124">Int32</span></span>|<span data-ttu-id="9b903-125">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9b903-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9b903-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="9b903-126">defaultStringValue</span></span>|<span data-ttu-id="9b903-127">String</span><span class="sxs-lookup"><span data-stu-id="9b903-127">String</span></span>|<span data-ttu-id="9b903-128">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9b903-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9b903-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="9b903-129">defaultStringArrayValue</span></span>|<span data-ttu-id="9b903-130">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b903-130">String collection</span></span>|<span data-ttu-id="9b903-131">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="9b903-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="9b903-132">dataType</span><span class="sxs-lookup"><span data-stu-id="9b903-132">dataType</span></span>|[<span data-ttu-id="9b903-133">Androidforwork Appconfigurationschemaitemdatatype</span><span class="sxs-lookup"><span data-stu-id="9b903-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="9b903-134">このアイテムが記述する値の種類。</span><span class="sxs-lookup"><span data-stu-id="9b903-134">The type of value this item describes.</span></span> <span data-ttu-id="9b903-135">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="9b903-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="9b903-136">selections</span><span class="sxs-lookup"><span data-stu-id="9b903-136">selections</span></span>|<span data-ttu-id="9b903-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9b903-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9b903-138">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="9b903-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b903-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b903-139">Relationships</span></span>
<span data-ttu-id="9b903-140">なし</span><span class="sxs-lookup"><span data-stu-id="9b903-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b903-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b903-141">JSON Representation</span></span>
<span data-ttu-id="9b903-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b903-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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





