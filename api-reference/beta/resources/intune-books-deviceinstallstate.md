---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: fb11f93682093655a38ac554b2816348f9b0c6bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360369"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="6539d-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6539d-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="6539d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6539d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6539d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6539d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6539d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6539d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6539d-107">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6539d-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="6539d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6539d-108">Methods</span></span>
|<span data-ttu-id="6539d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6539d-109">Method</span></span>|<span data-ttu-id="6539d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6539d-110">Return Type</span></span>|<span data-ttu-id="6539d-111">説明</span><span class="sxs-lookup"><span data-stu-id="6539d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6539d-112">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="6539d-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="6539d-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6539d-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6539d-114">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6539d-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="6539d-115">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="6539d-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="6539d-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6539d-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6539d-117">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6539d-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="6539d-118">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="6539d-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="6539d-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6539d-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6539d-120">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6539d-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="6539d-121">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="6539d-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="6539d-122">なし</span><span class="sxs-lookup"><span data-stu-id="6539d-122">None</span></span>|<span data-ttu-id="6539d-123">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6539d-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="6539d-124">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="6539d-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="6539d-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6539d-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6539d-126">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6539d-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6539d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6539d-127">Properties</span></span>
|<span data-ttu-id="6539d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6539d-128">Property</span></span>|<span data-ttu-id="6539d-129">種類</span><span class="sxs-lookup"><span data-stu-id="6539d-129">Type</span></span>|<span data-ttu-id="6539d-130">説明</span><span class="sxs-lookup"><span data-stu-id="6539d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6539d-131">ID</span><span class="sxs-lookup"><span data-stu-id="6539d-131">id</span></span>|<span data-ttu-id="6539d-132">String</span><span class="sxs-lookup"><span data-stu-id="6539d-132">String</span></span>|<span data-ttu-id="6539d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6539d-133">Key of the entity.</span></span>|
|<span data-ttu-id="6539d-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="6539d-134">deviceName</span></span>|<span data-ttu-id="6539d-135">String</span><span class="sxs-lookup"><span data-stu-id="6539d-135">String</span></span>|<span data-ttu-id="6539d-136">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="6539d-136">Device name.</span></span>|
|<span data-ttu-id="6539d-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="6539d-137">deviceId</span></span>|<span data-ttu-id="6539d-138">String</span><span class="sxs-lookup"><span data-stu-id="6539d-138">String</span></span>|<span data-ttu-id="6539d-139">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="6539d-139">Device Id.</span></span>|
|<span data-ttu-id="6539d-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6539d-140">lastSyncDateTime</span></span>|<span data-ttu-id="6539d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6539d-141">DateTimeOffset</span></span>|<span data-ttu-id="6539d-142">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="6539d-142">Last sync date and time.</span></span>|
|<span data-ttu-id="6539d-143">installState</span><span class="sxs-lookup"><span data-stu-id="6539d-143">installState</span></span>|[<span data-ttu-id="6539d-144">installState</span><span class="sxs-lookup"><span data-stu-id="6539d-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="6539d-145">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="6539d-145">The install state of the eBook.</span></span> <span data-ttu-id="6539d-146">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="6539d-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="6539d-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="6539d-147">errorCode</span></span>|<span data-ttu-id="6539d-148">String</span><span class="sxs-lookup"><span data-stu-id="6539d-148">String</span></span>|<span data-ttu-id="6539d-149">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="6539d-149">The error code for install failures.</span></span>|
|<span data-ttu-id="6539d-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="6539d-150">osVersion</span></span>|<span data-ttu-id="6539d-151">String</span><span class="sxs-lookup"><span data-stu-id="6539d-151">String</span></span>|<span data-ttu-id="6539d-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="6539d-152">OS Version.</span></span>|
|<span data-ttu-id="6539d-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="6539d-153">osDescription</span></span>|<span data-ttu-id="6539d-154">String</span><span class="sxs-lookup"><span data-stu-id="6539d-154">String</span></span>|<span data-ttu-id="6539d-155">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="6539d-155">OS Description.</span></span>|
|<span data-ttu-id="6539d-156">userName</span><span class="sxs-lookup"><span data-stu-id="6539d-156">userName</span></span>|<span data-ttu-id="6539d-157">String</span><span class="sxs-lookup"><span data-stu-id="6539d-157">String</span></span>|<span data-ttu-id="6539d-158">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="6539d-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6539d-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6539d-159">Relationships</span></span>
<span data-ttu-id="6539d-160">なし</span><span class="sxs-lookup"><span data-stu-id="6539d-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6539d-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6539d-161">JSON Representation</span></span>
<span data-ttu-id="6539d-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6539d-162">Here is a JSON representation of the resource.</span></span>
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





