---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
ms.openlocfilehash: 9fb7f7b2bbbb46a068d5ba41db022eed3072520d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024182"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="15e9d-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15e9d-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="15e9d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15e9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15e9d-105">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15e9d-105">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="15e9d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="15e9d-106">Methods</span></span>
|<span data-ttu-id="15e9d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="15e9d-107">Method</span></span>|<span data-ttu-id="15e9d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15e9d-108">Return Type</span></span>|<span data-ttu-id="15e9d-109">説明</span><span class="sxs-lookup"><span data-stu-id="15e9d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15e9d-110">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="15e9d-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="15e9d-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="15e9d-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="15e9d-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="15e9d-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="15e9d-113">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="15e9d-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="15e9d-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="15e9d-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="15e9d-115">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="15e9d-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="15e9d-116">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="15e9d-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="15e9d-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="15e9d-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="15e9d-118">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15e9d-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="15e9d-119">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="15e9d-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="15e9d-120">なし</span><span class="sxs-lookup"><span data-stu-id="15e9d-120">None</span></span>|<span data-ttu-id="15e9d-121">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="15e9d-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="15e9d-122">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="15e9d-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="15e9d-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="15e9d-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="15e9d-124">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15e9d-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15e9d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e9d-125">Properties</span></span>
|<span data-ttu-id="15e9d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e9d-126">Property</span></span>|<span data-ttu-id="15e9d-127">型</span><span class="sxs-lookup"><span data-stu-id="15e9d-127">Type</span></span>|<span data-ttu-id="15e9d-128">説明</span><span class="sxs-lookup"><span data-stu-id="15e9d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e9d-129">id</span><span class="sxs-lookup"><span data-stu-id="15e9d-129">id</span></span>|<span data-ttu-id="15e9d-130">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-130">String</span></span>|<span data-ttu-id="15e9d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="15e9d-131">Key of the entity.</span></span>|
|<span data-ttu-id="15e9d-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="15e9d-132">deviceName</span></span>|<span data-ttu-id="15e9d-133">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-133">String</span></span>|<span data-ttu-id="15e9d-134">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="15e9d-134">Device name.</span></span>|
|<span data-ttu-id="15e9d-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="15e9d-135">deviceId</span></span>|<span data-ttu-id="15e9d-136">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-136">String</span></span>|<span data-ttu-id="15e9d-137">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="15e9d-137">Device Id.</span></span>|
|<span data-ttu-id="15e9d-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="15e9d-138">lastSyncDateTime</span></span>|<span data-ttu-id="15e9d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e9d-139">DateTimeOffset</span></span>|<span data-ttu-id="15e9d-140">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="15e9d-140">Last sync date and time.</span></span>|
|<span data-ttu-id="15e9d-141">installState</span><span class="sxs-lookup"><span data-stu-id="15e9d-141">installState</span></span>|[<span data-ttu-id="15e9d-142">installState</span><span class="sxs-lookup"><span data-stu-id="15e9d-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="15e9d-143">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="15e9d-143">The install state of the eBook.</span></span> <span data-ttu-id="15e9d-144">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="15e9d-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="15e9d-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="15e9d-145">errorCode</span></span>|<span data-ttu-id="15e9d-146">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-146">String</span></span>|<span data-ttu-id="15e9d-147">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="15e9d-147">The error code for install failures.</span></span>|
|<span data-ttu-id="15e9d-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="15e9d-148">osVersion</span></span>|<span data-ttu-id="15e9d-149">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-149">String</span></span>|<span data-ttu-id="15e9d-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="15e9d-150">OS Version.</span></span>|
|<span data-ttu-id="15e9d-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="15e9d-151">osDescription</span></span>|<span data-ttu-id="15e9d-152">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-152">String</span></span>|<span data-ttu-id="15e9d-153">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="15e9d-153">OS Description.</span></span>|
|<span data-ttu-id="15e9d-154">userName</span><span class="sxs-lookup"><span data-stu-id="15e9d-154">userName</span></span>|<span data-ttu-id="15e9d-155">String</span><span class="sxs-lookup"><span data-stu-id="15e9d-155">String</span></span>|<span data-ttu-id="15e9d-156">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="15e9d-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15e9d-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15e9d-157">Relationships</span></span>
<span data-ttu-id="15e9d-158">なし</span><span class="sxs-lookup"><span data-stu-id="15e9d-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15e9d-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15e9d-159">JSON Representation</span></span>
<span data-ttu-id="15e9d-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15e9d-160">Here is a JSON representation of the resource.</span></span>
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



