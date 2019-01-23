---
title: RemoteActionAudit を作成します。
description: 新しい remoteActionAudit オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 47ba3de19ca5cdc9b01bb3b65eb8b04e75831d87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396883"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="178c1-103">RemoteActionAudit を作成します。</span><span class="sxs-lookup"><span data-stu-id="178c1-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="178c1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="178c1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="178c1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="178c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="178c1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="178c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="178c1-107">新しい[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="178c1-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="178c1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="178c1-108">Prerequisites</span></span>
<span data-ttu-id="178c1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="178c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="178c1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="178c1-111">Permission type</span></span>|<span data-ttu-id="178c1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="178c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="178c1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="178c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="178c1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="178c1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="178c1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="178c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="178c1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="178c1-116">Not supported.</span></span>|
|<span data-ttu-id="178c1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="178c1-117">Application</span></span>|<span data-ttu-id="178c1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="178c1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="178c1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="178c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="178c1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="178c1-120">Request headers</span></span>
|<span data-ttu-id="178c1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="178c1-121">Header</span></span>|<span data-ttu-id="178c1-122">値</span><span class="sxs-lookup"><span data-stu-id="178c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="178c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="178c1-123">Authorization</span></span>|<span data-ttu-id="178c1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="178c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="178c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="178c1-125">Accept</span></span>|<span data-ttu-id="178c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="178c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="178c1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="178c1-127">Request body</span></span>
<span data-ttu-id="178c1-128">要求の本文に remoteActionAudit オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="178c1-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="178c1-129">次の表は、remoteActionAudit を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="178c1-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="178c1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="178c1-130">Property</span></span>|<span data-ttu-id="178c1-131">型</span><span class="sxs-lookup"><span data-stu-id="178c1-131">Type</span></span>|<span data-ttu-id="178c1-132">説明</span><span class="sxs-lookup"><span data-stu-id="178c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="178c1-133">id</span><span class="sxs-lookup"><span data-stu-id="178c1-133">id</span></span>|<span data-ttu-id="178c1-134">String</span><span class="sxs-lookup"><span data-stu-id="178c1-134">String</span></span>|<span data-ttu-id="178c1-135">レポートの id。</span><span class="sxs-lookup"><span data-stu-id="178c1-135">Report Id.</span></span>|
|<span data-ttu-id="178c1-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="178c1-136">deviceDisplayName</span></span>|<span data-ttu-id="178c1-137">String</span><span class="sxs-lookup"><span data-stu-id="178c1-137">String</span></span>|<span data-ttu-id="178c1-138">Intune デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="178c1-138">Intune device name.</span></span>|
|<span data-ttu-id="178c1-139">userName</span><span class="sxs-lookup"><span data-stu-id="178c1-139">userName</span></span>|<span data-ttu-id="178c1-140">String</span><span class="sxs-lookup"><span data-stu-id="178c1-140">String</span></span>|<span data-ttu-id="178c1-141">\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="178c1-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="178c1-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="178c1-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="178c1-143">String</span><span class="sxs-lookup"><span data-stu-id="178c1-143">String</span></span>|<span data-ttu-id="178c1-144">デバイスのアクションを開始したユーザーは、UPN 形式です。</span><span class="sxs-lookup"><span data-stu-id="178c1-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="178c1-145">action</span><span class="sxs-lookup"><span data-stu-id="178c1-145">action</span></span>|[<span data-ttu-id="178c1-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="178c1-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="178c1-147">アクション名。</span><span class="sxs-lookup"><span data-stu-id="178c1-147">The action name.</span></span> <span data-ttu-id="178c1-148">使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="178c1-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="178c1-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="178c1-149">requestDateTime</span></span>|<span data-ttu-id="178c1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="178c1-150">DateTimeOffset</span></span>|<span data-ttu-id="178c1-151">UTC で指定されたアクションを発行した時の時間です。</span><span class="sxs-lookup"><span data-stu-id="178c1-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="178c1-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="178c1-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="178c1-153">String</span><span class="sxs-lookup"><span data-stu-id="178c1-153">String</span></span>|<span data-ttu-id="178c1-154">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="178c1-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="178c1-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="178c1-155">deviceIMEI</span></span>|<span data-ttu-id="178c1-156">String</span><span class="sxs-lookup"><span data-stu-id="178c1-156">String</span></span>|<span data-ttu-id="178c1-157">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="178c1-157">IMEI of the device.</span></span>|
|<span data-ttu-id="178c1-158">actionState</span><span class="sxs-lookup"><span data-stu-id="178c1-158">actionState</span></span>|[<span data-ttu-id="178c1-159">actionState</span><span class="sxs-lookup"><span data-stu-id="178c1-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="178c1-160">動作状態です。</span><span class="sxs-lookup"><span data-stu-id="178c1-160">Action state.</span></span> <span data-ttu-id="178c1-161">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="178c1-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="178c1-162">応答</span><span class="sxs-lookup"><span data-stu-id="178c1-162">Response</span></span>
<span data-ttu-id="178c1-163">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="178c1-163">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="178c1-164">例</span><span class="sxs-lookup"><span data-stu-id="178c1-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="178c1-165">要求</span><span class="sxs-lookup"><span data-stu-id="178c1-165">Request</span></span>
<span data-ttu-id="178c1-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="178c1-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a><span data-ttu-id="178c1-167">応答</span><span class="sxs-lookup"><span data-stu-id="178c1-167">Response</span></span>
<span data-ttu-id="178c1-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="178c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```




