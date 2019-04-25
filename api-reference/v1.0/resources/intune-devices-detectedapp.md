---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a9a31245676dfba465de61aca6527d112ce0b6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542047"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="98282-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98282-104">detectedApp resource type</span></span>

> <span data-ttu-id="98282-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98282-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98282-106">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="98282-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="98282-107">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="98282-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="98282-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="98282-108">Methods</span></span>
|<span data-ttu-id="98282-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="98282-109">Method</span></span>|<span data-ttu-id="98282-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="98282-110">Return Type</span></span>|<span data-ttu-id="98282-111">説明</span><span class="sxs-lookup"><span data-stu-id="98282-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98282-112">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="98282-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="98282-113">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="98282-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="98282-114">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="98282-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="98282-115">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="98282-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="98282-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="98282-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="98282-117">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="98282-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="98282-118">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="98282-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="98282-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="98282-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="98282-120">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="98282-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="98282-121">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="98282-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="98282-122">なし</span><span class="sxs-lookup"><span data-stu-id="98282-122">None</span></span>|<span data-ttu-id="98282-123">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="98282-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="98282-124">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="98282-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="98282-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="98282-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="98282-126">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98282-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98282-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98282-127">Properties</span></span>
|<span data-ttu-id="98282-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98282-128">Property</span></span>|<span data-ttu-id="98282-129">型</span><span class="sxs-lookup"><span data-stu-id="98282-129">Type</span></span>|<span data-ttu-id="98282-130">説明</span><span class="sxs-lookup"><span data-stu-id="98282-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98282-131">id</span><span class="sxs-lookup"><span data-stu-id="98282-131">id</span></span>|<span data-ttu-id="98282-132">String</span><span class="sxs-lookup"><span data-stu-id="98282-132">String</span></span>|<span data-ttu-id="98282-133">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="98282-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="98282-134">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="98282-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="98282-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="98282-135">Read-only.</span></span>|
|<span data-ttu-id="98282-136">displayName</span><span class="sxs-lookup"><span data-stu-id="98282-136">displayName</span></span>|<span data-ttu-id="98282-137">String</span><span class="sxs-lookup"><span data-stu-id="98282-137">String</span></span>|<span data-ttu-id="98282-138">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="98282-138">Name of the discovered application.</span></span> <span data-ttu-id="98282-139">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="98282-139">Read-only</span></span>|
|<span data-ttu-id="98282-140">version</span><span class="sxs-lookup"><span data-stu-id="98282-140">version</span></span>|<span data-ttu-id="98282-141">String</span><span class="sxs-lookup"><span data-stu-id="98282-141">String</span></span>|<span data-ttu-id="98282-142">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="98282-142">Version of the discovered application.</span></span> <span data-ttu-id="98282-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="98282-143">Read-only</span></span>|
|<span data-ttu-id="98282-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="98282-144">sizeInByte</span></span>|<span data-ttu-id="98282-145">Int64</span><span class="sxs-lookup"><span data-stu-id="98282-145">Int64</span></span>|<span data-ttu-id="98282-146">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="98282-146">Discovered application size in bytes.</span></span> <span data-ttu-id="98282-147">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="98282-147">Read-only</span></span>|
|<span data-ttu-id="98282-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="98282-148">deviceCount</span></span>|<span data-ttu-id="98282-149">Int32</span><span class="sxs-lookup"><span data-stu-id="98282-149">Int32</span></span>|<span data-ttu-id="98282-150">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="98282-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="98282-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98282-151">Relationships</span></span>
|<span data-ttu-id="98282-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98282-152">Relationship</span></span>|<span data-ttu-id="98282-153">型</span><span class="sxs-lookup"><span data-stu-id="98282-153">Type</span></span>|<span data-ttu-id="98282-154">説明</span><span class="sxs-lookup"><span data-stu-id="98282-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98282-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="98282-155">managedDevices</span></span>|<span data-ttu-id="98282-156">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="98282-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="98282-157">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="98282-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98282-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98282-158">JSON Representation</span></span>
<span data-ttu-id="98282-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98282-159">Here is a JSON representation of the resource.</span></span>
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



