---
title: androidManagedStoreAppConfigurationSchema リソースの種類
description: Android アプリケーションのカスタム構成を記述するスキーマです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 897e1315b0139d0c99e1ff07899d743b4c701078
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965545"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a><span data-ttu-id="59ad7-103">androidManagedStoreAppConfigurationSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59ad7-103">androidManagedStoreAppConfigurationSchema resource type</span></span>

> <span data-ttu-id="59ad7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59ad7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59ad7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59ad7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59ad7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59ad7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59ad7-107">Android アプリケーションのカスタム構成を記述するスキーマです。</span><span class="sxs-lookup"><span data-stu-id="59ad7-107">Schema describing an Android application's custom configurations.</span></span>
## <a name="methods"></a><span data-ttu-id="59ad7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="59ad7-108">Methods</span></span>
|<span data-ttu-id="59ad7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="59ad7-109">Method</span></span>|<span data-ttu-id="59ad7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59ad7-110">Return Type</span></span>|<span data-ttu-id="59ad7-111">説明</span><span class="sxs-lookup"><span data-stu-id="59ad7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59ad7-112">リスト androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="59ad7-112">List androidManagedStoreAppConfigurationSchemas</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|<span data-ttu-id="59ad7-113">[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="59ad7-113">[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) collection</span></span>|<span data-ttu-id="59ad7-114">[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-114">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>|
|[<span data-ttu-id="59ad7-115">AndroidManagedStoreAppConfigurationSchema を取得します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-115">Get androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[<span data-ttu-id="59ad7-116">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="59ad7-116">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="59ad7-117">[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59ad7-117">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="59ad7-118">AndroidManagedStoreAppConfigurationSchema を作成します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-118">Create androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[<span data-ttu-id="59ad7-119">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="59ad7-119">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="59ad7-120">新しい[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-120">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="59ad7-121">AndroidManagedStoreAppConfigurationSchema を削除します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-121">Delete androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|<span data-ttu-id="59ad7-122">なし</span><span class="sxs-lookup"><span data-stu-id="59ad7-122">None</span></span>|<span data-ttu-id="59ad7-123">の[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-123">Deletes a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>|
|[<span data-ttu-id="59ad7-124">AndroidManagedStoreAppConfigurationSchema を更新します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-124">Update androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[<span data-ttu-id="59ad7-125">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="59ad7-125">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="59ad7-126">[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="59ad7-126">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59ad7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59ad7-127">Properties</span></span>
|<span data-ttu-id="59ad7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59ad7-128">Property</span></span>|<span data-ttu-id="59ad7-129">種類</span><span class="sxs-lookup"><span data-stu-id="59ad7-129">Type</span></span>|<span data-ttu-id="59ad7-130">説明</span><span class="sxs-lookup"><span data-stu-id="59ad7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59ad7-131">ID</span><span class="sxs-lookup"><span data-stu-id="59ad7-131">id</span></span>|<span data-ttu-id="59ad7-132">String</span><span class="sxs-lookup"><span data-stu-id="59ad7-132">String</span></span>|<span data-ttu-id="59ad7-133">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="59ad7-133">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="59ad7-134">exampleJson</span><span class="sxs-lookup"><span data-stu-id="59ad7-134">exampleJson</span></span>|<span data-ttu-id="59ad7-135">Binary</span><span class="sxs-lookup"><span data-stu-id="59ad7-135">Binary</span></span>|<span data-ttu-id="59ad7-136">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="59ad7-136">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="59ad7-137">schemaItems</span><span class="sxs-lookup"><span data-stu-id="59ad7-137">schemaItems</span></span>|<span data-ttu-id="59ad7-138">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="59ad7-138">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="59ad7-139">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="59ad7-139">Collection of items each representing a named configuration option in the schema</span></span>|

## <a name="relationships"></a><span data-ttu-id="59ad7-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59ad7-140">Relationships</span></span>
<span data-ttu-id="59ad7-141">なし</span><span class="sxs-lookup"><span data-stu-id="59ad7-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59ad7-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59ad7-142">JSON Representation</span></span>
<span data-ttu-id="59ad7-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59ad7-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





