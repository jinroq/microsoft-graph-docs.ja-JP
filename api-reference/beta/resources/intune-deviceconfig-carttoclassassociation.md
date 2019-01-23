---
title: cartToClassAssociation リソースの種類
description: 教室カートのデバイスに関連付けるための CartToClassAssociation です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b832e4597b15f062289a086d068ea3da71d9f66a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395693"
---
# <a name="carttoclassassociation-resource-type"></a><span data-ttu-id="421e2-103">cartToClassAssociation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="421e2-103">cartToClassAssociation resource type</span></span>

> <span data-ttu-id="421e2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="421e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="421e2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="421e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="421e2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="421e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421e2-107">教室カートのデバイスに関連付けるための CartToClassAssociation です。</span><span class="sxs-lookup"><span data-stu-id="421e2-107">CartToClassAssociation for associating device carts with classrooms.</span></span>

## <a name="methods"></a><span data-ttu-id="421e2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="421e2-108">Methods</span></span>
|<span data-ttu-id="421e2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="421e2-109">Method</span></span>|<span data-ttu-id="421e2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="421e2-110">Return Type</span></span>|<span data-ttu-id="421e2-111">説明</span><span class="sxs-lookup"><span data-stu-id="421e2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="421e2-112">リスト cartToClassAssociations</span><span class="sxs-lookup"><span data-stu-id="421e2-112">List cartToClassAssociations</span></span>](../api/intune-deviceconfig-carttoclassassociation-list.md)|<span data-ttu-id="421e2-113">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="421e2-113">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) collection</span></span>|<span data-ttu-id="421e2-114">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="421e2-114">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>|
|[<span data-ttu-id="421e2-115">CartToClassAssociation を取得します。</span><span class="sxs-lookup"><span data-stu-id="421e2-115">Get cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-get.md)|[<span data-ttu-id="421e2-116">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="421e2-116">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="421e2-117">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="421e2-117">Read properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="421e2-118">CartToClassAssociation を作成します。</span><span class="sxs-lookup"><span data-stu-id="421e2-118">Create cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-create.md)|[<span data-ttu-id="421e2-119">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="421e2-119">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="421e2-120">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="421e2-120">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="421e2-121">CartToClassAssociation を削除します。</span><span class="sxs-lookup"><span data-stu-id="421e2-121">Delete cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-delete.md)|<span data-ttu-id="421e2-122">なし</span><span class="sxs-lookup"><span data-stu-id="421e2-122">None</span></span>|<span data-ttu-id="421e2-123">の[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="421e2-123">Deletes a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>|
|[<span data-ttu-id="421e2-124">CartToClassAssociation を更新します。</span><span class="sxs-lookup"><span data-stu-id="421e2-124">Update cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-update.md)|[<span data-ttu-id="421e2-125">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="421e2-125">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="421e2-126">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="421e2-126">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="421e2-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="421e2-127">Properties</span></span>
|<span data-ttu-id="421e2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="421e2-128">Property</span></span>|<span data-ttu-id="421e2-129">型</span><span class="sxs-lookup"><span data-stu-id="421e2-129">Type</span></span>|<span data-ttu-id="421e2-130">説明</span><span class="sxs-lookup"><span data-stu-id="421e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421e2-131">id</span><span class="sxs-lookup"><span data-stu-id="421e2-131">id</span></span>|<span data-ttu-id="421e2-132">String</span><span class="sxs-lookup"><span data-stu-id="421e2-132">String</span></span>|<span data-ttu-id="421e2-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="421e2-133">Key of the entity.</span></span>|
|<span data-ttu-id="421e2-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="421e2-134">createdDateTime</span></span>|<span data-ttu-id="421e2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421e2-135">DateTimeOffset</span></span>|<span data-ttu-id="421e2-136">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="421e2-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="421e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="421e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="421e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421e2-138">DateTimeOffset</span></span>|<span data-ttu-id="421e2-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="421e2-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="421e2-140">version</span><span class="sxs-lookup"><span data-stu-id="421e2-140">version</span></span>|<span data-ttu-id="421e2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="421e2-141">Int32</span></span>|<span data-ttu-id="421e2-142">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="421e2-142">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="421e2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="421e2-143">displayName</span></span>|<span data-ttu-id="421e2-144">String</span><span class="sxs-lookup"><span data-stu-id="421e2-144">String</span></span>|<span data-ttu-id="421e2-145">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="421e2-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="421e2-146">説明</span><span class="sxs-lookup"><span data-stu-id="421e2-146">description</span></span>|<span data-ttu-id="421e2-147">String</span><span class="sxs-lookup"><span data-stu-id="421e2-147">String</span></span>|<span data-ttu-id="421e2-148">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="421e2-148">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="421e2-149">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="421e2-149">deviceCartIds</span></span>|<span data-ttu-id="421e2-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="421e2-150">String collection</span></span>|<span data-ttu-id="421e2-151">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="421e2-151">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="421e2-152">classroomIds</span><span class="sxs-lookup"><span data-stu-id="421e2-152">classroomIds</span></span>|<span data-ttu-id="421e2-153">String コレクション</span><span class="sxs-lookup"><span data-stu-id="421e2-153">String collection</span></span>|<span data-ttu-id="421e2-154">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="421e2-154">Identifiers of classrooms to be associated with device carts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="421e2-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="421e2-155">Relationships</span></span>
<span data-ttu-id="421e2-156">なし</span><span class="sxs-lookup"><span data-stu-id="421e2-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="421e2-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="421e2-157">JSON Representation</span></span>
<span data-ttu-id="421e2-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="421e2-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```




