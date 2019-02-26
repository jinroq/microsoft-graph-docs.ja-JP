---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a9a31245676dfba465de61aca6527d112ce0b6d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252603"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="ec137-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec137-104">detectedApp resource type</span></span>

> <span data-ttu-id="ec137-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec137-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec137-106">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="ec137-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="ec137-107">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="ec137-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="ec137-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec137-108">Methods</span></span>
|<span data-ttu-id="ec137-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec137-109">Method</span></span>|<span data-ttu-id="ec137-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ec137-110">Return Type</span></span>|<span data-ttu-id="ec137-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec137-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec137-112">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="ec137-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="ec137-113">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ec137-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="ec137-114">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ec137-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="ec137-115">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="ec137-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="ec137-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="ec137-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="ec137-117">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ec137-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="ec137-118">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="ec137-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="ec137-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="ec137-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="ec137-120">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ec137-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="ec137-121">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="ec137-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="ec137-122">なし</span><span class="sxs-lookup"><span data-stu-id="ec137-122">None</span></span>|<span data-ttu-id="ec137-123">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ec137-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="ec137-124">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="ec137-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="ec137-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="ec137-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="ec137-126">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec137-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec137-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec137-127">Properties</span></span>
|<span data-ttu-id="ec137-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec137-128">Property</span></span>|<span data-ttu-id="ec137-129">型</span><span class="sxs-lookup"><span data-stu-id="ec137-129">Type</span></span>|<span data-ttu-id="ec137-130">説明</span><span class="sxs-lookup"><span data-stu-id="ec137-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec137-131">id</span><span class="sxs-lookup"><span data-stu-id="ec137-131">id</span></span>|<span data-ttu-id="ec137-132">文字列</span><span class="sxs-lookup"><span data-stu-id="ec137-132">String</span></span>|<span data-ttu-id="ec137-133">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ec137-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="ec137-134">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="ec137-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="ec137-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ec137-135">Read-only.</span></span>|
|<span data-ttu-id="ec137-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ec137-136">displayName</span></span>|<span data-ttu-id="ec137-137">String</span><span class="sxs-lookup"><span data-stu-id="ec137-137">String</span></span>|<span data-ttu-id="ec137-138">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="ec137-138">Name of the discovered application.</span></span> <span data-ttu-id="ec137-139">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="ec137-139">Read-only</span></span>|
|<span data-ttu-id="ec137-140">version</span><span class="sxs-lookup"><span data-stu-id="ec137-140">version</span></span>|<span data-ttu-id="ec137-141">String</span><span class="sxs-lookup"><span data-stu-id="ec137-141">String</span></span>|<span data-ttu-id="ec137-142">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ec137-142">Version of the discovered application.</span></span> <span data-ttu-id="ec137-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="ec137-143">Read-only</span></span>|
|<span data-ttu-id="ec137-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="ec137-144">sizeInByte</span></span>|<span data-ttu-id="ec137-145">Int64</span><span class="sxs-lookup"><span data-stu-id="ec137-145">Int64</span></span>|<span data-ttu-id="ec137-146">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="ec137-146">Discovered application size in bytes.</span></span> <span data-ttu-id="ec137-147">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="ec137-147">Read-only</span></span>|
|<span data-ttu-id="ec137-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ec137-148">deviceCount</span></span>|<span data-ttu-id="ec137-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ec137-149">Int32</span></span>|<span data-ttu-id="ec137-150">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ec137-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec137-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec137-151">Relationships</span></span>
|<span data-ttu-id="ec137-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec137-152">Relationship</span></span>|<span data-ttu-id="ec137-153">型</span><span class="sxs-lookup"><span data-stu-id="ec137-153">Type</span></span>|<span data-ttu-id="ec137-154">説明</span><span class="sxs-lookup"><span data-stu-id="ec137-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec137-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="ec137-155">managedDevices</span></span>|<span data-ttu-id="ec137-156">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ec137-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="ec137-157">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="ec137-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec137-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec137-158">JSON Representation</span></span>
<span data-ttu-id="ec137-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ec137-159">Here is a JSON representation of the resource.</span></span>
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



