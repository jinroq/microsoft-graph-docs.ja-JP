---
title: cartToClassAssociation リソースの種類
description: デバイスカートと教室を関連付けるための CartToClassAssociation。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b756e4b9f5bd00a812eba65948c415a5f0719c20
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549546"
---
# <a name="carttoclassassociation-resource-type"></a><span data-ttu-id="22ef1-103">cartToClassAssociation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22ef1-103">cartToClassAssociation resource type</span></span>

> <span data-ttu-id="22ef1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ef1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ef1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22ef1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ef1-106">デバイスカートと教室を関連付けるための CartToClassAssociation。</span><span class="sxs-lookup"><span data-stu-id="22ef1-106">CartToClassAssociation for associating device carts with classrooms.</span></span>

## <a name="methods"></a><span data-ttu-id="22ef1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="22ef1-107">Methods</span></span>
|<span data-ttu-id="22ef1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="22ef1-108">Method</span></span>|<span data-ttu-id="22ef1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22ef1-109">Return Type</span></span>|<span data-ttu-id="22ef1-110">説明</span><span class="sxs-lookup"><span data-stu-id="22ef1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22ef1-111">リスト cartToClassAssociations</span><span class="sxs-lookup"><span data-stu-id="22ef1-111">List cartToClassAssociations</span></span>](../api/intune-deviceconfig-carttoclassassociation-list.md)|<span data-ttu-id="22ef1-112">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22ef1-112">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) collection</span></span>|<span data-ttu-id="22ef1-113">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="22ef1-113">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>|
|[<span data-ttu-id="22ef1-114">cartToClassAssociation を取得する</span><span class="sxs-lookup"><span data-stu-id="22ef1-114">Get cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-get.md)|[<span data-ttu-id="22ef1-115">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="22ef1-115">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="22ef1-116">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="22ef1-116">Read properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="22ef1-117">cartToClassAssociation を作成する</span><span class="sxs-lookup"><span data-stu-id="22ef1-117">Create cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-create.md)|[<span data-ttu-id="22ef1-118">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="22ef1-118">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="22ef1-119">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-119">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="22ef1-120">cartToClassAssociation の削除</span><span class="sxs-lookup"><span data-stu-id="22ef1-120">Delete cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-delete.md)|<span data-ttu-id="22ef1-121">なし</span><span class="sxs-lookup"><span data-stu-id="22ef1-121">None</span></span>|<span data-ttu-id="22ef1-122">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-122">Deletes a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>|
|[<span data-ttu-id="22ef1-123">cartToClassAssociation の更新</span><span class="sxs-lookup"><span data-stu-id="22ef1-123">Update cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-update.md)|[<span data-ttu-id="22ef1-124">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="22ef1-124">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="22ef1-125">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-125">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22ef1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ef1-126">Properties</span></span>
|<span data-ttu-id="22ef1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ef1-127">Property</span></span>|<span data-ttu-id="22ef1-128">型</span><span class="sxs-lookup"><span data-stu-id="22ef1-128">Type</span></span>|<span data-ttu-id="22ef1-129">説明</span><span class="sxs-lookup"><span data-stu-id="22ef1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ef1-130">id</span><span class="sxs-lookup"><span data-stu-id="22ef1-130">id</span></span>|<span data-ttu-id="22ef1-131">String</span><span class="sxs-lookup"><span data-stu-id="22ef1-131">String</span></span>|<span data-ttu-id="22ef1-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22ef1-132">Key of the entity.</span></span>|
|<span data-ttu-id="22ef1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22ef1-133">createdDateTime</span></span>|<span data-ttu-id="22ef1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef1-134">DateTimeOffset</span></span>|<span data-ttu-id="22ef1-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="22ef1-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="22ef1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22ef1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="22ef1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef1-137">DateTimeOffset</span></span>|<span data-ttu-id="22ef1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="22ef1-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="22ef1-139">version</span><span class="sxs-lookup"><span data-stu-id="22ef1-139">version</span></span>|<span data-ttu-id="22ef1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="22ef1-140">Int32</span></span>|<span data-ttu-id="22ef1-141">CartToClassAssociation のバージョン。</span><span class="sxs-lookup"><span data-stu-id="22ef1-141">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="22ef1-142">displayName</span><span class="sxs-lookup"><span data-stu-id="22ef1-142">displayName</span></span>|<span data-ttu-id="22ef1-143">String</span><span class="sxs-lookup"><span data-stu-id="22ef1-143">String</span></span>|<span data-ttu-id="22ef1-144">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="22ef1-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="22ef1-145">description</span><span class="sxs-lookup"><span data-stu-id="22ef1-145">description</span></span>|<span data-ttu-id="22ef1-146">String</span><span class="sxs-lookup"><span data-stu-id="22ef1-146">String</span></span>|<span data-ttu-id="22ef1-147">CartToClassAssociation の管理者提供の説明。</span><span class="sxs-lookup"><span data-stu-id="22ef1-147">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="22ef1-148">devicecartids</span><span class="sxs-lookup"><span data-stu-id="22ef1-148">deviceCartIds</span></span>|<span data-ttu-id="22ef1-149">String collection</span><span class="sxs-lookup"><span data-stu-id="22ef1-149">String collection</span></span>|<span data-ttu-id="22ef1-150">クラスに関連付けられるデバイスカートの識別子。</span><span class="sxs-lookup"><span data-stu-id="22ef1-150">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="22ef1-151">classroomIds</span><span class="sxs-lookup"><span data-stu-id="22ef1-151">classroomIds</span></span>|<span data-ttu-id="22ef1-152">String collection</span><span class="sxs-lookup"><span data-stu-id="22ef1-152">String collection</span></span>|<span data-ttu-id="22ef1-153">デバイスカートに関連付ける教室の識別子。</span><span class="sxs-lookup"><span data-stu-id="22ef1-153">Identifiers of classrooms to be associated with device carts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22ef1-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22ef1-154">Relationships</span></span>
<span data-ttu-id="22ef1-155">なし</span><span class="sxs-lookup"><span data-stu-id="22ef1-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22ef1-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22ef1-156">JSON Representation</span></span>
<span data-ttu-id="22ef1-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22ef1-157">Here is a JSON representation of the resource.</span></span>
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





