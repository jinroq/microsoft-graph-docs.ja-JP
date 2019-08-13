---
title: deviceInstallState リソースの種類
description: デバイスのインストール状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2a62621fec39b50aac9ea422dad4dc35b85473b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335215"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="843e3-103">deviceInstallState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="843e3-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="843e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="843e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="843e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="843e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="843e3-106">デバイスのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="843e3-106">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="843e3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="843e3-107">Methods</span></span>
|<span data-ttu-id="843e3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="843e3-108">Method</span></span>|<span data-ttu-id="843e3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="843e3-109">Return Type</span></span>|<span data-ttu-id="843e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="843e3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="843e3-111">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="843e3-111">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="843e3-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="843e3-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="843e3-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="843e3-113">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="843e3-114">deviceInstallState の取得</span><span class="sxs-lookup"><span data-stu-id="843e3-114">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="843e3-115">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="843e3-115">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="843e3-116">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="843e3-116">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="843e3-117">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="843e3-117">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="843e3-118">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="843e3-118">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="843e3-119">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="843e3-119">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="843e3-120">deviceInstallState の削除</span><span class="sxs-lookup"><span data-stu-id="843e3-120">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="843e3-121">なし</span><span class="sxs-lookup"><span data-stu-id="843e3-121">None</span></span>|<span data-ttu-id="843e3-122">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="843e3-122">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="843e3-123">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="843e3-123">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="843e3-124">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="843e3-124">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="843e3-125">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="843e3-125">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="843e3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="843e3-126">Properties</span></span>
|<span data-ttu-id="843e3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="843e3-127">Property</span></span>|<span data-ttu-id="843e3-128">型</span><span class="sxs-lookup"><span data-stu-id="843e3-128">Type</span></span>|<span data-ttu-id="843e3-129">説明</span><span class="sxs-lookup"><span data-stu-id="843e3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="843e3-130">id</span><span class="sxs-lookup"><span data-stu-id="843e3-130">id</span></span>|<span data-ttu-id="843e3-131">String</span><span class="sxs-lookup"><span data-stu-id="843e3-131">String</span></span>|<span data-ttu-id="843e3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="843e3-132">Key of the entity.</span></span>|
|<span data-ttu-id="843e3-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="843e3-133">deviceName</span></span>|<span data-ttu-id="843e3-134">String</span><span class="sxs-lookup"><span data-stu-id="843e3-134">String</span></span>|<span data-ttu-id="843e3-135">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="843e3-135">Device name.</span></span>|
|<span data-ttu-id="843e3-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="843e3-136">deviceId</span></span>|<span data-ttu-id="843e3-137">String</span><span class="sxs-lookup"><span data-stu-id="843e3-137">String</span></span>|<span data-ttu-id="843e3-138">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="843e3-138">Device Id.</span></span>|
|<span data-ttu-id="843e3-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="843e3-139">lastSyncDateTime</span></span>|<span data-ttu-id="843e3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843e3-140">DateTimeOffset</span></span>|<span data-ttu-id="843e3-141">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="843e3-141">Last sync date and time.</span></span>|
|<span data-ttu-id="843e3-142">installState</span><span class="sxs-lookup"><span data-stu-id="843e3-142">installState</span></span>|[<span data-ttu-id="843e3-143">installState</span><span class="sxs-lookup"><span data-stu-id="843e3-143">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="843e3-144">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="843e3-144">The install state of the eBook.</span></span> <span data-ttu-id="843e3-145">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="843e3-145">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="843e3-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="843e3-146">errorCode</span></span>|<span data-ttu-id="843e3-147">String</span><span class="sxs-lookup"><span data-stu-id="843e3-147">String</span></span>|<span data-ttu-id="843e3-148">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="843e3-148">The error code for install failures.</span></span>|
|<span data-ttu-id="843e3-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="843e3-149">osVersion</span></span>|<span data-ttu-id="843e3-150">String</span><span class="sxs-lookup"><span data-stu-id="843e3-150">String</span></span>|<span data-ttu-id="843e3-151">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="843e3-151">OS Version.</span></span>|
|<span data-ttu-id="843e3-152">osDescription</span><span class="sxs-lookup"><span data-stu-id="843e3-152">osDescription</span></span>|<span data-ttu-id="843e3-153">String</span><span class="sxs-lookup"><span data-stu-id="843e3-153">String</span></span>|<span data-ttu-id="843e3-154">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="843e3-154">OS Description.</span></span>|
|<span data-ttu-id="843e3-155">userName</span><span class="sxs-lookup"><span data-stu-id="843e3-155">userName</span></span>|<span data-ttu-id="843e3-156">String</span><span class="sxs-lookup"><span data-stu-id="843e3-156">String</span></span>|<span data-ttu-id="843e3-157">デバイスのユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="843e3-157">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="843e3-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="843e3-158">Relationships</span></span>
<span data-ttu-id="843e3-159">なし</span><span class="sxs-lookup"><span data-stu-id="843e3-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="843e3-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="843e3-160">JSON Representation</span></span>
<span data-ttu-id="843e3-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="843e3-161">Here is a JSON representation of the resource.</span></span>
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



