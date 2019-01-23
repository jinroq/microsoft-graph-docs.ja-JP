---
title: managedMobileApp リソースの種類
description: アプリ展開の識別子。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b8de88976937a967f60a0842eeb9f24b465e50f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419255"
---
# <a name="managedmobileapp-resource-type"></a><span data-ttu-id="6c915-103">managedMobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c915-103">managedMobileApp resource type</span></span>

> <span data-ttu-id="6c915-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c915-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c915-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c915-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c915-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c915-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c915-107">アプリ展開の識別子。</span><span class="sxs-lookup"><span data-stu-id="6c915-107">The identifier for the deployment an app.</span></span>

## <a name="methods"></a><span data-ttu-id="6c915-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c915-108">Methods</span></span>
|<span data-ttu-id="6c915-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c915-109">Method</span></span>|<span data-ttu-id="6c915-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c915-110">Return Type</span></span>|<span data-ttu-id="6c915-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c915-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c915-112">List managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6c915-112">List managedMobileApps</span></span>](../api/intune-mam-managedmobileapp-list.md)|<span data-ttu-id="6c915-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6c915-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="6c915-114">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6c915-114">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>|
|[<span data-ttu-id="6c915-115">Get managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-115">Get managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-get.md)|[<span data-ttu-id="6c915-116">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-116">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="6c915-117">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c915-117">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="6c915-118">Create managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-118">Create managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-create.md)|[<span data-ttu-id="6c915-119">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-119">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="6c915-120">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c915-120">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="6c915-121">Delete managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-121">Delete managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-delete.md)|<span data-ttu-id="6c915-122">なし</span><span class="sxs-lookup"><span data-stu-id="6c915-122">None</span></span>|<span data-ttu-id="6c915-123">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c915-123">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>|
|[<span data-ttu-id="6c915-124">Update managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-124">Update managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-update.md)|[<span data-ttu-id="6c915-125">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6c915-125">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="6c915-126">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c915-126">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c915-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c915-127">Properties</span></span>
|<span data-ttu-id="6c915-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c915-128">Property</span></span>|<span data-ttu-id="6c915-129">型</span><span class="sxs-lookup"><span data-stu-id="6c915-129">Type</span></span>|<span data-ttu-id="6c915-130">説明</span><span class="sxs-lookup"><span data-stu-id="6c915-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c915-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c915-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="6c915-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c915-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6c915-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="6c915-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="6c915-134">id</span><span class="sxs-lookup"><span data-stu-id="6c915-134">id</span></span>|<span data-ttu-id="6c915-135">String</span><span class="sxs-lookup"><span data-stu-id="6c915-135">String</span></span>|<span data-ttu-id="6c915-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6c915-136">Key of the entity.</span></span>|
|<span data-ttu-id="6c915-137">version</span><span class="sxs-lookup"><span data-stu-id="6c915-137">version</span></span>|<span data-ttu-id="6c915-138">String</span><span class="sxs-lookup"><span data-stu-id="6c915-138">String</span></span>|<span data-ttu-id="6c915-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6c915-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c915-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c915-140">Relationships</span></span>
<span data-ttu-id="6c915-141">なし</span><span class="sxs-lookup"><span data-stu-id="6c915-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c915-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c915-142">JSON Representation</span></span>
<span data-ttu-id="6c915-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c915-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




