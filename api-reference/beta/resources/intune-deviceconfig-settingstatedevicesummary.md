---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: tfitzmac
ms.openlocfilehash: dff6f8966d321aa706fceabceb14a418ae8433f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318537"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="7fe0b-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7fe0b-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="7fe0b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fe0b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fe0b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fe0b-107">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="7fe0b-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="7fe0b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7fe0b-108">Methods</span></span>
|<span data-ttu-id="7fe0b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7fe0b-109">Method</span></span>|<span data-ttu-id="7fe0b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7fe0b-110">Return Type</span></span>|<span data-ttu-id="7fe0b-111">説明</span><span class="sxs-lookup"><span data-stu-id="7fe0b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7fe0b-112">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="7fe0b-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="7fe0b-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7fe0b-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7fe0b-114">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="7fe0b-115">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="7fe0b-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="7fe0b-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7fe0b-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="7fe0b-117">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="7fe0b-118">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="7fe0b-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="7fe0b-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7fe0b-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="7fe0b-120">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="7fe0b-121">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="7fe0b-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="7fe0b-122">なし</span><span class="sxs-lookup"><span data-stu-id="7fe0b-122">None</span></span>|<span data-ttu-id="7fe0b-123">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="7fe0b-124">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="7fe0b-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="7fe0b-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7fe0b-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="7fe0b-126">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7fe0b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fe0b-127">Properties</span></span>
|<span data-ttu-id="7fe0b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fe0b-128">Property</span></span>|<span data-ttu-id="7fe0b-129">種類</span><span class="sxs-lookup"><span data-stu-id="7fe0b-129">Type</span></span>|<span data-ttu-id="7fe0b-130">説明</span><span class="sxs-lookup"><span data-stu-id="7fe0b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe0b-131">ID</span><span class="sxs-lookup"><span data-stu-id="7fe0b-131">id</span></span>|<span data-ttu-id="7fe0b-132">String</span><span class="sxs-lookup"><span data-stu-id="7fe0b-132">String</span></span>|<span data-ttu-id="7fe0b-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-133">Key of the entity.</span></span>|
|<span data-ttu-id="7fe0b-134">settingName</span><span class="sxs-lookup"><span data-stu-id="7fe0b-134">settingName</span></span>|<span data-ttu-id="7fe0b-135">String</span><span class="sxs-lookup"><span data-stu-id="7fe0b-135">String</span></span>|<span data-ttu-id="7fe0b-136">設定の名前</span><span class="sxs-lookup"><span data-stu-id="7fe0b-136">Name of the setting</span></span>|
|<span data-ttu-id="7fe0b-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="7fe0b-137">instancePath</span></span>|<span data-ttu-id="7fe0b-138">String</span><span class="sxs-lookup"><span data-stu-id="7fe0b-138">String</span></span>|<span data-ttu-id="7fe0b-139">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="7fe0b-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="7fe0b-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-140">unknownDeviceCount</span></span>|<span data-ttu-id="7fe0b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-141">Int32</span></span>|<span data-ttu-id="7fe0b-142">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="7fe0b-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="7fe0b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-144">Int32</span></span>|<span data-ttu-id="7fe0b-145">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="7fe0b-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-146">compliantDeviceCount</span></span>|<span data-ttu-id="7fe0b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-147">Int32</span></span>|<span data-ttu-id="7fe0b-148">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7fe0b-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-149">remediatedDeviceCount</span></span>|<span data-ttu-id="7fe0b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-150">Int32</span></span>|<span data-ttu-id="7fe0b-151">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7fe0b-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7fe0b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-153">Int32</span></span>|<span data-ttu-id="7fe0b-154">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="7fe0b-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-155">errorDeviceCount</span></span>|<span data-ttu-id="7fe0b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-156">Int32</span></span>|<span data-ttu-id="7fe0b-157">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-157">Device error count for the setting</span></span>|
|<span data-ttu-id="7fe0b-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fe0b-158">conflictDeviceCount</span></span>|<span data-ttu-id="7fe0b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe0b-159">Int32</span></span>|<span data-ttu-id="7fe0b-160">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="7fe0b-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fe0b-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7fe0b-161">Relationships</span></span>
<span data-ttu-id="7fe0b-162">なし</span><span class="sxs-lookup"><span data-stu-id="7fe0b-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fe0b-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7fe0b-163">JSON Representation</span></span>
<span data-ttu-id="7fe0b-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7fe0b-164">Here is a JSON representation of the resource.</span></span>
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





