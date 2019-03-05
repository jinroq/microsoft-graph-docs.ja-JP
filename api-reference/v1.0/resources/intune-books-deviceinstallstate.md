---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e737a58fc9547d54feeeeef47136286285c1e99
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255060"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="5d9bf-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d9bf-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="5d9bf-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d9bf-105">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-105">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="5d9bf-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5d9bf-106">Methods</span></span>
|<span data-ttu-id="5d9bf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5d9bf-107">Method</span></span>|<span data-ttu-id="5d9bf-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5d9bf-108">Return Type</span></span>|<span data-ttu-id="5d9bf-109">説明</span><span class="sxs-lookup"><span data-stu-id="5d9bf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5d9bf-110">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="5d9bf-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="5d9bf-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5d9bf-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5d9bf-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="5d9bf-113">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="5d9bf-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="5d9bf-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="5d9bf-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="5d9bf-115">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="5d9bf-116">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="5d9bf-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="5d9bf-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="5d9bf-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="5d9bf-118">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="5d9bf-119">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="5d9bf-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="5d9bf-120">なし</span><span class="sxs-lookup"><span data-stu-id="5d9bf-120">None</span></span>|<span data-ttu-id="5d9bf-121">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="5d9bf-122">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="5d9bf-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="5d9bf-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="5d9bf-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="5d9bf-124">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5d9bf-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d9bf-125">Properties</span></span>
|<span data-ttu-id="5d9bf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d9bf-126">Property</span></span>|<span data-ttu-id="5d9bf-127">型</span><span class="sxs-lookup"><span data-stu-id="5d9bf-127">Type</span></span>|<span data-ttu-id="5d9bf-128">説明</span><span class="sxs-lookup"><span data-stu-id="5d9bf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d9bf-129">id</span><span class="sxs-lookup"><span data-stu-id="5d9bf-129">id</span></span>|<span data-ttu-id="5d9bf-130">文字列</span><span class="sxs-lookup"><span data-stu-id="5d9bf-130">String</span></span>|<span data-ttu-id="5d9bf-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-131">Key of the entity.</span></span>|
|<span data-ttu-id="5d9bf-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="5d9bf-132">deviceName</span></span>|<span data-ttu-id="5d9bf-133">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-133">String</span></span>|<span data-ttu-id="5d9bf-134">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-134">Device name.</span></span>|
|<span data-ttu-id="5d9bf-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="5d9bf-135">deviceId</span></span>|<span data-ttu-id="5d9bf-136">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-136">String</span></span>|<span data-ttu-id="5d9bf-137">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-137">Device Id.</span></span>|
|<span data-ttu-id="5d9bf-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5d9bf-138">lastSyncDateTime</span></span>|<span data-ttu-id="5d9bf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d9bf-139">DateTimeOffset</span></span>|<span data-ttu-id="5d9bf-140">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-140">Last sync date and time.</span></span>|
|<span data-ttu-id="5d9bf-141">installState</span><span class="sxs-lookup"><span data-stu-id="5d9bf-141">installState</span></span>|[<span data-ttu-id="5d9bf-142">installState</span><span class="sxs-lookup"><span data-stu-id="5d9bf-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="5d9bf-143">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-143">The install state of the eBook.</span></span> <span data-ttu-id="5d9bf-144">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="5d9bf-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="5d9bf-145">errorCode</span></span>|<span data-ttu-id="5d9bf-146">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-146">String</span></span>|<span data-ttu-id="5d9bf-147">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-147">The error code for install failures.</span></span>|
|<span data-ttu-id="5d9bf-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="5d9bf-148">osVersion</span></span>|<span data-ttu-id="5d9bf-149">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-149">String</span></span>|<span data-ttu-id="5d9bf-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-150">OS Version.</span></span>|
|<span data-ttu-id="5d9bf-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="5d9bf-151">osDescription</span></span>|<span data-ttu-id="5d9bf-152">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-152">String</span></span>|<span data-ttu-id="5d9bf-153">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-153">OS Description.</span></span>|
|<span data-ttu-id="5d9bf-154">userName</span><span class="sxs-lookup"><span data-stu-id="5d9bf-154">userName</span></span>|<span data-ttu-id="5d9bf-155">String</span><span class="sxs-lookup"><span data-stu-id="5d9bf-155">String</span></span>|<span data-ttu-id="5d9bf-156">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d9bf-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d9bf-157">Relationships</span></span>
<span data-ttu-id="5d9bf-158">なし</span><span class="sxs-lookup"><span data-stu-id="5d9bf-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d9bf-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d9bf-159">JSON Representation</span></span>
<span data-ttu-id="5d9bf-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5d9bf-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



