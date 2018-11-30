---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
ms.openlocfilehash: 944cb57d397ffe7b75f0a378680b0f1468b10f49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073022"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="9ee40-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ee40-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="9ee40-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ee40-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ee40-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ee40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ee40-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ee40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ee40-107">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ee40-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="9ee40-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ee40-108">Methods</span></span>
|<span data-ttu-id="9ee40-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ee40-109">Method</span></span>|<span data-ttu-id="9ee40-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9ee40-110">Return Type</span></span>|<span data-ttu-id="9ee40-111">説明</span><span class="sxs-lookup"><span data-stu-id="9ee40-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ee40-112">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="9ee40-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="9ee40-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ee40-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9ee40-114">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9ee40-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="9ee40-115">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="9ee40-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="9ee40-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9ee40-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9ee40-117">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9ee40-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9ee40-118">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="9ee40-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="9ee40-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9ee40-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9ee40-120">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ee40-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9ee40-121">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="9ee40-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="9ee40-122">なし</span><span class="sxs-lookup"><span data-stu-id="9ee40-122">None</span></span>|<span data-ttu-id="9ee40-123">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="9ee40-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="9ee40-124">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="9ee40-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="9ee40-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9ee40-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9ee40-126">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ee40-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ee40-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ee40-127">Properties</span></span>
|<span data-ttu-id="9ee40-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ee40-128">Property</span></span>|<span data-ttu-id="9ee40-129">型</span><span class="sxs-lookup"><span data-stu-id="9ee40-129">Type</span></span>|<span data-ttu-id="9ee40-130">説明</span><span class="sxs-lookup"><span data-stu-id="9ee40-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee40-131">id</span><span class="sxs-lookup"><span data-stu-id="9ee40-131">id</span></span>|<span data-ttu-id="9ee40-132">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-132">String</span></span>|<span data-ttu-id="9ee40-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ee40-133">Key of the entity.</span></span>|
|<span data-ttu-id="9ee40-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9ee40-134">deviceName</span></span>|<span data-ttu-id="9ee40-135">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-135">String</span></span>|<span data-ttu-id="9ee40-136">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="9ee40-136">Device name.</span></span>|
|<span data-ttu-id="9ee40-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9ee40-137">deviceId</span></span>|<span data-ttu-id="9ee40-138">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-138">String</span></span>|<span data-ttu-id="9ee40-139">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="9ee40-139">Device Id.</span></span>|
|<span data-ttu-id="9ee40-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee40-140">lastSyncDateTime</span></span>|<span data-ttu-id="9ee40-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee40-141">DateTimeOffset</span></span>|<span data-ttu-id="9ee40-142">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="9ee40-142">Last sync date and time.</span></span>|
|<span data-ttu-id="9ee40-143">installState</span><span class="sxs-lookup"><span data-stu-id="9ee40-143">installState</span></span>|[<span data-ttu-id="9ee40-144">installState</span><span class="sxs-lookup"><span data-stu-id="9ee40-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9ee40-145">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="9ee40-145">The install state of the eBook.</span></span> <span data-ttu-id="9ee40-146">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="9ee40-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9ee40-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="9ee40-147">errorCode</span></span>|<span data-ttu-id="9ee40-148">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-148">String</span></span>|<span data-ttu-id="9ee40-149">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="9ee40-149">The error code for install failures.</span></span>|
|<span data-ttu-id="9ee40-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="9ee40-150">osVersion</span></span>|<span data-ttu-id="9ee40-151">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-151">String</span></span>|<span data-ttu-id="9ee40-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="9ee40-152">OS Version.</span></span>|
|<span data-ttu-id="9ee40-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="9ee40-153">osDescription</span></span>|<span data-ttu-id="9ee40-154">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-154">String</span></span>|<span data-ttu-id="9ee40-155">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="9ee40-155">OS Description.</span></span>|
|<span data-ttu-id="9ee40-156">userName</span><span class="sxs-lookup"><span data-stu-id="9ee40-156">userName</span></span>|<span data-ttu-id="9ee40-157">String</span><span class="sxs-lookup"><span data-stu-id="9ee40-157">String</span></span>|<span data-ttu-id="9ee40-158">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="9ee40-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee40-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ee40-159">Relationships</span></span>
<span data-ttu-id="9ee40-160">なし</span><span class="sxs-lookup"><span data-stu-id="9ee40-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ee40-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ee40-161">JSON Representation</span></span>
<span data-ttu-id="9ee40-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ee40-162">Here is a JSON representation of the resource.</span></span>
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





