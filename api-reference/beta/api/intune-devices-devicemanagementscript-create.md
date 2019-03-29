---
title: devicemanagementscript の作成
description: 新しい devicemanagementscript オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a46e5eed8a4b5c678c9510d7471e3b7dc450ccb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959279"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="20e46-103">devicemanagementscript の作成</span><span class="sxs-lookup"><span data-stu-id="20e46-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="20e46-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20e46-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20e46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20e46-106">新しい[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="20e46-106">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20e46-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="20e46-107">Prerequisites</span></span>
<span data-ttu-id="20e46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e46-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20e46-110">Permission type</span></span>|<span data-ttu-id="20e46-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="20e46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20e46-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20e46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20e46-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e46-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20e46-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20e46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20e46-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e46-115">Not supported.</span></span>|
|<span data-ttu-id="20e46-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20e46-116">Application</span></span>|<span data-ttu-id="20e46-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e46-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20e46-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20e46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="20e46-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20e46-119">Request headers</span></span>
|<span data-ttu-id="20e46-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20e46-120">Header</span></span>|<span data-ttu-id="20e46-121">値</span><span class="sxs-lookup"><span data-stu-id="20e46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20e46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20e46-122">Authorization</span></span>|<span data-ttu-id="20e46-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="20e46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20e46-124">承諾</span><span class="sxs-lookup"><span data-stu-id="20e46-124">Accept</span></span>|<span data-ttu-id="20e46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20e46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20e46-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="20e46-126">Request body</span></span>
<span data-ttu-id="20e46-127">要求本文で、devicemanagementscript オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="20e46-127">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="20e46-128">次の表に、devicemanagementscript の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="20e46-128">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="20e46-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20e46-129">Property</span></span>|<span data-ttu-id="20e46-130">型</span><span class="sxs-lookup"><span data-stu-id="20e46-130">Type</span></span>|<span data-ttu-id="20e46-131">説明</span><span class="sxs-lookup"><span data-stu-id="20e46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20e46-132">id</span><span class="sxs-lookup"><span data-stu-id="20e46-132">id</span></span>|<span data-ttu-id="20e46-133">String</span><span class="sxs-lookup"><span data-stu-id="20e46-133">String</span></span>|<span data-ttu-id="20e46-134">デバイス管理スクリプトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="20e46-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="20e46-135">displayName</span><span class="sxs-lookup"><span data-stu-id="20e46-135">displayName</span></span>|<span data-ttu-id="20e46-136">String</span><span class="sxs-lookup"><span data-stu-id="20e46-136">String</span></span>|<span data-ttu-id="20e46-137">デバイス管理スクリプトの名前。</span><span class="sxs-lookup"><span data-stu-id="20e46-137">Name of the device management script.</span></span>|
|<span data-ttu-id="20e46-138">description</span><span class="sxs-lookup"><span data-stu-id="20e46-138">description</span></span>|<span data-ttu-id="20e46-139">String</span><span class="sxs-lookup"><span data-stu-id="20e46-139">String</span></span>|<span data-ttu-id="20e46-140">デバイス管理スクリプトの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="20e46-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="20e46-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="20e46-141">runSchedule</span></span>|[<span data-ttu-id="20e46-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="20e46-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="20e46-143">スクリプトを実行する間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="20e46-143">The interval for script to run.</span></span> <span data-ttu-id="20e46-144">定義されていない場合、スクリプトは1回だけ実行されます。</span><span class="sxs-lookup"><span data-stu-id="20e46-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="20e46-145">scriptcontent</span><span class="sxs-lookup"><span data-stu-id="20e46-145">scriptContent</span></span>|<span data-ttu-id="20e46-146">Binary</span><span class="sxs-lookup"><span data-stu-id="20e46-146">Binary</span></span>|<span data-ttu-id="20e46-147">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="20e46-147">The script content.</span></span>|
|<span data-ttu-id="20e46-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20e46-148">createdDateTime</span></span>|<span data-ttu-id="20e46-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20e46-149">DateTimeOffset</span></span>|<span data-ttu-id="20e46-150">デバイス管理スクリプトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="20e46-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="20e46-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20e46-151">lastModifiedDateTime</span></span>|<span data-ttu-id="20e46-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20e46-152">DateTimeOffset</span></span>|<span data-ttu-id="20e46-153">デバイス管理スクリプトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="20e46-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="20e46-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="20e46-154">runAsAccount</span></span>|[<span data-ttu-id="20e46-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="20e46-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="20e46-156">実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="20e46-156">Indicates the type of execution context.</span></span> <span data-ttu-id="20e46-157">可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="20e46-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="20e46-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="20e46-158">enforceSignatureCheck</span></span>|<span data-ttu-id="20e46-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="20e46-159">Boolean</span></span>|<span data-ttu-id="20e46-160">スクリプト署名をチェックする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="20e46-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="20e46-161">fileName</span><span class="sxs-lookup"><span data-stu-id="20e46-161">fileName</span></span>|<span data-ttu-id="20e46-162">String</span><span class="sxs-lookup"><span data-stu-id="20e46-162">String</span></span>|<span data-ttu-id="20e46-163">スクリプトファイル名。</span><span class="sxs-lookup"><span data-stu-id="20e46-163">Script file name.</span></span>|
|<span data-ttu-id="20e46-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20e46-164">roleScopeTagIds</span></span>|<span data-ttu-id="20e46-165">String collection</span><span class="sxs-lookup"><span data-stu-id="20e46-165">String collection</span></span>|<span data-ttu-id="20e46-166">この powershellscript インスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="20e46-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="20e46-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="20e46-167">runAs32Bit</span></span>|<span data-ttu-id="20e46-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="20e46-168">Boolean</span></span>|<span data-ttu-id="20e46-169">PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="20e46-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="20e46-170">応答</span><span class="sxs-lookup"><span data-stu-id="20e46-170">Response</span></span>
<span data-ttu-id="20e46-171">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20e46-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e46-172">例</span><span class="sxs-lookup"><span data-stu-id="20e46-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="20e46-173">要求</span><span class="sxs-lookup"><span data-stu-id="20e46-173">Request</span></span>
<span data-ttu-id="20e46-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20e46-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="20e46-175">応答</span><span class="sxs-lookup"><span data-stu-id="20e46-175">Response</span></span>
<span data-ttu-id="20e46-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20e46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
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
  "runAs32Bit": true
}
```




