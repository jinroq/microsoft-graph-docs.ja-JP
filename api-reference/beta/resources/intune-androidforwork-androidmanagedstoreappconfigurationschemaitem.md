---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 706a4daa53201f8bdf295ca26ecf6f20134437da
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991416"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="5c4dc-103">androidManagedStoreAppConfigurationSchemaItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c4dc-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="5c4dc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c4dc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c4dc-106">Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="5c4dc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c4dc-107">Properties</span></span>
|<span data-ttu-id="5c4dc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c4dc-108">Property</span></span>|<span data-ttu-id="5c4dc-109">型</span><span class="sxs-lookup"><span data-stu-id="5c4dc-109">Type</span></span>|<span data-ttu-id="5c4dc-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c4dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c4dc-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="5c4dc-111">schemaItemKey</span></span>|<span data-ttu-id="5c4dc-112">String</span><span class="sxs-lookup"><span data-stu-id="5c4dc-112">String</span></span>|<span data-ttu-id="5c4dc-113">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="5c4dc-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="5c4dc-114">displayName</span><span class="sxs-lookup"><span data-stu-id="5c4dc-114">displayName</span></span>|<span data-ttu-id="5c4dc-115">String</span><span class="sxs-lookup"><span data-stu-id="5c4dc-115">String</span></span>|<span data-ttu-id="5c4dc-116">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="5c4dc-116">Human readable name</span></span>|
|<span data-ttu-id="5c4dc-117">description</span><span class="sxs-lookup"><span data-stu-id="5c4dc-117">description</span></span>|<span data-ttu-id="5c4dc-118">String</span><span class="sxs-lookup"><span data-stu-id="5c4dc-118">String</span></span>|<span data-ttu-id="5c4dc-119">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="5c4dc-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="5c4dc-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="5c4dc-120">defaultBoolValue</span></span>|<span data-ttu-id="5c4dc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c4dc-121">Boolean</span></span>|<span data-ttu-id="5c4dc-122">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="5c4dc-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5c4dc-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="5c4dc-123">defaultIntValue</span></span>|<span data-ttu-id="5c4dc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4dc-124">Int32</span></span>|<span data-ttu-id="5c4dc-125">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="5c4dc-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5c4dc-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="5c4dc-126">defaultStringValue</span></span>|<span data-ttu-id="5c4dc-127">String</span><span class="sxs-lookup"><span data-stu-id="5c4dc-127">String</span></span>|<span data-ttu-id="5c4dc-128">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="5c4dc-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5c4dc-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="5c4dc-129">defaultStringArrayValue</span></span>|<span data-ttu-id="5c4dc-130">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5c4dc-130">String collection</span></span>|<span data-ttu-id="5c4dc-131">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="5c4dc-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="5c4dc-132">dataType</span><span class="sxs-lookup"><span data-stu-id="5c4dc-132">dataType</span></span>|[<span data-ttu-id="5c4dc-133">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="5c4dc-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="5c4dc-134">このアイテムが記述する値の種類。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-134">The type of value this item describes.</span></span> <span data-ttu-id="5c4dc-135">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="5c4dc-136">selections</span><span class="sxs-lookup"><span data-stu-id="5c4dc-136">selections</span></span>|<span data-ttu-id="5c4dc-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5c4dc-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5c4dc-138">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="5c4dc-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c4dc-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5c4dc-139">Relationships</span></span>
<span data-ttu-id="5c4dc-140">なし</span><span class="sxs-lookup"><span data-stu-id="5c4dc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c4dc-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c4dc-141">JSON Representation</span></span>
<span data-ttu-id="5c4dc-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c4dc-142">Here is a JSON representation of the resource.</span></span>
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





