---
title: settingStateDeviceSummary リソースの種類
description: 設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 207620758c35951f5de5b504889214f5270ef537
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969717"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="59638-103">settingStateDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59638-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="59638-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59638-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59638-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59638-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59638-106">設定状態の要約に対する、デバイス コンプライアンス ポリシーおよび構成</span><span class="sxs-lookup"><span data-stu-id="59638-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="59638-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="59638-107">Methods</span></span>
|<span data-ttu-id="59638-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="59638-108">Method</span></span>|<span data-ttu-id="59638-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59638-109">Return Type</span></span>|<span data-ttu-id="59638-110">説明</span><span class="sxs-lookup"><span data-stu-id="59638-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59638-111">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="59638-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="59638-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59638-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="59638-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="59638-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="59638-114">settingStateDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="59638-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="59638-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59638-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59638-116">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="59638-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="59638-117">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="59638-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="59638-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59638-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59638-119">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="59638-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="59638-120">settingStateDeviceSummary の削除</span><span class="sxs-lookup"><span data-stu-id="59638-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="59638-121">なし</span><span class="sxs-lookup"><span data-stu-id="59638-121">None</span></span>|<span data-ttu-id="59638-122">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="59638-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="59638-123">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="59638-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="59638-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59638-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59638-125">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="59638-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59638-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59638-126">Properties</span></span>
|<span data-ttu-id="59638-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59638-127">Property</span></span>|<span data-ttu-id="59638-128">型</span><span class="sxs-lookup"><span data-stu-id="59638-128">Type</span></span>|<span data-ttu-id="59638-129">説明</span><span class="sxs-lookup"><span data-stu-id="59638-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59638-130">id</span><span class="sxs-lookup"><span data-stu-id="59638-130">id</span></span>|<span data-ttu-id="59638-131">String</span><span class="sxs-lookup"><span data-stu-id="59638-131">String</span></span>|<span data-ttu-id="59638-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="59638-132">Key of the entity.</span></span>|
|<span data-ttu-id="59638-133">settingName</span><span class="sxs-lookup"><span data-stu-id="59638-133">settingName</span></span>|<span data-ttu-id="59638-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="59638-134">String</span></span>|<span data-ttu-id="59638-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="59638-135">Name of the setting</span></span>|
|<span data-ttu-id="59638-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="59638-136">instancePath</span></span>|<span data-ttu-id="59638-137">String</span><span class="sxs-lookup"><span data-stu-id="59638-137">String</span></span>|<span data-ttu-id="59638-138">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="59638-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="59638-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-139">unknownDeviceCount</span></span>|<span data-ttu-id="59638-140">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-140">Int32</span></span>|<span data-ttu-id="59638-141">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="59638-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="59638-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="59638-143">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-143">Int32</span></span>|<span data-ttu-id="59638-144">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="59638-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="59638-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-145">compliantDeviceCount</span></span>|<span data-ttu-id="59638-146">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-146">Int32</span></span>|<span data-ttu-id="59638-147">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="59638-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="59638-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-148">remediatedDeviceCount</span></span>|<span data-ttu-id="59638-149">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-149">Int32</span></span>|<span data-ttu-id="59638-150">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="59638-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="59638-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="59638-152">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-152">Int32</span></span>|<span data-ttu-id="59638-153">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="59638-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="59638-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-154">errorDeviceCount</span></span>|<span data-ttu-id="59638-155">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-155">Int32</span></span>|<span data-ttu-id="59638-156">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="59638-156">Device error count for the setting</span></span>|
|<span data-ttu-id="59638-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59638-157">conflictDeviceCount</span></span>|<span data-ttu-id="59638-158">Int32</span><span class="sxs-lookup"><span data-stu-id="59638-158">Int32</span></span>|<span data-ttu-id="59638-159">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="59638-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="59638-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59638-160">Relationships</span></span>
<span data-ttu-id="59638-161">なし</span><span class="sxs-lookup"><span data-stu-id="59638-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59638-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59638-162">JSON Representation</span></span>
<span data-ttu-id="59638-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59638-163">Here is a JSON representation of the resource.</span></span>
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





