---
title: cartToClassAssociation リソースの種類
description: 教室カートのデバイスに関連付けるための CartToClassAssociation です。
author: tfitzmac
ms.openlocfilehash: f712759d82b5edf7d364658211f1f2142fb6eb87
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328281"
---
# <a name="carttoclassassociation-resource-type"></a><span data-ttu-id="5df24-103">cartToClassAssociation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5df24-103">cartToClassAssociation resource type</span></span>

> <span data-ttu-id="5df24-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5df24-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5df24-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5df24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5df24-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5df24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5df24-107">教室カートのデバイスに関連付けるための CartToClassAssociation です。</span><span class="sxs-lookup"><span data-stu-id="5df24-107">CartToClassAssociation for associating device carts with classrooms.</span></span>
## <a name="methods"></a><span data-ttu-id="5df24-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5df24-108">Methods</span></span>
|<span data-ttu-id="5df24-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5df24-109">Method</span></span>|<span data-ttu-id="5df24-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5df24-110">Return Type</span></span>|<span data-ttu-id="5df24-111">説明</span><span class="sxs-lookup"><span data-stu-id="5df24-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5df24-112">リスト cartToClassAssociations</span><span class="sxs-lookup"><span data-stu-id="5df24-112">List cartToClassAssociations</span></span>](../api/intune-deviceconfig-carttoclassassociation-list.md)|<span data-ttu-id="5df24-113">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5df24-113">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) collection</span></span>|<span data-ttu-id="5df24-114">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5df24-114">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>|
|[<span data-ttu-id="5df24-115">CartToClassAssociation を取得します。</span><span class="sxs-lookup"><span data-stu-id="5df24-115">Get cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-get.md)|[<span data-ttu-id="5df24-116">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="5df24-116">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="5df24-117">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5df24-117">Read properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="5df24-118">CartToClassAssociation を作成します。</span><span class="sxs-lookup"><span data-stu-id="5df24-118">Create cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-create.md)|[<span data-ttu-id="5df24-119">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="5df24-119">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="5df24-120">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5df24-120">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|
|[<span data-ttu-id="5df24-121">CartToClassAssociation を削除します。</span><span class="sxs-lookup"><span data-stu-id="5df24-121">Delete cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-delete.md)|<span data-ttu-id="5df24-122">なし</span><span class="sxs-lookup"><span data-stu-id="5df24-122">None</span></span>|<span data-ttu-id="5df24-123">の[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5df24-123">Deletes a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>|
|[<span data-ttu-id="5df24-124">CartToClassAssociation を更新します。</span><span class="sxs-lookup"><span data-stu-id="5df24-124">Update cartToClassAssociation</span></span>](../api/intune-deviceconfig-carttoclassassociation-update.md)|[<span data-ttu-id="5df24-125">cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="5df24-125">cartToClassAssociation</span></span>](../resources/intune-deviceconfig-carttoclassassociation.md)|<span data-ttu-id="5df24-126">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5df24-126">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5df24-127">Properties</span><span class="sxs-lookup"><span data-stu-id="5df24-127">Properties</span></span>
|<span data-ttu-id="5df24-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5df24-128">Property</span></span>|<span data-ttu-id="5df24-129">種類</span><span class="sxs-lookup"><span data-stu-id="5df24-129">Type</span></span>|<span data-ttu-id="5df24-130">説明</span><span class="sxs-lookup"><span data-stu-id="5df24-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df24-131">ID</span><span class="sxs-lookup"><span data-stu-id="5df24-131">id</span></span>|<span data-ttu-id="5df24-132">String</span><span class="sxs-lookup"><span data-stu-id="5df24-132">String</span></span>|<span data-ttu-id="5df24-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5df24-133">Key of the entity.</span></span>|
|<span data-ttu-id="5df24-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5df24-134">createdDateTime</span></span>|<span data-ttu-id="5df24-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df24-135">DateTimeOffset</span></span>|<span data-ttu-id="5df24-136">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5df24-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="5df24-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5df24-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5df24-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df24-138">DateTimeOffset</span></span>|<span data-ttu-id="5df24-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5df24-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5df24-140">version</span><span class="sxs-lookup"><span data-stu-id="5df24-140">version</span></span>|<span data-ttu-id="5df24-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5df24-141">Int32</span></span>|<span data-ttu-id="5df24-142">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="5df24-142">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5df24-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5df24-143">displayName</span></span>|<span data-ttu-id="5df24-144">String</span><span class="sxs-lookup"><span data-stu-id="5df24-144">String</span></span>|<span data-ttu-id="5df24-145">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="5df24-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5df24-146">説明</span><span class="sxs-lookup"><span data-stu-id="5df24-146">description</span></span>|<span data-ttu-id="5df24-147">String</span><span class="sxs-lookup"><span data-stu-id="5df24-147">String</span></span>|<span data-ttu-id="5df24-148">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="5df24-148">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5df24-149">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="5df24-149">deviceCartIds</span></span>|<span data-ttu-id="5df24-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5df24-150">String collection</span></span>|<span data-ttu-id="5df24-151">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="5df24-151">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="5df24-152">classroomIds</span><span class="sxs-lookup"><span data-stu-id="5df24-152">classroomIds</span></span>|<span data-ttu-id="5df24-153">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5df24-153">String collection</span></span>|<span data-ttu-id="5df24-154">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5df24-154">Identifiers of classrooms to be associated with device carts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df24-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5df24-155">Relationships</span></span>
<span data-ttu-id="5df24-156">なし</span><span class="sxs-lookup"><span data-stu-id="5df24-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5df24-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5df24-157">JSON Representation</span></span>
<span data-ttu-id="5df24-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5df24-158">Here is a JSON representation of the resource.</span></span>
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





