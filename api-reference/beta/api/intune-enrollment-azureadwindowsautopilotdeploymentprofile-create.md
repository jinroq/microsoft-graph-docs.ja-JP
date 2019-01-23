---
title: AzureADWindowsAutopilotDeploymentProfile を作成します。
description: 新しい azureADWindowsAutopilotDeploymentProfile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62b73c9041477a5aa103e08ce952c5d713bed83b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398829"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="a70b1-103">AzureADWindowsAutopilotDeploymentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="a70b1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a70b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a70b1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a70b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a70b1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a70b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70b1-107">新しい[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70b1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a70b1-108">Prerequisites</span></span>
<span data-ttu-id="a70b1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a70b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a70b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a70b1-111">Permission type</span></span>|<span data-ttu-id="a70b1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a70b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a70b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a70b1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70b1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a70b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a70b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a70b1-116">Not supported.</span></span>|
|<span data-ttu-id="a70b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a70b1-117">Application</span></span>|<span data-ttu-id="a70b1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a70b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a70b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a70b1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a70b1-120">Request headers</span></span>
|<span data-ttu-id="a70b1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a70b1-121">Header</span></span>|<span data-ttu-id="a70b1-122">値</span><span class="sxs-lookup"><span data-stu-id="a70b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a70b1-123">Authorization</span></span>|<span data-ttu-id="a70b1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a70b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a70b1-125">Accept</span></span>|<span data-ttu-id="a70b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a70b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70b1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a70b1-127">Request body</span></span>
<span data-ttu-id="a70b1-128">要求の本文に azureADWindowsAutopilotDeploymentProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="a70b1-129">次の表は、azureADWindowsAutopilotDeploymentProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="a70b1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a70b1-130">Property</span></span>|<span data-ttu-id="a70b1-131">型</span><span class="sxs-lookup"><span data-stu-id="a70b1-131">Type</span></span>|<span data-ttu-id="a70b1-132">説明</span><span class="sxs-lookup"><span data-stu-id="a70b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70b1-133">id</span><span class="sxs-lookup"><span data-stu-id="a70b1-133">id</span></span>|<span data-ttu-id="a70b1-134">String</span><span class="sxs-lookup"><span data-stu-id="a70b1-134">String</span></span>|<span data-ttu-id="a70b1-135">プロファイル キーは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a70b1-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a70b1-136">displayName</span></span>|<span data-ttu-id="a70b1-137">String</span><span class="sxs-lookup"><span data-stu-id="a70b1-137">String</span></span>|<span data-ttu-id="a70b1-138">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="a70b1-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-139">説明</span><span class="sxs-lookup"><span data-stu-id="a70b1-139">description</span></span>|<span data-ttu-id="a70b1-140">String</span><span class="sxs-lookup"><span data-stu-id="a70b1-140">String</span></span>|<span data-ttu-id="a70b1-141">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="a70b1-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-142">language</span><span class="sxs-lookup"><span data-stu-id="a70b1-142">language</span></span>|<span data-ttu-id="a70b1-143">String</span><span class="sxs-lookup"><span data-stu-id="a70b1-143">String</span></span>|<span data-ttu-id="a70b1-144">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="a70b1-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a70b1-145">createdDateTime</span></span>|<span data-ttu-id="a70b1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70b1-146">DateTimeOffset</span></span>|<span data-ttu-id="a70b1-147">継承されるプロファイル作成時は、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="a70b1-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a70b1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a70b1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70b1-149">DateTimeOffset</span></span>|<span data-ttu-id="a70b1-150">プロファイルは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承の時間を最終更新日</span><span class="sxs-lookup"><span data-stu-id="a70b1-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a70b1-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="a70b1-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a70b1-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="a70b1-153">ボックス発生[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a70b1-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="a70b1-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a70b1-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="a70b1-156">登録ステータス画面が[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="a70b1-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="a70b1-157">extractHardwareHash</span></span>|<span data-ttu-id="a70b1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a70b1-158">Boolean</span></span>|<span data-ttu-id="a70b1-159">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの HardwareHash の抽出</span><span class="sxs-lookup"><span data-stu-id="a70b1-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a70b1-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="a70b1-160">deviceNameTemplate</span></span>|<span data-ttu-id="a70b1-161">String</span><span class="sxs-lookup"><span data-stu-id="a70b1-161">String</span></span>|<span data-ttu-id="a70b1-162">自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。</span><span class="sxs-lookup"><span data-stu-id="a70b1-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="a70b1-163">これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。</span><span class="sxs-lookup"><span data-stu-id="a70b1-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="a70b1-164">テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a70b1-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="a70b1-165">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a70b1-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a70b1-166">応答</span><span class="sxs-lookup"><span data-stu-id="a70b1-166">Response</span></span>
<span data-ttu-id="a70b1-167">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a70b1-167">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70b1-168">例</span><span class="sxs-lookup"><span data-stu-id="a70b1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70b1-169">要求</span><span class="sxs-lookup"><span data-stu-id="a70b1-169">Request</span></span>
<span data-ttu-id="a70b1-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a70b1-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1036

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="a70b1-171">応答</span><span class="sxs-lookup"><span data-stu-id="a70b1-171">Response</span></span>
<span data-ttu-id="a70b1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a70b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1208

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value"
}
```




