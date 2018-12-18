---
title: RemoteActionAudit を更新します。
description: RemoteActionAudit オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: a27cd54246aaa1badc9bdbf54379c5d9d2a5a218
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352130"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="bb414-103">RemoteActionAudit を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb414-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="bb414-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bb414-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb414-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb414-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb414-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb414-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb414-107">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb414-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb414-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb414-108">Prerequisites</span></span>
<span data-ttu-id="bb414-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb414-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb414-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb414-111">Permission type</span></span>|<span data-ttu-id="bb414-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb414-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb414-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb414-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb414-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb414-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb414-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb414-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb414-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb414-116">Not supported.</span></span>|
|<span data-ttu-id="bb414-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb414-117">Application</span></span>|<span data-ttu-id="bb414-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb414-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb414-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb414-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="bb414-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb414-120">Request headers</span></span>
|<span data-ttu-id="bb414-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb414-121">Header</span></span>|<span data-ttu-id="bb414-122">値</span><span class="sxs-lookup"><span data-stu-id="bb414-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb414-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb414-123">Authorization</span></span>|<span data-ttu-id="bb414-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bb414-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb414-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb414-125">Accept</span></span>|<span data-ttu-id="bb414-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb414-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb414-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb414-127">Request body</span></span>
<span data-ttu-id="bb414-128">要求の本文に[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb414-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="bb414-129">[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="bb414-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="bb414-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb414-130">Property</span></span>|<span data-ttu-id="bb414-131">種類</span><span class="sxs-lookup"><span data-stu-id="bb414-131">Type</span></span>|<span data-ttu-id="bb414-132">説明</span><span class="sxs-lookup"><span data-stu-id="bb414-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb414-133">ID</span><span class="sxs-lookup"><span data-stu-id="bb414-133">id</span></span>|<span data-ttu-id="bb414-134">String</span><span class="sxs-lookup"><span data-stu-id="bb414-134">String</span></span>|<span data-ttu-id="bb414-135">レポートの id。</span><span class="sxs-lookup"><span data-stu-id="bb414-135">Report Id.</span></span>|
|<span data-ttu-id="bb414-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb414-136">deviceDisplayName</span></span>|<span data-ttu-id="bb414-137">String</span><span class="sxs-lookup"><span data-stu-id="bb414-137">String</span></span>|<span data-ttu-id="bb414-138">Intune デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="bb414-138">Intune device name.</span></span>|
|<span data-ttu-id="bb414-139">userName</span><span class="sxs-lookup"><span data-stu-id="bb414-139">userName</span></span>|<span data-ttu-id="bb414-140">String</span><span class="sxs-lookup"><span data-stu-id="bb414-140">String</span></span>|<span data-ttu-id="bb414-141">\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。</span><span class="sxs-lookup"><span data-stu-id="bb414-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="bb414-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb414-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="bb414-143">String</span><span class="sxs-lookup"><span data-stu-id="bb414-143">String</span></span>|<span data-ttu-id="bb414-144">デバイスのアクションを開始したユーザーは、UPN 形式です。</span><span class="sxs-lookup"><span data-stu-id="bb414-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="bb414-145">action</span><span class="sxs-lookup"><span data-stu-id="bb414-145">action</span></span>|[<span data-ttu-id="bb414-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="bb414-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="bb414-147">アクション名。</span><span class="sxs-lookup"><span data-stu-id="bb414-147">The action name.</span></span> <span data-ttu-id="bb414-148">使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="bb414-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="bb414-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="bb414-149">requestDateTime</span></span>|<span data-ttu-id="bb414-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb414-150">DateTimeOffset</span></span>|<span data-ttu-id="bb414-151">UTC で指定されたアクションを発行した時の時間です。</span><span class="sxs-lookup"><span data-stu-id="bb414-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="bb414-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb414-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="bb414-153">String</span><span class="sxs-lookup"><span data-stu-id="bb414-153">String</span></span>|<span data-ttu-id="bb414-154">デバイス所有者の Upn。</span><span class="sxs-lookup"><span data-stu-id="bb414-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="bb414-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="bb414-155">deviceIMEI</span></span>|<span data-ttu-id="bb414-156">String</span><span class="sxs-lookup"><span data-stu-id="bb414-156">String</span></span>|<span data-ttu-id="bb414-157">デバイスの IMEI。</span><span class="sxs-lookup"><span data-stu-id="bb414-157">IMEI of the device.</span></span>|
|<span data-ttu-id="bb414-158">actionState</span><span class="sxs-lookup"><span data-stu-id="bb414-158">actionState</span></span>|[<span data-ttu-id="bb414-159">actionState</span><span class="sxs-lookup"><span data-stu-id="bb414-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bb414-160">動作状態です。</span><span class="sxs-lookup"><span data-stu-id="bb414-160">Action state.</span></span> <span data-ttu-id="bb414-161">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="bb414-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="bb414-162">応答</span><span class="sxs-lookup"><span data-stu-id="bb414-162">Response</span></span>
<span data-ttu-id="bb414-163">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bb414-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb414-164">例</span><span class="sxs-lookup"><span data-stu-id="bb414-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb414-165">要求</span><span class="sxs-lookup"><span data-stu-id="bb414-165">Request</span></span>
<span data-ttu-id="bb414-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb414-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 399

{
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

### <a name="response"></a><span data-ttu-id="bb414-167">応答</span><span class="sxs-lookup"><span data-stu-id="bb414-167">Response</span></span>
<span data-ttu-id="bb414-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb414-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





