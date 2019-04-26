---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01233111e74da95f84d0cbeb81e4675a5c6e049d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552827"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="5d9ab-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d9ab-104">detectedApp resource type</span></span>

> <span data-ttu-id="5d9ab-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d9ab-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d9ab-107">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="5d9ab-108">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="5d9ab-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5d9ab-109">Methods</span></span>
|<span data-ttu-id="5d9ab-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5d9ab-110">Method</span></span>|<span data-ttu-id="5d9ab-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5d9ab-111">Return Type</span></span>|<span data-ttu-id="5d9ab-112">説明</span><span class="sxs-lookup"><span data-stu-id="5d9ab-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5d9ab-113">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="5d9ab-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="5d9ab-114">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5d9ab-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="5d9ab-115">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="5d9ab-116">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="5d9ab-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="5d9ab-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="5d9ab-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="5d9ab-118">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="5d9ab-119">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="5d9ab-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="5d9ab-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="5d9ab-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="5d9ab-121">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="5d9ab-122">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="5d9ab-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="5d9ab-123">なし</span><span class="sxs-lookup"><span data-stu-id="5d9ab-123">None</span></span>|<span data-ttu-id="5d9ab-124">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="5d9ab-125">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="5d9ab-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="5d9ab-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="5d9ab-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="5d9ab-127">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5d9ab-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d9ab-128">Properties</span></span>
|<span data-ttu-id="5d9ab-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d9ab-129">Property</span></span>|<span data-ttu-id="5d9ab-130">型</span><span class="sxs-lookup"><span data-stu-id="5d9ab-130">Type</span></span>|<span data-ttu-id="5d9ab-131">説明</span><span class="sxs-lookup"><span data-stu-id="5d9ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d9ab-132">id</span><span class="sxs-lookup"><span data-stu-id="5d9ab-132">id</span></span>|<span data-ttu-id="5d9ab-133">String</span><span class="sxs-lookup"><span data-stu-id="5d9ab-133">String</span></span>|<span data-ttu-id="5d9ab-134">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="5d9ab-135">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="5d9ab-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-136">Read-only.</span></span>|
|<span data-ttu-id="5d9ab-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5d9ab-137">displayName</span></span>|<span data-ttu-id="5d9ab-138">String</span><span class="sxs-lookup"><span data-stu-id="5d9ab-138">String</span></span>|<span data-ttu-id="5d9ab-139">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-139">Name of the discovered application.</span></span> <span data-ttu-id="5d9ab-140">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="5d9ab-140">Read-only</span></span>|
|<span data-ttu-id="5d9ab-141">version</span><span class="sxs-lookup"><span data-stu-id="5d9ab-141">version</span></span>|<span data-ttu-id="5d9ab-142">String</span><span class="sxs-lookup"><span data-stu-id="5d9ab-142">String</span></span>|<span data-ttu-id="5d9ab-143">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-143">Version of the discovered application.</span></span> <span data-ttu-id="5d9ab-144">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="5d9ab-144">Read-only</span></span>|
|<span data-ttu-id="5d9ab-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="5d9ab-145">sizeInByte</span></span>|<span data-ttu-id="5d9ab-146">Int64</span><span class="sxs-lookup"><span data-stu-id="5d9ab-146">Int64</span></span>|<span data-ttu-id="5d9ab-147">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-147">Discovered application size in bytes.</span></span> <span data-ttu-id="5d9ab-148">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="5d9ab-148">Read-only</span></span>|
|<span data-ttu-id="5d9ab-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5d9ab-149">deviceCount</span></span>|<span data-ttu-id="5d9ab-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5d9ab-150">Int32</span></span>|<span data-ttu-id="5d9ab-151">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5d9ab-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d9ab-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d9ab-152">Relationships</span></span>
|<span data-ttu-id="5d9ab-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d9ab-153">Relationship</span></span>|<span data-ttu-id="5d9ab-154">型</span><span class="sxs-lookup"><span data-stu-id="5d9ab-154">Type</span></span>|<span data-ttu-id="5d9ab-155">説明</span><span class="sxs-lookup"><span data-stu-id="5d9ab-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d9ab-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="5d9ab-156">managedDevices</span></span>|<span data-ttu-id="5d9ab-157">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5d9ab-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="5d9ab-158">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="5d9ab-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d9ab-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d9ab-159">JSON Representation</span></span>
<span data-ttu-id="5d9ab-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5d9ab-160">Here is a JSON representation of the resource.</span></span>
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





