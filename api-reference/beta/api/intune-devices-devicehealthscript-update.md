---
title: DeviceHealthScript の更新
description: DeviceHealthScript オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd5d44e45639ed59518cc4af413b8db76a6c6430
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311709"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="2d917-103">DeviceHealthScript の更新</span><span class="sxs-lookup"><span data-stu-id="2d917-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="2d917-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d917-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d917-106">[DeviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d917-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d917-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d917-107">Prerequisites</span></span>
<span data-ttu-id="2d917-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d917-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d917-110">Permission type</span></span>|<span data-ttu-id="2d917-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d917-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d917-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d917-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d917-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d917-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2d917-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d917-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d917-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d917-115">Not supported.</span></span>|
|<span data-ttu-id="2d917-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d917-116">Application</span></span>|<span data-ttu-id="2d917-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d917-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d917-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d917-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="2d917-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d917-119">Request headers</span></span>
|<span data-ttu-id="2d917-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d917-120">Header</span></span>|<span data-ttu-id="2d917-121">値</span><span class="sxs-lookup"><span data-stu-id="2d917-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d917-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d917-122">Authorization</span></span>|<span data-ttu-id="2d917-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d917-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d917-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2d917-124">Accept</span></span>|<span data-ttu-id="2d917-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d917-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d917-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d917-126">Request body</span></span>
<span data-ttu-id="2d917-127">要求本文で、 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d917-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="2d917-128">次の表に、 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d917-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="2d917-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d917-129">Property</span></span>|<span data-ttu-id="2d917-130">型</span><span class="sxs-lookup"><span data-stu-id="2d917-130">Type</span></span>|<span data-ttu-id="2d917-131">説明</span><span class="sxs-lookup"><span data-stu-id="2d917-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d917-132">id</span><span class="sxs-lookup"><span data-stu-id="2d917-132">id</span></span>|<span data-ttu-id="2d917-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2d917-133">String</span></span>|<span data-ttu-id="2d917-134">デバイス管理スクリプトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2d917-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="2d917-135">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-135">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2d917-136">displayName</span></span>|<span data-ttu-id="2d917-137">String</span><span class="sxs-lookup"><span data-stu-id="2d917-137">String</span></span>|<span data-ttu-id="2d917-138">デバイス管理スクリプトの名前。</span><span class="sxs-lookup"><span data-stu-id="2d917-138">Name of the device management script.</span></span> <span data-ttu-id="2d917-139">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-139">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-140">description</span><span class="sxs-lookup"><span data-stu-id="2d917-140">description</span></span>|<span data-ttu-id="2d917-141">String</span><span class="sxs-lookup"><span data-stu-id="2d917-141">String</span></span>|<span data-ttu-id="2d917-142">デバイス管理スクリプトの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="2d917-142">Optional description for the device management script.</span></span> <span data-ttu-id="2d917-143">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-143">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2d917-144">runSchedule</span></span>|[<span data-ttu-id="2d917-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2d917-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="2d917-146">スクリプトを実行する間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d917-146">The interval for script to run.</span></span> <span data-ttu-id="2d917-147">定義されていない場合、スクリプトは[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承された後に実行されます</span><span class="sxs-lookup"><span data-stu-id="2d917-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2d917-148">scriptContent</span></span>|<span data-ttu-id="2d917-149">Binary</span><span class="sxs-lookup"><span data-stu-id="2d917-149">Binary</span></span>|<span data-ttu-id="2d917-150">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="2d917-150">The script content.</span></span> <span data-ttu-id="2d917-151">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-151">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d917-152">createdDateTime</span></span>|<span data-ttu-id="2d917-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d917-153">DateTimeOffset</span></span>|<span data-ttu-id="2d917-154">デバイス管理スクリプトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="2d917-154">The date and time the device management script was created.</span></span> <span data-ttu-id="2d917-155">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-155">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d917-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2d917-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d917-157">DateTimeOffset</span></span>|<span data-ttu-id="2d917-158">デバイス管理スクリプトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="2d917-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2d917-159">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-159">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2d917-160">runAsAccount</span></span>|[<span data-ttu-id="2d917-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="2d917-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2d917-162">実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="2d917-162">Indicates the type of execution context.</span></span> <span data-ttu-id="2d917-163">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2d917-163">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span> <span data-ttu-id="2d917-164">可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="2d917-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2d917-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="2d917-165">enforceSignatureCheck</span></span>|<span data-ttu-id="2d917-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d917-166">Boolean</span></span>|<span data-ttu-id="2d917-167">スクリプト署名をチェックする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2d917-167">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="2d917-168">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-168">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-169">fileName</span><span class="sxs-lookup"><span data-stu-id="2d917-169">fileName</span></span>|<span data-ttu-id="2d917-170">String</span><span class="sxs-lookup"><span data-stu-id="2d917-170">String</span></span>|<span data-ttu-id="2d917-171">スクリプトファイル名。</span><span class="sxs-lookup"><span data-stu-id="2d917-171">Script file name.</span></span> <span data-ttu-id="2d917-172">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-172">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d917-173">roleScopeTagIds</span></span>|<span data-ttu-id="2d917-174">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2d917-174">String collection</span></span>|<span data-ttu-id="2d917-175">この PowerShellScript インスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="2d917-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="2d917-176">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2d917-176">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="2d917-177">runAs32Bit</span></span>|<span data-ttu-id="2d917-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d917-178">Boolean</span></span>|<span data-ttu-id="2d917-179">PowerShell スクリプトを[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承した32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="2d917-179">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="2d917-180">complianceRule</span><span class="sxs-lookup"><span data-stu-id="2d917-180">complianceRule</span></span>|[<span data-ttu-id="2d917-181">deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="2d917-181">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="2d917-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2d917-182">Not yet documented</span></span>|
|<span data-ttu-id="2d917-183">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="2d917-183">remediationScriptContent</span></span>|<span data-ttu-id="2d917-184">Binary</span><span class="sxs-lookup"><span data-stu-id="2d917-184">Binary</span></span>|<span data-ttu-id="2d917-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2d917-185">Not yet documented</span></span>|
|<span data-ttu-id="2d917-186">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="2d917-186">runRemediationScript</span></span>|<span data-ttu-id="2d917-187">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2d917-187">Boolean</span></span>|<span data-ttu-id="2d917-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2d917-188">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2d917-189">応答</span><span class="sxs-lookup"><span data-stu-id="2d917-189">Response</span></span>
<span data-ttu-id="2d917-190">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d917-190">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d917-191">例</span><span class="sxs-lookup"><span data-stu-id="2d917-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d917-192">要求</span><span class="sxs-lookup"><span data-stu-id="2d917-192">Request</span></span>
<span data-ttu-id="2d917-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d917-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a><span data-ttu-id="2d917-194">応答</span><span class="sxs-lookup"><span data-stu-id="2d917-194">Response</span></span>
<span data-ttu-id="2d917-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d917-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






