---
title: DeviceManagementScript を作成します。
description: 新しい deviceManagementScript オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be0ffb8b912b25684ba0ed3dc383a995fb872f3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409273"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="aec08-103">DeviceManagementScript を作成します。</span><span class="sxs-lookup"><span data-stu-id="aec08-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="aec08-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aec08-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aec08-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aec08-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aec08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec08-107">新しい[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aec08-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aec08-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="aec08-108">Prerequisites</span></span>
<span data-ttu-id="aec08-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aec08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aec08-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aec08-111">Permission type</span></span>|<span data-ttu-id="aec08-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aec08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec08-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aec08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aec08-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec08-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aec08-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aec08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec08-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec08-116">Not supported.</span></span>|
|<span data-ttu-id="aec08-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aec08-117">Application</span></span>|<span data-ttu-id="aec08-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aec08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aec08-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aec08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="aec08-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aec08-120">Request headers</span></span>
|<span data-ttu-id="aec08-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aec08-121">Header</span></span>|<span data-ttu-id="aec08-122">値</span><span class="sxs-lookup"><span data-stu-id="aec08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aec08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aec08-123">Authorization</span></span>|<span data-ttu-id="aec08-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aec08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aec08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aec08-125">Accept</span></span>|<span data-ttu-id="aec08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aec08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec08-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aec08-127">Request body</span></span>
<span data-ttu-id="aec08-128">要求の本文に deviceManagementScript オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="aec08-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="aec08-129">次の表は、deviceManagementScript を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aec08-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="aec08-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aec08-130">Property</span></span>|<span data-ttu-id="aec08-131">型</span><span class="sxs-lookup"><span data-stu-id="aec08-131">Type</span></span>|<span data-ttu-id="aec08-132">説明</span><span class="sxs-lookup"><span data-stu-id="aec08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec08-133">id</span><span class="sxs-lookup"><span data-stu-id="aec08-133">id</span></span>|<span data-ttu-id="aec08-134">String</span><span class="sxs-lookup"><span data-stu-id="aec08-134">String</span></span>|<span data-ttu-id="aec08-135">デバイス管理スクリプト用の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="aec08-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="aec08-136">displayName</span><span class="sxs-lookup"><span data-stu-id="aec08-136">displayName</span></span>|<span data-ttu-id="aec08-137">String</span><span class="sxs-lookup"><span data-stu-id="aec08-137">String</span></span>|<span data-ttu-id="aec08-138">デバイスの管理スクリプトの名前です。</span><span class="sxs-lookup"><span data-stu-id="aec08-138">Name of the device management script.</span></span>|
|<span data-ttu-id="aec08-139">説明</span><span class="sxs-lookup"><span data-stu-id="aec08-139">description</span></span>|<span data-ttu-id="aec08-140">String</span><span class="sxs-lookup"><span data-stu-id="aec08-140">String</span></span>|<span data-ttu-id="aec08-141">デバイスの管理スクリプトのオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="aec08-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="aec08-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="aec08-142">runSchedule</span></span>|[<span data-ttu-id="aec08-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="aec08-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="aec08-144">スクリプトを実行する間隔です。</span><span class="sxs-lookup"><span data-stu-id="aec08-144">The interval for script to run.</span></span> <span data-ttu-id="aec08-145">定義されていないスクリプトは実行 1 回</span><span class="sxs-lookup"><span data-stu-id="aec08-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="aec08-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="aec08-146">scriptContent</span></span>|<span data-ttu-id="aec08-147">Binary</span><span class="sxs-lookup"><span data-stu-id="aec08-147">Binary</span></span>|<span data-ttu-id="aec08-148">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="aec08-148">The script content.</span></span>|
|<span data-ttu-id="aec08-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aec08-149">createdDateTime</span></span>|<span data-ttu-id="aec08-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec08-150">DateTimeOffset</span></span>|<span data-ttu-id="aec08-151">デバイス管理スクリプトが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="aec08-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="aec08-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aec08-152">lastModifiedDateTime</span></span>|<span data-ttu-id="aec08-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec08-153">DateTimeOffset</span></span>|<span data-ttu-id="aec08-154">日付と時刻、デバイス管理のスクリプトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="aec08-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="aec08-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="aec08-155">runAsAccount</span></span>|[<span data-ttu-id="aec08-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="aec08-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="aec08-157">デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="aec08-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="aec08-158">使用可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="aec08-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="aec08-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="aec08-159">enforceSignatureCheck</span></span>|<span data-ttu-id="aec08-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec08-160">Boolean</span></span>|<span data-ttu-id="aec08-161">スクリプト署名をチェックする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aec08-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="aec08-162">fileName</span><span class="sxs-lookup"><span data-stu-id="aec08-162">fileName</span></span>|<span data-ttu-id="aec08-163">String</span><span class="sxs-lookup"><span data-stu-id="aec08-163">String</span></span>|<span data-ttu-id="aec08-164">スクリプト ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="aec08-164">Script file name.</span></span>|
|<span data-ttu-id="aec08-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aec08-165">roleScopeTagIds</span></span>|<span data-ttu-id="aec08-166">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aec08-166">String collection</span></span>|<span data-ttu-id="aec08-167">この PowerShellScript インスタンスのスコープのタグ Id のリストです。</span><span class="sxs-lookup"><span data-stu-id="aec08-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="aec08-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="aec08-168">runAs32Bit</span></span>|<span data-ttu-id="aec08-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec08-169">Boolean</span></span>|<span data-ttu-id="aec08-170">PowerShell スクリプトが 32 ビットとして実行する必要があるかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="aec08-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="aec08-171">応答</span><span class="sxs-lookup"><span data-stu-id="aec08-171">Response</span></span>
<span data-ttu-id="aec08-172">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="aec08-172">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec08-173">例</span><span class="sxs-lookup"><span data-stu-id="aec08-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="aec08-174">要求</span><span class="sxs-lookup"><span data-stu-id="aec08-174">Request</span></span>
<span data-ttu-id="aec08-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aec08-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aec08-176">応答</span><span class="sxs-lookup"><span data-stu-id="aec08-176">Response</span></span>
<span data-ttu-id="aec08-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aec08-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




