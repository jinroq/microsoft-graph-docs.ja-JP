---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: tfitzmac
ms.openlocfilehash: 0b8e234651c0936fea71d8420b30fcc5d1c6fb7a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356897"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="7181d-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7181d-104">detectedApp resource type</span></span>

> <span data-ttu-id="7181d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7181d-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7181d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7181d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7181d-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7181d-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7181d-108">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="7181d-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="7181d-109">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="7181d-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="7181d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="7181d-110">Methods</span></span>
|<span data-ttu-id="7181d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="7181d-111">Method</span></span>|<span data-ttu-id="7181d-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7181d-112">Return Type</span></span>|<span data-ttu-id="7181d-113">説明</span><span class="sxs-lookup"><span data-stu-id="7181d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7181d-114">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="7181d-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="7181d-115">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7181d-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="7181d-116">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7181d-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="7181d-117">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="7181d-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="7181d-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7181d-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7181d-119">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7181d-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="7181d-120">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="7181d-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="7181d-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7181d-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7181d-122">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7181d-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="7181d-123">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="7181d-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="7181d-124">なし</span><span class="sxs-lookup"><span data-stu-id="7181d-124">None</span></span>|<span data-ttu-id="7181d-125">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7181d-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="7181d-126">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="7181d-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="7181d-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7181d-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7181d-128">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7181d-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7181d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7181d-129">Properties</span></span>
|<span data-ttu-id="7181d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7181d-130">Property</span></span>|<span data-ttu-id="7181d-131">種類</span><span class="sxs-lookup"><span data-stu-id="7181d-131">Type</span></span>|<span data-ttu-id="7181d-132">説明</span><span class="sxs-lookup"><span data-stu-id="7181d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7181d-133">ID</span><span class="sxs-lookup"><span data-stu-id="7181d-133">id</span></span>|<span data-ttu-id="7181d-134">String</span><span class="sxs-lookup"><span data-stu-id="7181d-134">String</span></span>|<span data-ttu-id="7181d-135">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7181d-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="7181d-136">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="7181d-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="7181d-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7181d-137">Read-only.</span></span>|
|<span data-ttu-id="7181d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7181d-138">displayName</span></span>|<span data-ttu-id="7181d-139">String</span><span class="sxs-lookup"><span data-stu-id="7181d-139">String</span></span>|<span data-ttu-id="7181d-140">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="7181d-140">Name of the discovered application.</span></span> <span data-ttu-id="7181d-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="7181d-141">Read-only</span></span>|
|<span data-ttu-id="7181d-142">version</span><span class="sxs-lookup"><span data-stu-id="7181d-142">version</span></span>|<span data-ttu-id="7181d-143">String</span><span class="sxs-lookup"><span data-stu-id="7181d-143">String</span></span>|<span data-ttu-id="7181d-144">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7181d-144">Version of the discovered application.</span></span> <span data-ttu-id="7181d-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="7181d-145">Read-only</span></span>|
|<span data-ttu-id="7181d-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="7181d-146">sizeInByte</span></span>|<span data-ttu-id="7181d-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7181d-147">Int64</span></span>|<span data-ttu-id="7181d-148">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="7181d-148">Discovered application size in bytes.</span></span> <span data-ttu-id="7181d-149">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="7181d-149">Read-only</span></span>|
|<span data-ttu-id="7181d-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7181d-150">deviceCount</span></span>|<span data-ttu-id="7181d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7181d-151">Int32</span></span>|<span data-ttu-id="7181d-152">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7181d-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7181d-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7181d-153">Relationships</span></span>
|<span data-ttu-id="7181d-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7181d-154">Relationship</span></span>|<span data-ttu-id="7181d-155">型</span><span class="sxs-lookup"><span data-stu-id="7181d-155">Type</span></span>|<span data-ttu-id="7181d-156">説明</span><span class="sxs-lookup"><span data-stu-id="7181d-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7181d-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="7181d-157">managedDevices</span></span>|<span data-ttu-id="7181d-158">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7181d-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="7181d-159">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="7181d-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7181d-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7181d-160">JSON Representation</span></span>
<span data-ttu-id="7181d-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7181d-161">Here is a JSON representation of the resource.</span></span>
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




