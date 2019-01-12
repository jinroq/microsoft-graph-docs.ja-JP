---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2104998cfdd65659114b1850d3cfcf1392bf9642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925876"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="a4c8d-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4c8d-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="a4c8d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4c8d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4c8d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4c8d-107">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="a4c8d-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="a4c8d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4c8d-108">Methods</span></span>
|<span data-ttu-id="a4c8d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4c8d-109">Method</span></span>|<span data-ttu-id="a4c8d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4c8d-110">Return Type</span></span>|<span data-ttu-id="a4c8d-111">説明</span><span class="sxs-lookup"><span data-stu-id="a4c8d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a4c8d-112">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="a4c8d-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="a4c8d-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4c8d-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a4c8d-114">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="a4c8d-115">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="a4c8d-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="a4c8d-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a4c8d-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="a4c8d-117">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="a4c8d-118">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="a4c8d-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="a4c8d-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a4c8d-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="a4c8d-120">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="a4c8d-121">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="a4c8d-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="a4c8d-122">なし</span><span class="sxs-lookup"><span data-stu-id="a4c8d-122">None</span></span>|<span data-ttu-id="a4c8d-123">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="a4c8d-124">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a4c8d-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="a4c8d-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a4c8d-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="a4c8d-126">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4c8d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4c8d-127">Properties</span></span>
|<span data-ttu-id="a4c8d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4c8d-128">Property</span></span>|<span data-ttu-id="a4c8d-129">型</span><span class="sxs-lookup"><span data-stu-id="a4c8d-129">Type</span></span>|<span data-ttu-id="a4c8d-130">説明</span><span class="sxs-lookup"><span data-stu-id="a4c8d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c8d-131">ID</span><span class="sxs-lookup"><span data-stu-id="a4c8d-131">id</span></span>|<span data-ttu-id="a4c8d-132">String</span><span class="sxs-lookup"><span data-stu-id="a4c8d-132">String</span></span>|<span data-ttu-id="a4c8d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-133">Key of the entity.</span></span>|
|<span data-ttu-id="a4c8d-134">settingName</span><span class="sxs-lookup"><span data-stu-id="a4c8d-134">settingName</span></span>|<span data-ttu-id="a4c8d-135">String</span><span class="sxs-lookup"><span data-stu-id="a4c8d-135">String</span></span>|<span data-ttu-id="a4c8d-136">設定の名前</span><span class="sxs-lookup"><span data-stu-id="a4c8d-136">Name of the setting</span></span>|
|<span data-ttu-id="a4c8d-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="a4c8d-137">instancePath</span></span>|<span data-ttu-id="a4c8d-138">String</span><span class="sxs-lookup"><span data-stu-id="a4c8d-138">String</span></span>|<span data-ttu-id="a4c8d-139">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="a4c8d-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="a4c8d-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-140">unknownDeviceCount</span></span>|<span data-ttu-id="a4c8d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-141">Int32</span></span>|<span data-ttu-id="a4c8d-142">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="a4c8d-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="a4c8d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-144">Int32</span></span>|<span data-ttu-id="a4c8d-145">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="a4c8d-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-146">compliantDeviceCount</span></span>|<span data-ttu-id="a4c8d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-147">Int32</span></span>|<span data-ttu-id="a4c8d-148">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a4c8d-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-149">remediatedDeviceCount</span></span>|<span data-ttu-id="a4c8d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-150">Int32</span></span>|<span data-ttu-id="a4c8d-151">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a4c8d-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a4c8d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-153">Int32</span></span>|<span data-ttu-id="a4c8d-154">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="a4c8d-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-155">errorDeviceCount</span></span>|<span data-ttu-id="a4c8d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-156">Int32</span></span>|<span data-ttu-id="a4c8d-157">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-157">Device error count for the setting</span></span>|
|<span data-ttu-id="a4c8d-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c8d-158">conflictDeviceCount</span></span>|<span data-ttu-id="a4c8d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c8d-159">Int32</span></span>|<span data-ttu-id="a4c8d-160">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="a4c8d-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4c8d-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4c8d-161">Relationships</span></span>
<span data-ttu-id="a4c8d-162">なし</span><span class="sxs-lookup"><span data-stu-id="a4c8d-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4c8d-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4c8d-163">JSON Representation</span></span>
<span data-ttu-id="a4c8d-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4c8d-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





