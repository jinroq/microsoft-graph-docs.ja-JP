---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cba801689cb5051926a3139574d5a27294090a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403099"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="d55cf-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d55cf-104">detectedApp resource type</span></span>

> <span data-ttu-id="d55cf-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d55cf-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d55cf-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d55cf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d55cf-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d55cf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d55cf-108">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="d55cf-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="d55cf-109">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="d55cf-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="d55cf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d55cf-110">Methods</span></span>
|<span data-ttu-id="d55cf-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d55cf-111">Method</span></span>|<span data-ttu-id="d55cf-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d55cf-112">Return Type</span></span>|<span data-ttu-id="d55cf-113">説明</span><span class="sxs-lookup"><span data-stu-id="d55cf-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d55cf-114">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="d55cf-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="d55cf-115">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d55cf-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="d55cf-116">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d55cf-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="d55cf-117">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="d55cf-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="d55cf-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d55cf-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d55cf-119">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d55cf-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d55cf-120">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="d55cf-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="d55cf-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d55cf-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d55cf-122">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d55cf-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d55cf-123">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="d55cf-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="d55cf-124">なし</span><span class="sxs-lookup"><span data-stu-id="d55cf-124">None</span></span>|<span data-ttu-id="d55cf-125">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d55cf-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="d55cf-126">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="d55cf-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="d55cf-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d55cf-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d55cf-128">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d55cf-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d55cf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d55cf-129">Properties</span></span>
|<span data-ttu-id="d55cf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d55cf-130">Property</span></span>|<span data-ttu-id="d55cf-131">型</span><span class="sxs-lookup"><span data-stu-id="d55cf-131">Type</span></span>|<span data-ttu-id="d55cf-132">説明</span><span class="sxs-lookup"><span data-stu-id="d55cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d55cf-133">id</span><span class="sxs-lookup"><span data-stu-id="d55cf-133">id</span></span>|<span data-ttu-id="d55cf-134">String</span><span class="sxs-lookup"><span data-stu-id="d55cf-134">String</span></span>|<span data-ttu-id="d55cf-135">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d55cf-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="d55cf-136">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="d55cf-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="d55cf-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d55cf-137">Read-only.</span></span>|
|<span data-ttu-id="d55cf-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d55cf-138">displayName</span></span>|<span data-ttu-id="d55cf-139">String</span><span class="sxs-lookup"><span data-stu-id="d55cf-139">String</span></span>|<span data-ttu-id="d55cf-140">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="d55cf-140">Name of the discovered application.</span></span> <span data-ttu-id="d55cf-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="d55cf-141">Read-only</span></span>|
|<span data-ttu-id="d55cf-142">version</span><span class="sxs-lookup"><span data-stu-id="d55cf-142">version</span></span>|<span data-ttu-id="d55cf-143">String</span><span class="sxs-lookup"><span data-stu-id="d55cf-143">String</span></span>|<span data-ttu-id="d55cf-144">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d55cf-144">Version of the discovered application.</span></span> <span data-ttu-id="d55cf-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="d55cf-145">Read-only</span></span>|
|<span data-ttu-id="d55cf-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="d55cf-146">sizeInByte</span></span>|<span data-ttu-id="d55cf-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d55cf-147">Int64</span></span>|<span data-ttu-id="d55cf-148">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="d55cf-148">Discovered application size in bytes.</span></span> <span data-ttu-id="d55cf-149">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="d55cf-149">Read-only</span></span>|
|<span data-ttu-id="d55cf-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d55cf-150">deviceCount</span></span>|<span data-ttu-id="d55cf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d55cf-151">Int32</span></span>|<span data-ttu-id="d55cf-152">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d55cf-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d55cf-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d55cf-153">Relationships</span></span>
|<span data-ttu-id="d55cf-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d55cf-154">Relationship</span></span>|<span data-ttu-id="d55cf-155">型</span><span class="sxs-lookup"><span data-stu-id="d55cf-155">Type</span></span>|<span data-ttu-id="d55cf-156">説明</span><span class="sxs-lookup"><span data-stu-id="d55cf-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d55cf-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d55cf-157">managedDevices</span></span>|<span data-ttu-id="d55cf-158">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d55cf-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="d55cf-159">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="d55cf-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d55cf-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d55cf-160">JSON Representation</span></span>
<span data-ttu-id="d55cf-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d55cf-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```




