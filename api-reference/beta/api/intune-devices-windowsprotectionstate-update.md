---
title: WindowsProtectionState の更新
description: WindowsProtectionState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fbdfd6ad0ca934b97fd5410b35d2806a8fa067
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908960"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="a484f-103">WindowsProtectionState の更新</span><span class="sxs-lookup"><span data-stu-id="a484f-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="a484f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a484f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a484f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a484f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a484f-106">[Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a484f-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a484f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a484f-107">Prerequisites</span></span>
<span data-ttu-id="a484f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a484f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a484f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a484f-110">Permission type</span></span>|<span data-ttu-id="a484f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a484f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a484f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a484f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a484f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a484f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a484f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a484f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a484f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a484f-115">Not supported.</span></span>|
|<span data-ttu-id="a484f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a484f-116">Application</span></span>|<span data-ttu-id="a484f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a484f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a484f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a484f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="a484f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a484f-119">Request headers</span></span>
|<span data-ttu-id="a484f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a484f-120">Header</span></span>|<span data-ttu-id="a484f-121">値</span><span class="sxs-lookup"><span data-stu-id="a484f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a484f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a484f-122">Authorization</span></span>|<span data-ttu-id="a484f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a484f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a484f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a484f-124">Accept</span></span>|<span data-ttu-id="a484f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a484f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a484f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a484f-126">Request body</span></span>
<span data-ttu-id="a484f-127">要求本文で、 [Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a484f-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="a484f-128">次の表に、 [Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a484f-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="a484f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a484f-129">Property</span></span>|<span data-ttu-id="a484f-130">型</span><span class="sxs-lookup"><span data-stu-id="a484f-130">Type</span></span>|<span data-ttu-id="a484f-131">説明</span><span class="sxs-lookup"><span data-stu-id="a484f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a484f-132">id</span><span class="sxs-lookup"><span data-stu-id="a484f-132">id</span></span>|<span data-ttu-id="a484f-133">String</span><span class="sxs-lookup"><span data-stu-id="a484f-133">String</span></span>|<span data-ttu-id="a484f-134">デバイス保護状態オブジェクトの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a484f-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a484f-135">これはデバイスのデバイス id です</span><span class="sxs-lookup"><span data-stu-id="a484f-135">This is device id of the device</span></span>|
|<span data-ttu-id="a484f-136">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a484f-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="a484f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-137">Boolean</span></span>|<span data-ttu-id="a484f-138">マルウェア対策が有効になっているか、または使用できない</span><span class="sxs-lookup"><span data-stu-id="a484f-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a484f-139">deviceState</span><span class="sxs-lookup"><span data-stu-id="a484f-139">deviceState</span></span>|[<span data-ttu-id="a484f-140">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a484f-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a484f-141">コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。</span><span class="sxs-lookup"><span data-stu-id="a484f-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a484f-142">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="a484f-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a484f-143">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a484f-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a484f-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-144">Boolean</span></span>|<span data-ttu-id="a484f-145">リアルタイム保護が有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="a484f-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a484f-146">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a484f-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a484f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-147">Boolean</span></span>|<span data-ttu-id="a484f-148">ネットワーク検査システムが有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="a484f-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a484f-149">quickScanOverdue 超過</span><span class="sxs-lookup"><span data-stu-id="a484f-149">quickScanOverdue</span></span>|<span data-ttu-id="a484f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-150">Boolean</span></span>|<span data-ttu-id="a484f-151">クイックスキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="a484f-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a484f-152">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a484f-152">fullScanOverdue</span></span>|<span data-ttu-id="a484f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-153">Boolean</span></span>|<span data-ttu-id="a484f-154">完全スキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="a484f-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a484f-155">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a484f-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="a484f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-156">Boolean</span></span>|<span data-ttu-id="a484f-157">署名が古くなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="a484f-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="a484f-158">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a484f-158">rebootRequired</span></span>|<span data-ttu-id="a484f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-159">Boolean</span></span>|<span data-ttu-id="a484f-160">再起動が必要かどうか</span><span class="sxs-lookup"><span data-stu-id="a484f-160">Reboot required or not?</span></span>|
|<span data-ttu-id="a484f-161">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a484f-161">fullScanRequired</span></span>|<span data-ttu-id="a484f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a484f-162">Boolean</span></span>|<span data-ttu-id="a484f-163">フルスキャンが必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="a484f-163">Full scan required or not?</span></span>|
|<span data-ttu-id="a484f-164">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a484f-164">engineVersion</span></span>|<span data-ttu-id="a484f-165">String</span><span class="sxs-lookup"><span data-stu-id="a484f-165">String</span></span>|<span data-ttu-id="a484f-166">現在のエンドポイント保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="a484f-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a484f-167">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a484f-167">signatureVersion</span></span>|<span data-ttu-id="a484f-168">String</span><span class="sxs-lookup"><span data-stu-id="a484f-168">String</span></span>|<span data-ttu-id="a484f-169">現在のマルウェア定義バージョン</span><span class="sxs-lookup"><span data-stu-id="a484f-169">Current malware definitions version</span></span>|
|<span data-ttu-id="a484f-170">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a484f-170">antiMalwareVersion</span></span>|<span data-ttu-id="a484f-171">String</span><span class="sxs-lookup"><span data-stu-id="a484f-171">String</span></span>|<span data-ttu-id="a484f-172">現在のマルウェア対策バージョン</span><span class="sxs-lookup"><span data-stu-id="a484f-172">Current anti malware version</span></span>|
|<span data-ttu-id="a484f-173">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a484f-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="a484f-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a484f-174">DateTimeOffset</span></span>|<span data-ttu-id="a484f-175">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="a484f-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="a484f-176">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a484f-176">lastFullScanDateTime</span></span>|<span data-ttu-id="a484f-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a484f-177">DateTimeOffset</span></span>|<span data-ttu-id="a484f-178">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="a484f-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="a484f-179">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a484f-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a484f-180">String</span><span class="sxs-lookup"><span data-stu-id="a484f-180">String</span></span>|<span data-ttu-id="a484f-181">最終クイックスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="a484f-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="a484f-182">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a484f-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a484f-183">String</span><span class="sxs-lookup"><span data-stu-id="a484f-183">String</span></span>|<span data-ttu-id="a484f-184">前回のフルスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="a484f-184">Last full scan signature version</span></span>|
|<span data-ttu-id="a484f-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a484f-185">lastReportedDateTime</span></span>|<span data-ttu-id="a484f-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a484f-186">DateTimeOffset</span></span>|<span data-ttu-id="a484f-187">前回のデバイス正常性の状態が報告された時刻</span><span class="sxs-lookup"><span data-stu-id="a484f-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="a484f-188">応答</span><span class="sxs-lookup"><span data-stu-id="a484f-188">Response</span></span>
<span data-ttu-id="a484f-189">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a484f-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a484f-190">例</span><span class="sxs-lookup"><span data-stu-id="a484f-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="a484f-191">要求</span><span class="sxs-lookup"><span data-stu-id="a484f-191">Request</span></span>
<span data-ttu-id="a484f-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a484f-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a484f-193">応答</span><span class="sxs-lookup"><span data-stu-id="a484f-193">Response</span></span>
<span data-ttu-id="a484f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a484f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




