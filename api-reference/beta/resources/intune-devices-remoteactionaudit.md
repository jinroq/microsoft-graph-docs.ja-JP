---
title: remoteActionAudit リソースの種類
description: 特定のテナントに属するデバイスで開始されたリモートアクションのレポート。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a691997c985de17646a28d3a72262ae3c99c174
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968324"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="a7e6c-103">remoteActionAudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7e6c-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="a7e6c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7e6c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e6c-106">特定のテナントに属するデバイスで開始されたリモートアクションのレポート。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="a7e6c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7e6c-107">Methods</span></span>
|<span data-ttu-id="a7e6c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7e6c-108">Method</span></span>|<span data-ttu-id="a7e6c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7e6c-109">Return Type</span></span>|<span data-ttu-id="a7e6c-110">説明</span><span class="sxs-lookup"><span data-stu-id="a7e6c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7e6c-111">RemoteActionAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a7e6c-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="a7e6c-112">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7e6c-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="a7e6c-113">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="a7e6c-114">RemoteActionAudit の取得</span><span class="sxs-lookup"><span data-stu-id="a7e6c-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="a7e6c-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a7e6c-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a7e6c-116">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="a7e6c-117">RemoteActionAudit の作成</span><span class="sxs-lookup"><span data-stu-id="a7e6c-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="a7e6c-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a7e6c-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a7e6c-119">新しい[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="a7e6c-120">RemoteActionAudit の削除</span><span class="sxs-lookup"><span data-stu-id="a7e6c-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="a7e6c-121">None</span><span class="sxs-lookup"><span data-stu-id="a7e6c-121">None</span></span>|<span data-ttu-id="a7e6c-122">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="a7e6c-123">RemoteActionAudit の更新</span><span class="sxs-lookup"><span data-stu-id="a7e6c-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="a7e6c-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a7e6c-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a7e6c-125">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7e6c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e6c-126">Properties</span></span>
|<span data-ttu-id="a7e6c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e6c-127">Property</span></span>|<span data-ttu-id="a7e6c-128">型</span><span class="sxs-lookup"><span data-stu-id="a7e6c-128">Type</span></span>|<span data-ttu-id="a7e6c-129">説明</span><span class="sxs-lookup"><span data-stu-id="a7e6c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e6c-130">id</span><span class="sxs-lookup"><span data-stu-id="a7e6c-130">id</span></span>|<span data-ttu-id="a7e6c-131">String</span><span class="sxs-lookup"><span data-stu-id="a7e6c-131">String</span></span>|<span data-ttu-id="a7e6c-132">レポート Id。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-132">Report Id.</span></span>|
|<span data-ttu-id="a7e6c-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7e6c-133">deviceDisplayName</span></span>|<span data-ttu-id="a7e6c-134">String</span><span class="sxs-lookup"><span data-stu-id="a7e6c-134">String</span></span>|<span data-ttu-id="a7e6c-135">Intune デバイス名。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-135">Intune device name.</span></span>|
|<span data-ttu-id="a7e6c-136">userName</span><span class="sxs-lookup"><span data-stu-id="a7e6c-136">userName</span></span>|<span data-ttu-id="a7e6c-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a7e6c-137">String</span></span>|<span data-ttu-id="a7e6c-138">\[非\]推奨 InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="a7e6c-139">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7e6c-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="a7e6c-140">String</span><span class="sxs-lookup"><span data-stu-id="a7e6c-140">String</span></span>|<span data-ttu-id="a7e6c-141">デバイスのアクションを開始したユーザーの形式は UPN です。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="a7e6c-142">action</span><span class="sxs-lookup"><span data-stu-id="a7e6c-142">action</span></span>|[<span data-ttu-id="a7e6c-143">remoteAction</span><span class="sxs-lookup"><span data-stu-id="a7e6c-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="a7e6c-144">アクション名。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-144">The action name.</span></span> <span data-ttu-id="a7e6c-145">可能な値は、`unknown`、`factoryReset`、`removeCompanyData`、`resetPasscode`、`remoteLock`、`enableLostMode`、`disableLostMode`、`locateDevice`、`rebootNow`、`recoverPasscode`、`cleanWindowsDevice`、`logoutSharedAppleDeviceActiveUser`、`quickScan`、`fullScan`、`windowsDefenderUpdateSignatures`、`factoryResetKeepEnrollmentData`、`updateDeviceAccount`、`automaticRedeployment`、`shutDown`、`rotateFileVaultKey`、`getFileVaultKey` です。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateFileVaultKey`, `getFileVaultKey`.</span></span>|
|<span data-ttu-id="a7e6c-146">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e6c-146">requestDateTime</span></span>|<span data-ttu-id="a7e6c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7e6c-147">DateTimeOffset</span></span>|<span data-ttu-id="a7e6c-148">アクションが発行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="a7e6c-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7e6c-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="a7e6c-150">String</span><span class="sxs-lookup"><span data-stu-id="a7e6c-150">String</span></span>|<span data-ttu-id="a7e6c-151">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="a7e6c-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="a7e6c-152">deviceIMEI</span></span>|<span data-ttu-id="a7e6c-153">String</span><span class="sxs-lookup"><span data-stu-id="a7e6c-153">String</span></span>|<span data-ttu-id="a7e6c-154">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-154">IMEI of the device.</span></span>|
|<span data-ttu-id="a7e6c-155">actionState</span><span class="sxs-lookup"><span data-stu-id="a7e6c-155">actionState</span></span>|[<span data-ttu-id="a7e6c-156">actionState</span><span class="sxs-lookup"><span data-stu-id="a7e6c-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a7e6c-157">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-157">Action state.</span></span> <span data-ttu-id="a7e6c-158">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7e6c-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7e6c-159">Relationships</span></span>
<span data-ttu-id="a7e6c-160">なし</span><span class="sxs-lookup"><span data-stu-id="a7e6c-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7e6c-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7e6c-161">JSON Representation</span></span>
<span data-ttu-id="a7e6c-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7e6c-162">Here is a JSON representation of the resource.</span></span>
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





