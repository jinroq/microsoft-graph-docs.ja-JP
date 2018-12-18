---
title: remoteActionAudit リソースの種類
description: 特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。
author: tfitzmac
ms.openlocfilehash: 48d74cb088a2e16e244898834e3d717302713e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323479"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="b70f0-103">remoteActionAudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b70f0-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="b70f0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b70f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b70f0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b70f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b70f0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b70f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b70f0-107">特定のテナントに属するデバイス上で初期化されたリモートの操作のレポートです。</span><span class="sxs-lookup"><span data-stu-id="b70f0-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="b70f0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b70f0-108">Methods</span></span>
|<span data-ttu-id="b70f0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b70f0-109">Method</span></span>|<span data-ttu-id="b70f0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b70f0-110">Return Type</span></span>|<span data-ttu-id="b70f0-111">説明</span><span class="sxs-lookup"><span data-stu-id="b70f0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b70f0-112">リスト remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="b70f0-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="b70f0-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b70f0-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="b70f0-114">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="b70f0-115">RemoteActionAudit を取得します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="b70f0-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b70f0-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b70f0-117">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b70f0-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="b70f0-118">RemoteActionAudit を作成します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="b70f0-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b70f0-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b70f0-120">新しい[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="b70f0-121">RemoteActionAudit を削除します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="b70f0-122">なし</span><span class="sxs-lookup"><span data-stu-id="b70f0-122">None</span></span>|<span data-ttu-id="b70f0-123">の[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="b70f0-124">RemoteActionAudit を更新します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="b70f0-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b70f0-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b70f0-126">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b70f0-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b70f0-127">Properties</span><span class="sxs-lookup"><span data-stu-id="b70f0-127">Properties</span></span>
|<span data-ttu-id="b70f0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b70f0-128">Property</span></span>|<span data-ttu-id="b70f0-129">種類</span><span class="sxs-lookup"><span data-stu-id="b70f0-129">Type</span></span>|<span data-ttu-id="b70f0-130">説明</span><span class="sxs-lookup"><span data-stu-id="b70f0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b70f0-131">ID</span><span class="sxs-lookup"><span data-stu-id="b70f0-131">id</span></span>|<span data-ttu-id="b70f0-132">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-132">String</span></span>|<span data-ttu-id="b70f0-133">レポートの id。</span><span class="sxs-lookup"><span data-stu-id="b70f0-133">Report Id.</span></span>|
|<span data-ttu-id="b70f0-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b70f0-134">deviceDisplayName</span></span>|<span data-ttu-id="b70f0-135">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-135">String</span></span>|<span data-ttu-id="b70f0-136">Intune デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-136">Intune device name.</span></span>|
|<span data-ttu-id="b70f0-137">userName</span><span class="sxs-lookup"><span data-stu-id="b70f0-137">userName</span></span>|<span data-ttu-id="b70f0-138">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-138">String</span></span>|<span data-ttu-id="b70f0-139">\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="b70f0-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="b70f0-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b70f0-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="b70f0-141">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-141">String</span></span>|<span data-ttu-id="b70f0-142">デバイスのアクションを開始したユーザーは、UPN 形式です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="b70f0-143">action</span><span class="sxs-lookup"><span data-stu-id="b70f0-143">action</span></span>|[<span data-ttu-id="b70f0-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="b70f0-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="b70f0-145">アクション名。</span><span class="sxs-lookup"><span data-stu-id="b70f0-145">The action name.</span></span> <span data-ttu-id="b70f0-146">使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="b70f0-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="b70f0-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="b70f0-147">requestDateTime</span></span>|<span data-ttu-id="b70f0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b70f0-148">DateTimeOffset</span></span>|<span data-ttu-id="b70f0-149">UTC で指定されたアクションを発行した時の時間です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="b70f0-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b70f0-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="b70f0-151">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-151">String</span></span>|<span data-ttu-id="b70f0-152">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="b70f0-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="b70f0-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="b70f0-153">deviceIMEI</span></span>|<span data-ttu-id="b70f0-154">String</span><span class="sxs-lookup"><span data-stu-id="b70f0-154">String</span></span>|<span data-ttu-id="b70f0-155">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="b70f0-155">IMEI of the device.</span></span>|
|<span data-ttu-id="b70f0-156">actionState</span><span class="sxs-lookup"><span data-stu-id="b70f0-156">actionState</span></span>|[<span data-ttu-id="b70f0-157">actionState</span><span class="sxs-lookup"><span data-stu-id="b70f0-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b70f0-158">動作状態です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-158">Action state.</span></span> <span data-ttu-id="b70f0-159">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b70f0-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b70f0-160">Relationships</span></span>
<span data-ttu-id="b70f0-161">なし</span><span class="sxs-lookup"><span data-stu-id="b70f0-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b70f0-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b70f0-162">JSON Representation</span></span>
<span data-ttu-id="b70f0-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b70f0-163">Here is a JSON representation of the resource.</span></span>
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





