---
title: detectedApp リソースの種類
description: 管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01e942790136deb967d1efc22928ed9144b5012b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951398"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="8804f-104">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8804f-104">detectedApp resource type</span></span>

> <span data-ttu-id="8804f-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8804f-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8804f-106">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="8804f-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="8804f-107">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="8804f-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="8804f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8804f-108">Methods</span></span>
|<span data-ttu-id="8804f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8804f-109">Method</span></span>|<span data-ttu-id="8804f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8804f-110">Return Type</span></span>|<span data-ttu-id="8804f-111">説明</span><span class="sxs-lookup"><span data-stu-id="8804f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8804f-112">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="8804f-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="8804f-113">[detectedApp](../resources/intune-devices-detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8804f-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="8804f-114">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8804f-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="8804f-115">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="8804f-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="8804f-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8804f-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8804f-117">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8804f-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8804f-118">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="8804f-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="8804f-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8804f-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8804f-120">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8804f-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8804f-121">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="8804f-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="8804f-122">なし</span><span class="sxs-lookup"><span data-stu-id="8804f-122">None</span></span>|<span data-ttu-id="8804f-123">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8804f-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="8804f-124">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="8804f-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="8804f-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8804f-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8804f-126">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8804f-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8804f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8804f-127">Properties</span></span>
|<span data-ttu-id="8804f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8804f-128">Property</span></span>|<span data-ttu-id="8804f-129">種類</span><span class="sxs-lookup"><span data-stu-id="8804f-129">Type</span></span>|<span data-ttu-id="8804f-130">説明</span><span class="sxs-lookup"><span data-stu-id="8804f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8804f-131">ID</span><span class="sxs-lookup"><span data-stu-id="8804f-131">id</span></span>|<span data-ttu-id="8804f-132">String</span><span class="sxs-lookup"><span data-stu-id="8804f-132">String</span></span>|<span data-ttu-id="8804f-133">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8804f-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="8804f-134">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="8804f-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="8804f-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8804f-135">Read-only.</span></span>|
|<span data-ttu-id="8804f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8804f-136">displayName</span></span>|<span data-ttu-id="8804f-137">String</span><span class="sxs-lookup"><span data-stu-id="8804f-137">String</span></span>|<span data-ttu-id="8804f-138">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="8804f-138">Name of the discovered application.</span></span> <span data-ttu-id="8804f-139">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="8804f-139">Read-only</span></span>|
|<span data-ttu-id="8804f-140">version</span><span class="sxs-lookup"><span data-stu-id="8804f-140">version</span></span>|<span data-ttu-id="8804f-141">String</span><span class="sxs-lookup"><span data-stu-id="8804f-141">String</span></span>|<span data-ttu-id="8804f-142">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8804f-142">Version of the discovered application.</span></span> <span data-ttu-id="8804f-143">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="8804f-143">Read-only</span></span>|
|<span data-ttu-id="8804f-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="8804f-144">sizeInByte</span></span>|<span data-ttu-id="8804f-145">Int64</span><span class="sxs-lookup"><span data-stu-id="8804f-145">Int64</span></span>|<span data-ttu-id="8804f-146">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="8804f-146">Discovered application size in bytes.</span></span> <span data-ttu-id="8804f-147">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="8804f-147">Read-only</span></span>|
|<span data-ttu-id="8804f-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8804f-148">deviceCount</span></span>|<span data-ttu-id="8804f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8804f-149">Int32</span></span>|<span data-ttu-id="8804f-150">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8804f-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="8804f-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8804f-151">Relationships</span></span>
|<span data-ttu-id="8804f-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8804f-152">Relationship</span></span>|<span data-ttu-id="8804f-153">型</span><span class="sxs-lookup"><span data-stu-id="8804f-153">Type</span></span>|<span data-ttu-id="8804f-154">説明</span><span class="sxs-lookup"><span data-stu-id="8804f-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8804f-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="8804f-155">managedDevices</span></span>|<span data-ttu-id="8804f-156">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8804f-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="8804f-157">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="8804f-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8804f-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8804f-158">JSON Representation</span></span>
<span data-ttu-id="8804f-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8804f-159">Here is a JSON representation of the resource.</span></span>
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



