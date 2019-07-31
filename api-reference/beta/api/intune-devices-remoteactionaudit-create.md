---
title: RemoteActionAudit の作成
description: 新しい remoteActionAudit オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f4573429db6ccb359feb4b4280483b8d7bbe7c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987076"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="395c3-103">RemoteActionAudit の作成</span><span class="sxs-lookup"><span data-stu-id="395c3-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="395c3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="395c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="395c3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="395c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="395c3-106">新しい[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="395c3-106">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="395c3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="395c3-107">Prerequisites</span></span>
<span data-ttu-id="395c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="395c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="395c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="395c3-110">Permission type</span></span>|<span data-ttu-id="395c3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="395c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="395c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="395c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="395c3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="395c3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="395c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="395c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="395c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="395c3-115">Not supported.</span></span>|
|<span data-ttu-id="395c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="395c3-116">Application</span></span>|<span data-ttu-id="395c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="395c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="395c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="395c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="395c3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="395c3-119">Request headers</span></span>
|<span data-ttu-id="395c3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="395c3-120">Header</span></span>|<span data-ttu-id="395c3-121">値</span><span class="sxs-lookup"><span data-stu-id="395c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="395c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="395c3-122">Authorization</span></span>|<span data-ttu-id="395c3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="395c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="395c3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="395c3-124">Accept</span></span>|<span data-ttu-id="395c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="395c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="395c3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="395c3-126">Request body</span></span>
<span data-ttu-id="395c3-127">要求本文で、remoteActionAudit オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="395c3-127">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="395c3-128">次の表に、remoteActionAudit の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="395c3-128">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="395c3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="395c3-129">Property</span></span>|<span data-ttu-id="395c3-130">型</span><span class="sxs-lookup"><span data-stu-id="395c3-130">Type</span></span>|<span data-ttu-id="395c3-131">説明</span><span class="sxs-lookup"><span data-stu-id="395c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="395c3-132">id</span><span class="sxs-lookup"><span data-stu-id="395c3-132">id</span></span>|<span data-ttu-id="395c3-133">String</span><span class="sxs-lookup"><span data-stu-id="395c3-133">String</span></span>|<span data-ttu-id="395c3-134">レポート Id。</span><span class="sxs-lookup"><span data-stu-id="395c3-134">Report Id.</span></span>|
|<span data-ttu-id="395c3-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="395c3-135">deviceDisplayName</span></span>|<span data-ttu-id="395c3-136">String</span><span class="sxs-lookup"><span data-stu-id="395c3-136">String</span></span>|<span data-ttu-id="395c3-137">Intune デバイス名。</span><span class="sxs-lookup"><span data-stu-id="395c3-137">Intune device name.</span></span>|
|<span data-ttu-id="395c3-138">userName</span><span class="sxs-lookup"><span data-stu-id="395c3-138">userName</span></span>|<span data-ttu-id="395c3-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="395c3-139">String</span></span>|<span data-ttu-id="395c3-140">\[非\]推奨 InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="395c3-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="395c3-141">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="395c3-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="395c3-142">String</span><span class="sxs-lookup"><span data-stu-id="395c3-142">String</span></span>|<span data-ttu-id="395c3-143">デバイスのアクションを開始したユーザーの形式は UPN です。</span><span class="sxs-lookup"><span data-stu-id="395c3-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="395c3-144">action</span><span class="sxs-lookup"><span data-stu-id="395c3-144">action</span></span>|[<span data-ttu-id="395c3-145">remoteAction</span><span class="sxs-lookup"><span data-stu-id="395c3-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="395c3-146">アクション名。</span><span class="sxs-lookup"><span data-stu-id="395c3-146">The action name.</span></span> <span data-ttu-id="395c3-147">可能な値は、`unknown`、`factoryReset`、`removeCompanyData`、`resetPasscode`、`remoteLock`、`enableLostMode`、`disableLostMode`、`locateDevice`、`rebootNow`、`recoverPasscode`、`cleanWindowsDevice`、`logoutSharedAppleDeviceActiveUser`、`quickScan`、`fullScan`、`windowsDefenderUpdateSignatures`、`factoryResetKeepEnrollmentData`、`updateDeviceAccount`、`automaticRedeployment`、`shutDown`、`rotateFileVaultKey`、`getFileVaultKey` です。</span><span class="sxs-lookup"><span data-stu-id="395c3-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateFileVaultKey`, `getFileVaultKey`.</span></span>|
|<span data-ttu-id="395c3-148">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="395c3-148">requestDateTime</span></span>|<span data-ttu-id="395c3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="395c3-149">DateTimeOffset</span></span>|<span data-ttu-id="395c3-150">アクションが発行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="395c3-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="395c3-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="395c3-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="395c3-152">String</span><span class="sxs-lookup"><span data-stu-id="395c3-152">String</span></span>|<span data-ttu-id="395c3-153">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="395c3-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="395c3-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="395c3-154">deviceIMEI</span></span>|<span data-ttu-id="395c3-155">String</span><span class="sxs-lookup"><span data-stu-id="395c3-155">String</span></span>|<span data-ttu-id="395c3-156">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="395c3-156">IMEI of the device.</span></span>|
|<span data-ttu-id="395c3-157">actionState</span><span class="sxs-lookup"><span data-stu-id="395c3-157">actionState</span></span>|[<span data-ttu-id="395c3-158">actionState</span><span class="sxs-lookup"><span data-stu-id="395c3-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="395c3-159">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="395c3-159">Action state.</span></span> <span data-ttu-id="395c3-160">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="395c3-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="395c3-161">応答</span><span class="sxs-lookup"><span data-stu-id="395c3-161">Response</span></span>
<span data-ttu-id="395c3-162">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="395c3-162">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="395c3-163">例</span><span class="sxs-lookup"><span data-stu-id="395c3-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="395c3-164">要求</span><span class="sxs-lookup"><span data-stu-id="395c3-164">Request</span></span>
<span data-ttu-id="395c3-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="395c3-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="395c3-166">応答</span><span class="sxs-lookup"><span data-stu-id="395c3-166">Response</span></span>
<span data-ttu-id="395c3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="395c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





