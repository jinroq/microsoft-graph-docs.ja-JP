---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: acd4717901a63963e1e02c3a031bdd1630e84cd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834427"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="1bc7e-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bc7e-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="1bc7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bc7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bc7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bc7e-107">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="1bc7e-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="1bc7e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1bc7e-108">Methods</span></span>
|<span data-ttu-id="1bc7e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1bc7e-109">Method</span></span>|<span data-ttu-id="1bc7e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1bc7e-110">Return Type</span></span>|<span data-ttu-id="1bc7e-111">説明</span><span class="sxs-lookup"><span data-stu-id="1bc7e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1bc7e-112">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="1bc7e-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="1bc7e-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1bc7e-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1bc7e-114">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="1bc7e-115">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="1bc7e-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="1bc7e-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1bc7e-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1bc7e-117">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="1bc7e-118">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="1bc7e-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="1bc7e-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1bc7e-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1bc7e-120">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="1bc7e-121">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="1bc7e-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="1bc7e-122">なし</span><span class="sxs-lookup"><span data-stu-id="1bc7e-122">None</span></span>|<span data-ttu-id="1bc7e-123">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="1bc7e-124">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="1bc7e-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="1bc7e-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1bc7e-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1bc7e-126">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1bc7e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bc7e-127">Properties</span></span>
|<span data-ttu-id="1bc7e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bc7e-128">Property</span></span>|<span data-ttu-id="1bc7e-129">種類</span><span class="sxs-lookup"><span data-stu-id="1bc7e-129">Type</span></span>|<span data-ttu-id="1bc7e-130">説明</span><span class="sxs-lookup"><span data-stu-id="1bc7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc7e-131">ID</span><span class="sxs-lookup"><span data-stu-id="1bc7e-131">id</span></span>|<span data-ttu-id="1bc7e-132">String</span><span class="sxs-lookup"><span data-stu-id="1bc7e-132">String</span></span>|<span data-ttu-id="1bc7e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-133">Key of the entity.</span></span>|
|<span data-ttu-id="1bc7e-134">settingName</span><span class="sxs-lookup"><span data-stu-id="1bc7e-134">settingName</span></span>|<span data-ttu-id="1bc7e-135">String</span><span class="sxs-lookup"><span data-stu-id="1bc7e-135">String</span></span>|<span data-ttu-id="1bc7e-136">設定の名前</span><span class="sxs-lookup"><span data-stu-id="1bc7e-136">Name of the setting</span></span>|
|<span data-ttu-id="1bc7e-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="1bc7e-137">instancePath</span></span>|<span data-ttu-id="1bc7e-138">String</span><span class="sxs-lookup"><span data-stu-id="1bc7e-138">String</span></span>|<span data-ttu-id="1bc7e-139">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="1bc7e-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="1bc7e-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-140">unknownDeviceCount</span></span>|<span data-ttu-id="1bc7e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-141">Int32</span></span>|<span data-ttu-id="1bc7e-142">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="1bc7e-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="1bc7e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-144">Int32</span></span>|<span data-ttu-id="1bc7e-145">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="1bc7e-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-146">compliantDeviceCount</span></span>|<span data-ttu-id="1bc7e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-147">Int32</span></span>|<span data-ttu-id="1bc7e-148">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="1bc7e-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-149">remediatedDeviceCount</span></span>|<span data-ttu-id="1bc7e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-150">Int32</span></span>|<span data-ttu-id="1bc7e-151">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="1bc7e-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1bc7e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-153">Int32</span></span>|<span data-ttu-id="1bc7e-154">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="1bc7e-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-155">errorDeviceCount</span></span>|<span data-ttu-id="1bc7e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-156">Int32</span></span>|<span data-ttu-id="1bc7e-157">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-157">Device error count for the setting</span></span>|
|<span data-ttu-id="1bc7e-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1bc7e-158">conflictDeviceCount</span></span>|<span data-ttu-id="1bc7e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1bc7e-159">Int32</span></span>|<span data-ttu-id="1bc7e-160">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="1bc7e-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bc7e-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1bc7e-161">Relationships</span></span>
<span data-ttu-id="1bc7e-162">なし</span><span class="sxs-lookup"><span data-stu-id="1bc7e-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1bc7e-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1bc7e-163">JSON Representation</span></span>
<span data-ttu-id="1bc7e-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1bc7e-164">Here is a JSON representation of the resource.</span></span>
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





