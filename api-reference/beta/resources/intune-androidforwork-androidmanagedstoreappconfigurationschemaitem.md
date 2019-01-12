---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 08c73a177e176ddf82ae64c4eb6b8efd0c662c97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927969"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="043bd-103">androidManagedStoreAppConfigurationSchemaItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="043bd-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="043bd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="043bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="043bd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="043bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="043bd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="043bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="043bd-107">Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。</span><span class="sxs-lookup"><span data-stu-id="043bd-107">Single configuration item inside an Android application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="043bd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="043bd-108">Properties</span></span>
|<span data-ttu-id="043bd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="043bd-109">Property</span></span>|<span data-ttu-id="043bd-110">型</span><span class="sxs-lookup"><span data-stu-id="043bd-110">Type</span></span>|<span data-ttu-id="043bd-111">説明</span><span class="sxs-lookup"><span data-stu-id="043bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="043bd-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="043bd-112">schemaItemKey</span></span>|<span data-ttu-id="043bd-113">String</span><span class="sxs-lookup"><span data-stu-id="043bd-113">String</span></span>|<span data-ttu-id="043bd-114">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="043bd-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="043bd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="043bd-115">displayName</span></span>|<span data-ttu-id="043bd-116">String</span><span class="sxs-lookup"><span data-stu-id="043bd-116">String</span></span>|<span data-ttu-id="043bd-117">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="043bd-117">Human readable name</span></span>|
|<span data-ttu-id="043bd-118">説明</span><span class="sxs-lookup"><span data-stu-id="043bd-118">description</span></span>|<span data-ttu-id="043bd-119">String</span><span class="sxs-lookup"><span data-stu-id="043bd-119">String</span></span>|<span data-ttu-id="043bd-120">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="043bd-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="043bd-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="043bd-121">defaultBoolValue</span></span>|<span data-ttu-id="043bd-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="043bd-122">Boolean</span></span>|<span data-ttu-id="043bd-123">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="043bd-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="043bd-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="043bd-124">defaultIntValue</span></span>|<span data-ttu-id="043bd-125">Int32</span><span class="sxs-lookup"><span data-stu-id="043bd-125">Int32</span></span>|<span data-ttu-id="043bd-126">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="043bd-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="043bd-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="043bd-127">defaultStringValue</span></span>|<span data-ttu-id="043bd-128">String</span><span class="sxs-lookup"><span data-stu-id="043bd-128">String</span></span>|<span data-ttu-id="043bd-129">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="043bd-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="043bd-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="043bd-130">defaultStringArrayValue</span></span>|<span data-ttu-id="043bd-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="043bd-131">String collection</span></span>|<span data-ttu-id="043bd-132">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="043bd-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="043bd-133">dataType</span><span class="sxs-lookup"><span data-stu-id="043bd-133">dataType</span></span>|[<span data-ttu-id="043bd-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="043bd-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="043bd-135">この項目を記述する値の型。</span><span class="sxs-lookup"><span data-stu-id="043bd-135">The type of value this item describes.</span></span> <span data-ttu-id="043bd-136">可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="043bd-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="043bd-137">selections</span><span class="sxs-lookup"><span data-stu-id="043bd-137">selections</span></span>|<span data-ttu-id="043bd-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="043bd-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="043bd-139">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="043bd-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="043bd-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="043bd-140">Relationships</span></span>
<span data-ttu-id="043bd-141">なし</span><span class="sxs-lookup"><span data-stu-id="043bd-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="043bd-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="043bd-142">JSON Representation</span></span>
<span data-ttu-id="043bd-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="043bd-143">Here is a JSON representation of the resource.</span></span>
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





