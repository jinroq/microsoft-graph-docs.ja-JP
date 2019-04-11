---
title: remoteactionaudit リソースの種類
description: 特定のテナントに属するデバイスで開始されたリモートアクションのレポート。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a4a95019db6ca3025d0090981ca6563d335ffe
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804264"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="f4eeb-103">remoteactionaudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4eeb-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="f4eeb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4eeb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4eeb-106">特定のテナントに属するデバイスで開始されたリモートアクションのレポート。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="f4eeb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4eeb-107">Methods</span></span>
|<span data-ttu-id="f4eeb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4eeb-108">Method</span></span>|<span data-ttu-id="f4eeb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f4eeb-109">Return Type</span></span>|<span data-ttu-id="f4eeb-110">説明</span><span class="sxs-lookup"><span data-stu-id="f4eeb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4eeb-111">remoteactionaudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f4eeb-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="f4eeb-112">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f4eeb-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="f4eeb-113">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="f4eeb-114">remoteactionaudit の取得</span><span class="sxs-lookup"><span data-stu-id="f4eeb-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="f4eeb-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f4eeb-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f4eeb-116">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="f4eeb-117">remoteactionaudit の作成</span><span class="sxs-lookup"><span data-stu-id="f4eeb-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="f4eeb-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f4eeb-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f4eeb-119">新しい[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="f4eeb-120">remoteactionaudit の削除</span><span class="sxs-lookup"><span data-stu-id="f4eeb-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="f4eeb-121">なし</span><span class="sxs-lookup"><span data-stu-id="f4eeb-121">None</span></span>|<span data-ttu-id="f4eeb-122">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="f4eeb-123">remoteactionaudit の更新</span><span class="sxs-lookup"><span data-stu-id="f4eeb-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="f4eeb-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f4eeb-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f4eeb-125">[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4eeb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4eeb-126">Properties</span></span>
|<span data-ttu-id="f4eeb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4eeb-127">Property</span></span>|<span data-ttu-id="f4eeb-128">型</span><span class="sxs-lookup"><span data-stu-id="f4eeb-128">Type</span></span>|<span data-ttu-id="f4eeb-129">説明</span><span class="sxs-lookup"><span data-stu-id="f4eeb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4eeb-130">id</span><span class="sxs-lookup"><span data-stu-id="f4eeb-130">id</span></span>|<span data-ttu-id="f4eeb-131">String</span><span class="sxs-lookup"><span data-stu-id="f4eeb-131">String</span></span>|<span data-ttu-id="f4eeb-132">レポート Id。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-132">Report Id.</span></span>|
|<span data-ttu-id="f4eeb-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4eeb-133">deviceDisplayName</span></span>|<span data-ttu-id="f4eeb-134">String</span><span class="sxs-lookup"><span data-stu-id="f4eeb-134">String</span></span>|<span data-ttu-id="f4eeb-135">Intune デバイス名。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-135">Intune device name.</span></span>|
|<span data-ttu-id="f4eeb-136">userName</span><span class="sxs-lookup"><span data-stu-id="f4eeb-136">userName</span></span>|<span data-ttu-id="f4eeb-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f4eeb-137">String</span></span>|<span data-ttu-id="f4eeb-138">\[非\]推奨 initiatedbyuserprincipalname を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="f4eeb-139">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4eeb-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="f4eeb-140">文字列</span><span class="sxs-lookup"><span data-stu-id="f4eeb-140">String</span></span>|<span data-ttu-id="f4eeb-141">デバイスのアクションを開始したユーザーの形式は UPN です。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="f4eeb-142">アクション</span><span class="sxs-lookup"><span data-stu-id="f4eeb-142">action</span></span>|[<span data-ttu-id="f4eeb-143">remoteaction</span><span class="sxs-lookup"><span data-stu-id="f4eeb-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="f4eeb-144">アクション名。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-144">The action name.</span></span> <span data-ttu-id="f4eeb-145">可能な値: `unknown`、 `factoryReset` `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`、、、、、、、、、、、、 `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="f4eeb-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="f4eeb-146">requestdatetime</span><span class="sxs-lookup"><span data-stu-id="f4eeb-146">requestDateTime</span></span>|<span data-ttu-id="f4eeb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4eeb-147">DateTimeOffset</span></span>|<span data-ttu-id="f4eeb-148">アクションが発行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="f4eeb-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4eeb-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="f4eeb-150">文字列</span><span class="sxs-lookup"><span data-stu-id="f4eeb-150">String</span></span>|<span data-ttu-id="f4eeb-151">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="f4eeb-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="f4eeb-152">deviceIMEI</span></span>|<span data-ttu-id="f4eeb-153">文字列</span><span class="sxs-lookup"><span data-stu-id="f4eeb-153">String</span></span>|<span data-ttu-id="f4eeb-154">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-154">IMEI of the device.</span></span>|
|<span data-ttu-id="f4eeb-155">actionState</span><span class="sxs-lookup"><span data-stu-id="f4eeb-155">actionState</span></span>|[<span data-ttu-id="f4eeb-156">actionState</span><span class="sxs-lookup"><span data-stu-id="f4eeb-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f4eeb-157">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-157">Action state.</span></span> <span data-ttu-id="f4eeb-158">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4eeb-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4eeb-159">Relationships</span></span>
<span data-ttu-id="f4eeb-160">なし</span><span class="sxs-lookup"><span data-stu-id="f4eeb-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4eeb-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4eeb-161">JSON Representation</span></span>
<span data-ttu-id="f4eeb-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4eeb-162">Here is a JSON representation of the resource.</span></span>
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





