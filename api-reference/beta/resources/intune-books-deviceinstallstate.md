---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c90b3e8e0693a28781a45f77cd00661528648439
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410722"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="fada4-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fada4-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="fada4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fada4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fada4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fada4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fada4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fada4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fada4-107">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fada4-107">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="fada4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fada4-108">Methods</span></span>
|<span data-ttu-id="fada4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fada4-109">Method</span></span>|<span data-ttu-id="fada4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fada4-110">Return Type</span></span>|<span data-ttu-id="fada4-111">説明</span><span class="sxs-lookup"><span data-stu-id="fada4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fada4-112">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="fada4-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="fada4-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fada4-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="fada4-114">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fada4-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="fada4-115">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="fada4-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="fada4-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="fada4-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="fada4-117">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fada4-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="fada4-118">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="fada4-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="fada4-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="fada4-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="fada4-120">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fada4-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="fada4-121">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="fada4-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="fada4-122">なし</span><span class="sxs-lookup"><span data-stu-id="fada4-122">None</span></span>|<span data-ttu-id="fada4-123">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fada4-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="fada4-124">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="fada4-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="fada4-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="fada4-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="fada4-126">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fada4-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fada4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fada4-127">Properties</span></span>
|<span data-ttu-id="fada4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fada4-128">Property</span></span>|<span data-ttu-id="fada4-129">型</span><span class="sxs-lookup"><span data-stu-id="fada4-129">Type</span></span>|<span data-ttu-id="fada4-130">説明</span><span class="sxs-lookup"><span data-stu-id="fada4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fada4-131">id</span><span class="sxs-lookup"><span data-stu-id="fada4-131">id</span></span>|<span data-ttu-id="fada4-132">String</span><span class="sxs-lookup"><span data-stu-id="fada4-132">String</span></span>|<span data-ttu-id="fada4-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fada4-133">Key of the entity.</span></span>|
|<span data-ttu-id="fada4-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="fada4-134">deviceName</span></span>|<span data-ttu-id="fada4-135">String</span><span class="sxs-lookup"><span data-stu-id="fada4-135">String</span></span>|<span data-ttu-id="fada4-136">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="fada4-136">Device name.</span></span>|
|<span data-ttu-id="fada4-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="fada4-137">deviceId</span></span>|<span data-ttu-id="fada4-138">String</span><span class="sxs-lookup"><span data-stu-id="fada4-138">String</span></span>|<span data-ttu-id="fada4-139">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="fada4-139">Device Id.</span></span>|
|<span data-ttu-id="fada4-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fada4-140">lastSyncDateTime</span></span>|<span data-ttu-id="fada4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fada4-141">DateTimeOffset</span></span>|<span data-ttu-id="fada4-142">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="fada4-142">Last sync date and time.</span></span>|
|<span data-ttu-id="fada4-143">installState</span><span class="sxs-lookup"><span data-stu-id="fada4-143">installState</span></span>|[<span data-ttu-id="fada4-144">installState</span><span class="sxs-lookup"><span data-stu-id="fada4-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="fada4-145">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="fada4-145">The install state of the eBook.</span></span> <span data-ttu-id="fada4-146">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="fada4-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="fada4-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="fada4-147">errorCode</span></span>|<span data-ttu-id="fada4-148">String</span><span class="sxs-lookup"><span data-stu-id="fada4-148">String</span></span>|<span data-ttu-id="fada4-149">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="fada4-149">The error code for install failures.</span></span>|
|<span data-ttu-id="fada4-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="fada4-150">osVersion</span></span>|<span data-ttu-id="fada4-151">String</span><span class="sxs-lookup"><span data-stu-id="fada4-151">String</span></span>|<span data-ttu-id="fada4-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="fada4-152">OS Version.</span></span>|
|<span data-ttu-id="fada4-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="fada4-153">osDescription</span></span>|<span data-ttu-id="fada4-154">String</span><span class="sxs-lookup"><span data-stu-id="fada4-154">String</span></span>|<span data-ttu-id="fada4-155">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="fada4-155">OS Description.</span></span>|
|<span data-ttu-id="fada4-156">userName</span><span class="sxs-lookup"><span data-stu-id="fada4-156">userName</span></span>|<span data-ttu-id="fada4-157">String</span><span class="sxs-lookup"><span data-stu-id="fada4-157">String</span></span>|<span data-ttu-id="fada4-158">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="fada4-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fada4-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fada4-159">Relationships</span></span>
<span data-ttu-id="fada4-160">なし</span><span class="sxs-lookup"><span data-stu-id="fada4-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fada4-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fada4-161">JSON Representation</span></span>
<span data-ttu-id="fada4-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fada4-162">Here is a JSON representation of the resource.</span></span>
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




