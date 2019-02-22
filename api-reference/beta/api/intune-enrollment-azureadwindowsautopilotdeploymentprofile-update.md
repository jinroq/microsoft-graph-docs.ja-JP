---
title: azureADWindowsAutopilotDeploymentProfile の更新
description: azureADWindowsAutopilotDeploymentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1c7d8ca7fec97d687bc359bd9137ef368ce585f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144276"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="912d1-103">azureADWindowsAutopilotDeploymentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="912d1-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="912d1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="912d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="912d1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="912d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="912d1-106">[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="912d1-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="912d1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="912d1-107">Prerequisites</span></span>
<span data-ttu-id="912d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="912d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="912d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="912d1-110">Permission type</span></span>|<span data-ttu-id="912d1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="912d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="912d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="912d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="912d1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912d1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="912d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="912d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="912d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="912d1-115">Not supported.</span></span>|
|<span data-ttu-id="912d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="912d1-116">Application</span></span>|<span data-ttu-id="912d1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="912d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="912d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="912d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="912d1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="912d1-119">Request headers</span></span>
|<span data-ttu-id="912d1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="912d1-120">Header</span></span>|<span data-ttu-id="912d1-121">値</span><span class="sxs-lookup"><span data-stu-id="912d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="912d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="912d1-122">Authorization</span></span>|<span data-ttu-id="912d1-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="912d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="912d1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="912d1-124">Accept</span></span>|<span data-ttu-id="912d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="912d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="912d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="912d1-126">Request body</span></span>
<span data-ttu-id="912d1-127">要求本文で、 [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="912d1-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="912d1-128">次の表に、 [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="912d1-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="912d1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="912d1-129">Property</span></span>|<span data-ttu-id="912d1-130">型</span><span class="sxs-lookup"><span data-stu-id="912d1-130">Type</span></span>|<span data-ttu-id="912d1-131">説明</span><span class="sxs-lookup"><span data-stu-id="912d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912d1-132">id</span><span class="sxs-lookup"><span data-stu-id="912d1-132">id</span></span>|<span data-ttu-id="912d1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="912d1-133">String</span></span>|<span data-ttu-id="912d1-134">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルキー</span><span class="sxs-lookup"><span data-stu-id="912d1-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="912d1-135">displayName</span></span>|<span data-ttu-id="912d1-136">String</span><span class="sxs-lookup"><span data-stu-id="912d1-136">String</span></span>|<span data-ttu-id="912d1-137">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="912d1-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-138">説明</span><span class="sxs-lookup"><span data-stu-id="912d1-138">description</span></span>|<span data-ttu-id="912d1-139">文字列</span><span class="sxs-lookup"><span data-stu-id="912d1-139">String</span></span>|<span data-ttu-id="912d1-140">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="912d1-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-141">language</span><span class="sxs-lookup"><span data-stu-id="912d1-141">language</span></span>|<span data-ttu-id="912d1-142">String</span><span class="sxs-lookup"><span data-stu-id="912d1-142">String</span></span>|<span data-ttu-id="912d1-143">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承したデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="912d1-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="912d1-144">createdDateTime</span></span>|<span data-ttu-id="912d1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912d1-145">DateTimeOffset</span></span>|<span data-ttu-id="912d1-146">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="912d1-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="912d1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="912d1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912d1-148">DateTimeOffset</span></span>|<span data-ttu-id="912d1-149">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="912d1-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="912d1-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="912d1-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="912d1-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="912d1-152">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された、すぐに使える状態設定</span><span class="sxs-lookup"><span data-stu-id="912d1-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="912d1-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="912d1-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="912d1-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="912d1-155">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="912d1-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="912d1-156">extractHardwareHash</span></span>|<span data-ttu-id="912d1-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="912d1-157">Boolean</span></span>|<span data-ttu-id="912d1-158">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="912d1-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="912d1-159">deviceNameTemplate</span></span>|<span data-ttu-id="912d1-160">String</span><span class="sxs-lookup"><span data-stu-id="912d1-160">String</span></span>|<span data-ttu-id="912d1-161">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="912d1-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="912d1-162">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="912d1-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="912d1-163">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="912d1-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="912d1-164">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="912d1-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="912d1-165">enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="912d1-165">enableWhiteGlove</span></span>|<span data-ttu-id="912d1-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="912d1-166">Boolean</span></span>|<span data-ttu-id="912d1-167">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="912d1-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="912d1-168">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="912d1-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="912d1-169">応答</span><span class="sxs-lookup"><span data-stu-id="912d1-169">Response</span></span>
<span data-ttu-id="912d1-170">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="912d1-170">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="912d1-171">例</span><span class="sxs-lookup"><span data-stu-id="912d1-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="912d1-172">要求</span><span class="sxs-lookup"><span data-stu-id="912d1-172">Request</span></span>
<span data-ttu-id="912d1-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="912d1-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1065

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
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="912d1-174">応答</span><span class="sxs-lookup"><span data-stu-id="912d1-174">Response</span></span>
<span data-ttu-id="912d1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="912d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1237

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
  "deviceNameTemplate": "Device Name Template value",
  "enableWhiteGlove": true
}
```




