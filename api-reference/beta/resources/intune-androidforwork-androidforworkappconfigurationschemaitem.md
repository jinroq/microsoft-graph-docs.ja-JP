---
title: androidForWorkAppConfigurationSchemaItem リソース タイプ
description: Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。
localization_priority: Normal
ms.openlocfilehash: 1fb6cb56f754b6d2b100ea2f4d666e31c21efaaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890896"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="42186-103">androidForWorkAppConfigurationSchemaItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="42186-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="42186-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42186-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42186-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42186-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42186-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42186-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42186-107">Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。</span><span class="sxs-lookup"><span data-stu-id="42186-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="42186-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42186-108">Properties</span></span>
|<span data-ttu-id="42186-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42186-109">Property</span></span>|<span data-ttu-id="42186-110">種類</span><span class="sxs-lookup"><span data-stu-id="42186-110">Type</span></span>|<span data-ttu-id="42186-111">説明</span><span class="sxs-lookup"><span data-stu-id="42186-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42186-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="42186-112">schemaItemKey</span></span>|<span data-ttu-id="42186-113">String</span><span class="sxs-lookup"><span data-stu-id="42186-113">String</span></span>|<span data-ttu-id="42186-114">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="42186-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="42186-115">displayName</span><span class="sxs-lookup"><span data-stu-id="42186-115">displayName</span></span>|<span data-ttu-id="42186-116">String</span><span class="sxs-lookup"><span data-stu-id="42186-116">String</span></span>|<span data-ttu-id="42186-117">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="42186-117">Human readable name</span></span>|
|<span data-ttu-id="42186-118">説明</span><span class="sxs-lookup"><span data-stu-id="42186-118">description</span></span>|<span data-ttu-id="42186-119">String</span><span class="sxs-lookup"><span data-stu-id="42186-119">String</span></span>|<span data-ttu-id="42186-120">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="42186-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="42186-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="42186-121">defaultBoolValue</span></span>|<span data-ttu-id="42186-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="42186-122">Boolean</span></span>|<span data-ttu-id="42186-123">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="42186-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="42186-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="42186-124">defaultIntValue</span></span>|<span data-ttu-id="42186-125">Int32</span><span class="sxs-lookup"><span data-stu-id="42186-125">Int32</span></span>|<span data-ttu-id="42186-126">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="42186-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="42186-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="42186-127">defaultStringValue</span></span>|<span data-ttu-id="42186-128">String</span><span class="sxs-lookup"><span data-stu-id="42186-128">String</span></span>|<span data-ttu-id="42186-129">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="42186-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="42186-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="42186-130">defaultStringArrayValue</span></span>|<span data-ttu-id="42186-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="42186-131">String collection</span></span>|<span data-ttu-id="42186-132">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="42186-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="42186-133">dataType</span><span class="sxs-lookup"><span data-stu-id="42186-133">dataType</span></span>|[<span data-ttu-id="42186-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="42186-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="42186-135">この項目を記述する値の型。</span><span class="sxs-lookup"><span data-stu-id="42186-135">The type of value this item describes.</span></span> <span data-ttu-id="42186-136">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="42186-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="42186-137">selections</span><span class="sxs-lookup"><span data-stu-id="42186-137">selections</span></span>|<span data-ttu-id="42186-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42186-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="42186-139">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="42186-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="42186-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42186-140">Relationships</span></span>
<span data-ttu-id="42186-141">なし</span><span class="sxs-lookup"><span data-stu-id="42186-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42186-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42186-142">JSON Representation</span></span>
<span data-ttu-id="42186-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42186-143">Here is a JSON representation of the resource.</span></span>
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





