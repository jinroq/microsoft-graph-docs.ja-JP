---
title: remoteactionaudit リソースの種類
description: 特定のテナントに属するデバイスで開始されたリモートアクションのレポート。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c06f7472addff7c475eeeb8ac3f1a26cc7ea78bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165878"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="362e9-103">remoteactionaudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="362e9-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="362e9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="362e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="362e9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="362e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="362e9-106">特定のテナントに属するデバイスで開始されたリモートアクションのレポート。</span><span class="sxs-lookup"><span data-stu-id="362e9-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="362e9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="362e9-107">Methods</span></span>
|<span data-ttu-id="362e9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="362e9-108">Method</span></span>|<span data-ttu-id="362e9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="362e9-109">Return Type</span></span>|<span data-ttu-id="362e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="362e9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="362e9-111">remoteactionaudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="362e9-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="362e9-112">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="362e9-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="362e9-113">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="362e9-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="362e9-114">remoteactionaudit の取得</span><span class="sxs-lookup"><span data-stu-id="362e9-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="362e9-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="362e9-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="362e9-116">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="362e9-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="362e9-117">remoteactionaudit の作成</span><span class="sxs-lookup"><span data-stu-id="362e9-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="362e9-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="362e9-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="362e9-119">新しい[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="362e9-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="362e9-120">remoteactionaudit の削除</span><span class="sxs-lookup"><span data-stu-id="362e9-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="362e9-121">なし</span><span class="sxs-lookup"><span data-stu-id="362e9-121">None</span></span>|<span data-ttu-id="362e9-122">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="362e9-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="362e9-123">remoteactionaudit の更新</span><span class="sxs-lookup"><span data-stu-id="362e9-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="362e9-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="362e9-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="362e9-125">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="362e9-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="362e9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="362e9-126">Properties</span></span>
|<span data-ttu-id="362e9-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="362e9-127">Property</span></span>|<span data-ttu-id="362e9-128">型</span><span class="sxs-lookup"><span data-stu-id="362e9-128">Type</span></span>|<span data-ttu-id="362e9-129">説明</span><span class="sxs-lookup"><span data-stu-id="362e9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="362e9-130">id</span><span class="sxs-lookup"><span data-stu-id="362e9-130">id</span></span>|<span data-ttu-id="362e9-131">String</span><span class="sxs-lookup"><span data-stu-id="362e9-131">String</span></span>|<span data-ttu-id="362e9-132">レポート Id。</span><span class="sxs-lookup"><span data-stu-id="362e9-132">Report Id.</span></span>|
|<span data-ttu-id="362e9-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="362e9-133">deviceDisplayName</span></span>|<span data-ttu-id="362e9-134">String</span><span class="sxs-lookup"><span data-stu-id="362e9-134">String</span></span>|<span data-ttu-id="362e9-135">Intune デバイス名。</span><span class="sxs-lookup"><span data-stu-id="362e9-135">Intune device name.</span></span>|
|<span data-ttu-id="362e9-136">userName</span><span class="sxs-lookup"><span data-stu-id="362e9-136">userName</span></span>|<span data-ttu-id="362e9-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="362e9-137">String</span></span>|<span data-ttu-id="362e9-138">\[非\]推奨 initiatedbyuserprincipalname を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="362e9-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="362e9-139">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="362e9-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="362e9-140">String</span><span class="sxs-lookup"><span data-stu-id="362e9-140">String</span></span>|<span data-ttu-id="362e9-141">デバイスのアクションを開始したユーザーの形式は UPN です。</span><span class="sxs-lookup"><span data-stu-id="362e9-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="362e9-142">action</span><span class="sxs-lookup"><span data-stu-id="362e9-142">action</span></span>|[<span data-ttu-id="362e9-143">remoteaction</span><span class="sxs-lookup"><span data-stu-id="362e9-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="362e9-144">アクション名。</span><span class="sxs-lookup"><span data-stu-id="362e9-144">The action name.</span></span> <span data-ttu-id="362e9-145">可能な値: `unknown`、 `factoryReset` `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`、、、、、、、、、、、、 `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="362e9-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="362e9-146">requestdatetime</span><span class="sxs-lookup"><span data-stu-id="362e9-146">requestDateTime</span></span>|<span data-ttu-id="362e9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="362e9-147">DateTimeOffset</span></span>|<span data-ttu-id="362e9-148">アクションが発行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="362e9-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="362e9-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="362e9-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="362e9-150">String</span><span class="sxs-lookup"><span data-stu-id="362e9-150">String</span></span>|<span data-ttu-id="362e9-151">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="362e9-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="362e9-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="362e9-152">deviceIMEI</span></span>|<span data-ttu-id="362e9-153">String</span><span class="sxs-lookup"><span data-stu-id="362e9-153">String</span></span>|<span data-ttu-id="362e9-154">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="362e9-154">IMEI of the device.</span></span>|
|<span data-ttu-id="362e9-155">actionState</span><span class="sxs-lookup"><span data-stu-id="362e9-155">actionState</span></span>|[<span data-ttu-id="362e9-156">actionState</span><span class="sxs-lookup"><span data-stu-id="362e9-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="362e9-157">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="362e9-157">Action state.</span></span> <span data-ttu-id="362e9-158">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="362e9-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="362e9-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="362e9-159">Relationships</span></span>
<span data-ttu-id="362e9-160">なし</span><span class="sxs-lookup"><span data-stu-id="362e9-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="362e9-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="362e9-161">JSON Representation</span></span>
<span data-ttu-id="362e9-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="362e9-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```




