---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 39f7331f8bc83840b8b5865cb71414382b3d5a50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963690"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="6e776-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e776-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="6e776-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e776-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e776-105">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e776-105">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="6e776-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e776-106">Methods</span></span>
|<span data-ttu-id="6e776-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e776-107">Method</span></span>|<span data-ttu-id="6e776-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e776-108">Return Type</span></span>|<span data-ttu-id="6e776-109">説明</span><span class="sxs-lookup"><span data-stu-id="6e776-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e776-110">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="6e776-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="6e776-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e776-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6e776-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6e776-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="6e776-113">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="6e776-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="6e776-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6e776-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6e776-115">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6e776-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="6e776-116">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="6e776-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="6e776-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6e776-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6e776-118">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e776-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="6e776-119">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="6e776-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="6e776-120">なし</span><span class="sxs-lookup"><span data-stu-id="6e776-120">None</span></span>|<span data-ttu-id="6e776-121">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6e776-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="6e776-122">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="6e776-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="6e776-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6e776-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="6e776-124">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6e776-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e776-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e776-125">Properties</span></span>
|<span data-ttu-id="6e776-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e776-126">Property</span></span>|<span data-ttu-id="6e776-127">型</span><span class="sxs-lookup"><span data-stu-id="6e776-127">Type</span></span>|<span data-ttu-id="6e776-128">説明</span><span class="sxs-lookup"><span data-stu-id="6e776-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e776-129">ID</span><span class="sxs-lookup"><span data-stu-id="6e776-129">id</span></span>|<span data-ttu-id="6e776-130">String</span><span class="sxs-lookup"><span data-stu-id="6e776-130">String</span></span>|<span data-ttu-id="6e776-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6e776-131">Key of the entity.</span></span>|
|<span data-ttu-id="6e776-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="6e776-132">deviceName</span></span>|<span data-ttu-id="6e776-133">String</span><span class="sxs-lookup"><span data-stu-id="6e776-133">String</span></span>|<span data-ttu-id="6e776-134">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="6e776-134">Device name.</span></span>|
|<span data-ttu-id="6e776-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="6e776-135">deviceId</span></span>|<span data-ttu-id="6e776-136">String</span><span class="sxs-lookup"><span data-stu-id="6e776-136">String</span></span>|<span data-ttu-id="6e776-137">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="6e776-137">Device Id.</span></span>|
|<span data-ttu-id="6e776-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6e776-138">lastSyncDateTime</span></span>|<span data-ttu-id="6e776-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e776-139">DateTimeOffset</span></span>|<span data-ttu-id="6e776-140">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="6e776-140">Last sync date and time.</span></span>|
|<span data-ttu-id="6e776-141">installState</span><span class="sxs-lookup"><span data-stu-id="6e776-141">installState</span></span>|[<span data-ttu-id="6e776-142">installState</span><span class="sxs-lookup"><span data-stu-id="6e776-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="6e776-143">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="6e776-143">The install state of the eBook.</span></span> <span data-ttu-id="6e776-144">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="6e776-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="6e776-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="6e776-145">errorCode</span></span>|<span data-ttu-id="6e776-146">String</span><span class="sxs-lookup"><span data-stu-id="6e776-146">String</span></span>|<span data-ttu-id="6e776-147">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="6e776-147">The error code for install failures.</span></span>|
|<span data-ttu-id="6e776-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="6e776-148">osVersion</span></span>|<span data-ttu-id="6e776-149">String</span><span class="sxs-lookup"><span data-stu-id="6e776-149">String</span></span>|<span data-ttu-id="6e776-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="6e776-150">OS Version.</span></span>|
|<span data-ttu-id="6e776-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="6e776-151">osDescription</span></span>|<span data-ttu-id="6e776-152">String</span><span class="sxs-lookup"><span data-stu-id="6e776-152">String</span></span>|<span data-ttu-id="6e776-153">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="6e776-153">OS Description.</span></span>|
|<span data-ttu-id="6e776-154">userName</span><span class="sxs-lookup"><span data-stu-id="6e776-154">userName</span></span>|<span data-ttu-id="6e776-155">String</span><span class="sxs-lookup"><span data-stu-id="6e776-155">String</span></span>|<span data-ttu-id="6e776-156">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="6e776-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e776-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e776-157">Relationships</span></span>
<span data-ttu-id="6e776-158">なし</span><span class="sxs-lookup"><span data-stu-id="6e776-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e776-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e776-159">JSON Representation</span></span>
<span data-ttu-id="6e776-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e776-160">Here is a JSON representation of the resource.</span></span>
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



