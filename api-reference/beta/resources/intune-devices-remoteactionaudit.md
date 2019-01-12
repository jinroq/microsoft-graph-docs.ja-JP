---
title: remoteActionAudit リソースの種類
description: 特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad583f13311e5baece70c5ec28ca8f7c73f5349e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972594"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="799d8-103">remoteActionAudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="799d8-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="799d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="799d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="799d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="799d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="799d8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="799d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="799d8-107">特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。</span><span class="sxs-lookup"><span data-stu-id="799d8-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="799d8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="799d8-108">Methods</span></span>
|<span data-ttu-id="799d8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="799d8-109">Method</span></span>|<span data-ttu-id="799d8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="799d8-110">Return Type</span></span>|<span data-ttu-id="799d8-111">説明</span><span class="sxs-lookup"><span data-stu-id="799d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="799d8-112">リスト remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="799d8-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="799d8-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="799d8-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="799d8-114">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="799d8-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="799d8-115">RemoteActionAudit を取得します。</span><span class="sxs-lookup"><span data-stu-id="799d8-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="799d8-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="799d8-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="799d8-117">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="799d8-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="799d8-118">RemoteActionAudit を作成します。</span><span class="sxs-lookup"><span data-stu-id="799d8-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="799d8-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="799d8-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="799d8-120">新しい[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="799d8-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="799d8-121">RemoteActionAudit を削除します。</span><span class="sxs-lookup"><span data-stu-id="799d8-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="799d8-122">なし</span><span class="sxs-lookup"><span data-stu-id="799d8-122">None</span></span>|<span data-ttu-id="799d8-123">の[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="799d8-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="799d8-124">RemoteActionAudit を更新します。</span><span class="sxs-lookup"><span data-stu-id="799d8-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="799d8-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="799d8-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="799d8-126">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="799d8-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="799d8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="799d8-127">Properties</span></span>
|<span data-ttu-id="799d8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="799d8-128">Property</span></span>|<span data-ttu-id="799d8-129">型</span><span class="sxs-lookup"><span data-stu-id="799d8-129">Type</span></span>|<span data-ttu-id="799d8-130">説明</span><span class="sxs-lookup"><span data-stu-id="799d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="799d8-131">ID</span><span class="sxs-lookup"><span data-stu-id="799d8-131">id</span></span>|<span data-ttu-id="799d8-132">String</span><span class="sxs-lookup"><span data-stu-id="799d8-132">String</span></span>|<span data-ttu-id="799d8-133">レポートの id。</span><span class="sxs-lookup"><span data-stu-id="799d8-133">Report Id.</span></span>|
|<span data-ttu-id="799d8-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="799d8-134">deviceDisplayName</span></span>|<span data-ttu-id="799d8-135">String</span><span class="sxs-lookup"><span data-stu-id="799d8-135">String</span></span>|<span data-ttu-id="799d8-136">Intune デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="799d8-136">Intune device name.</span></span>|
|<span data-ttu-id="799d8-137">userName</span><span class="sxs-lookup"><span data-stu-id="799d8-137">userName</span></span>|<span data-ttu-id="799d8-138">String</span><span class="sxs-lookup"><span data-stu-id="799d8-138">String</span></span>|<span data-ttu-id="799d8-139">\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="799d8-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="799d8-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="799d8-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="799d8-141">String</span><span class="sxs-lookup"><span data-stu-id="799d8-141">String</span></span>|<span data-ttu-id="799d8-142">デバイスのアクションを開始したユーザーは、UPN 形式です。</span><span class="sxs-lookup"><span data-stu-id="799d8-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="799d8-143">action</span><span class="sxs-lookup"><span data-stu-id="799d8-143">action</span></span>|[<span data-ttu-id="799d8-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="799d8-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="799d8-145">アクション名。</span><span class="sxs-lookup"><span data-stu-id="799d8-145">The action name.</span></span> <span data-ttu-id="799d8-146">使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="799d8-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="799d8-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="799d8-147">requestDateTime</span></span>|<span data-ttu-id="799d8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="799d8-148">DateTimeOffset</span></span>|<span data-ttu-id="799d8-149">UTC で指定されたアクションを発行した時の時間です。</span><span class="sxs-lookup"><span data-stu-id="799d8-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="799d8-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="799d8-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="799d8-151">String</span><span class="sxs-lookup"><span data-stu-id="799d8-151">String</span></span>|<span data-ttu-id="799d8-152">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="799d8-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="799d8-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="799d8-153">deviceIMEI</span></span>|<span data-ttu-id="799d8-154">String</span><span class="sxs-lookup"><span data-stu-id="799d8-154">String</span></span>|<span data-ttu-id="799d8-155">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="799d8-155">IMEI of the device.</span></span>|
|<span data-ttu-id="799d8-156">actionState</span><span class="sxs-lookup"><span data-stu-id="799d8-156">actionState</span></span>|[<span data-ttu-id="799d8-157">actionState</span><span class="sxs-lookup"><span data-stu-id="799d8-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="799d8-158">動作状態です。</span><span class="sxs-lookup"><span data-stu-id="799d8-158">Action state.</span></span> <span data-ttu-id="799d8-159">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="799d8-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="799d8-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="799d8-160">Relationships</span></span>
<span data-ttu-id="799d8-161">なし</span><span class="sxs-lookup"><span data-stu-id="799d8-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="799d8-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="799d8-162">JSON Representation</span></span>
<span data-ttu-id="799d8-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="799d8-163">Here is a JSON representation of the resource.</span></span>
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





