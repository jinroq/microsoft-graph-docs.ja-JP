---
title: androidForWorkAppConfigurationSchemaItem リソース タイプ
description: Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7e8500df3065c68ae8ddc2ad85413aa4d31f8980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923454"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="a90ff-103">androidForWorkAppConfigurationSchemaItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a90ff-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="a90ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a90ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a90ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a90ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a90ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a90ff-107">Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。</span><span class="sxs-lookup"><span data-stu-id="a90ff-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="a90ff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a90ff-108">Properties</span></span>
|<span data-ttu-id="a90ff-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a90ff-109">Property</span></span>|<span data-ttu-id="a90ff-110">種類</span><span class="sxs-lookup"><span data-stu-id="a90ff-110">Type</span></span>|<span data-ttu-id="a90ff-111">説明</span><span class="sxs-lookup"><span data-stu-id="a90ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a90ff-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="a90ff-112">schemaItemKey</span></span>|<span data-ttu-id="a90ff-113">String</span><span class="sxs-lookup"><span data-stu-id="a90ff-113">String</span></span>|<span data-ttu-id="a90ff-114">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="a90ff-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="a90ff-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a90ff-115">displayName</span></span>|<span data-ttu-id="a90ff-116">String</span><span class="sxs-lookup"><span data-stu-id="a90ff-116">String</span></span>|<span data-ttu-id="a90ff-117">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="a90ff-117">Human readable name</span></span>|
|<span data-ttu-id="a90ff-118">説明</span><span class="sxs-lookup"><span data-stu-id="a90ff-118">description</span></span>|<span data-ttu-id="a90ff-119">String</span><span class="sxs-lookup"><span data-stu-id="a90ff-119">String</span></span>|<span data-ttu-id="a90ff-120">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="a90ff-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="a90ff-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="a90ff-121">defaultBoolValue</span></span>|<span data-ttu-id="a90ff-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a90ff-122">Boolean</span></span>|<span data-ttu-id="a90ff-123">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a90ff-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a90ff-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="a90ff-124">defaultIntValue</span></span>|<span data-ttu-id="a90ff-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a90ff-125">Int32</span></span>|<span data-ttu-id="a90ff-126">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a90ff-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a90ff-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="a90ff-127">defaultStringValue</span></span>|<span data-ttu-id="a90ff-128">String</span><span class="sxs-lookup"><span data-stu-id="a90ff-128">String</span></span>|<span data-ttu-id="a90ff-129">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a90ff-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a90ff-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="a90ff-130">defaultStringArrayValue</span></span>|<span data-ttu-id="a90ff-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a90ff-131">String collection</span></span>|<span data-ttu-id="a90ff-132">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="a90ff-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="a90ff-133">dataType</span><span class="sxs-lookup"><span data-stu-id="a90ff-133">dataType</span></span>|[<span data-ttu-id="a90ff-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="a90ff-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="a90ff-135">この項目を記述する値の型。</span><span class="sxs-lookup"><span data-stu-id="a90ff-135">The type of value this item describes.</span></span> <span data-ttu-id="a90ff-136">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="a90ff-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="a90ff-137">selections</span><span class="sxs-lookup"><span data-stu-id="a90ff-137">selections</span></span>|<span data-ttu-id="a90ff-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a90ff-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a90ff-139">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="a90ff-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a90ff-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a90ff-140">Relationships</span></span>
<span data-ttu-id="a90ff-141">なし</span><span class="sxs-lookup"><span data-stu-id="a90ff-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a90ff-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a90ff-142">JSON Representation</span></span>
<span data-ttu-id="a90ff-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a90ff-143">Here is a JSON representation of the resource.</span></span>
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





