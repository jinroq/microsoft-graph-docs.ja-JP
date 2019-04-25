---
title: androidForWorkAppConfigurationSchema リソース タイプ
description: Android for Work アプリケーションのカスタム構成を記述するスキーマです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e73da8fba5db59d1b1dc849f67c86ff87a27017c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552771"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a><span data-ttu-id="610f6-103">androidForWorkAppConfigurationSchema リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="610f6-103">androidForWorkAppConfigurationSchema resource type</span></span>

> <span data-ttu-id="610f6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="610f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="610f6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="610f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="610f6-106">Android for Work アプリケーションのカスタム構成を記述するスキーマです。</span><span class="sxs-lookup"><span data-stu-id="610f6-106">Schema describing an Android for Work application's custom configurations.</span></span>

## <a name="methods"></a><span data-ttu-id="610f6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="610f6-107">Methods</span></span>
|<span data-ttu-id="610f6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="610f6-108">Method</span></span>|<span data-ttu-id="610f6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="610f6-109">Return Type</span></span>|<span data-ttu-id="610f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="610f6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="610f6-111">List androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="610f6-111">List androidForWorkAppConfigurationSchemas</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|<span data-ttu-id="610f6-112">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="610f6-112">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="610f6-113">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="610f6-113">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>|
|[<span data-ttu-id="610f6-114">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-114">Get androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[<span data-ttu-id="610f6-115">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-115">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="610f6-116">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="610f6-116">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="610f6-117">Create androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-117">Create androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[<span data-ttu-id="610f6-118">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-118">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="610f6-119">新しい [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="610f6-119">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="610f6-120">Delete androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-120">Delete androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|<span data-ttu-id="610f6-121">なし</span><span class="sxs-lookup"><span data-stu-id="610f6-121">None</span></span>|<span data-ttu-id="610f6-122">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="610f6-122">Deletes a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>|
|[<span data-ttu-id="610f6-123">Update androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-123">Update androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[<span data-ttu-id="610f6-124">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="610f6-124">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="610f6-125">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="610f6-125">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="610f6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="610f6-126">Properties</span></span>
|<span data-ttu-id="610f6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="610f6-127">Property</span></span>|<span data-ttu-id="610f6-128">型</span><span class="sxs-lookup"><span data-stu-id="610f6-128">Type</span></span>|<span data-ttu-id="610f6-129">説明</span><span class="sxs-lookup"><span data-stu-id="610f6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="610f6-130">id</span><span class="sxs-lookup"><span data-stu-id="610f6-130">id</span></span>|<span data-ttu-id="610f6-131">String</span><span class="sxs-lookup"><span data-stu-id="610f6-131">String</span></span>|<span data-ttu-id="610f6-132">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="610f6-132">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="610f6-133">exampleJson</span><span class="sxs-lookup"><span data-stu-id="610f6-133">exampleJson</span></span>|<span data-ttu-id="610f6-134">Binary</span><span class="sxs-lookup"><span data-stu-id="610f6-134">Binary</span></span>|<span data-ttu-id="610f6-135">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="610f6-135">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="610f6-136">schemaItems</span><span class="sxs-lookup"><span data-stu-id="610f6-136">schemaItems</span></span>|<span data-ttu-id="610f6-137">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="610f6-137">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="610f6-138">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="610f6-138">Collection of items each representing a named configuration option in the schema</span></span>|

## <a name="relationships"></a><span data-ttu-id="610f6-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="610f6-139">Relationships</span></span>
<span data-ttu-id="610f6-140">なし</span><span class="sxs-lookup"><span data-stu-id="610f6-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="610f6-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="610f6-141">JSON Representation</span></span>
<span data-ttu-id="610f6-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="610f6-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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
  ]
}
```





