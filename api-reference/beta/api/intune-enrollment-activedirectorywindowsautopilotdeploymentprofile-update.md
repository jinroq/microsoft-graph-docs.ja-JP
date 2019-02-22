---
title: activeDirectoryWindowsAutopilotDeploymentProfile の更新
description: activeDirectoryWindowsAutopilotDeploymentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e76fc466195989c82728bf1bba972e876c9ef186
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160061"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="e53d3-103">activeDirectoryWindowsAutopilotDeploymentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="e53d3-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="e53d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e53d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e53d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e53d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e53d3-106">[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e53d3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e53d3-107">Prerequisites</span></span>
<span data-ttu-id="e53d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e53d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e53d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e53d3-110">Permission type</span></span>|<span data-ttu-id="e53d3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e53d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e53d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e53d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e53d3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e53d3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e53d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e53d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e53d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e53d3-115">Not supported.</span></span>|
|<span data-ttu-id="e53d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e53d3-116">Application</span></span>|<span data-ttu-id="e53d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e53d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e53d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e53d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="e53d3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e53d3-119">Request headers</span></span>
|<span data-ttu-id="e53d3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e53d3-120">Header</span></span>|<span data-ttu-id="e53d3-121">値</span><span class="sxs-lookup"><span data-stu-id="e53d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e53d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e53d3-122">Authorization</span></span>|<span data-ttu-id="e53d3-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e53d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e53d3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e53d3-124">Accept</span></span>|<span data-ttu-id="e53d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e53d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e53d3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e53d3-126">Request body</span></span>
<span data-ttu-id="e53d3-127">要求本文で、 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="e53d3-128">次の表に、 [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="e53d3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e53d3-129">Property</span></span>|<span data-ttu-id="e53d3-130">型</span><span class="sxs-lookup"><span data-stu-id="e53d3-130">Type</span></span>|<span data-ttu-id="e53d3-131">説明</span><span class="sxs-lookup"><span data-stu-id="e53d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e53d3-132">id</span><span class="sxs-lookup"><span data-stu-id="e53d3-132">id</span></span>|<span data-ttu-id="e53d3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e53d3-133">String</span></span>|<span data-ttu-id="e53d3-134">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルキー</span><span class="sxs-lookup"><span data-stu-id="e53d3-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e53d3-135">displayName</span></span>|<span data-ttu-id="e53d3-136">String</span><span class="sxs-lookup"><span data-stu-id="e53d3-136">String</span></span>|<span data-ttu-id="e53d3-137">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="e53d3-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-138">説明</span><span class="sxs-lookup"><span data-stu-id="e53d3-138">description</span></span>|<span data-ttu-id="e53d3-139">文字列</span><span class="sxs-lookup"><span data-stu-id="e53d3-139">String</span></span>|<span data-ttu-id="e53d3-140">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="e53d3-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-141">language</span><span class="sxs-lookup"><span data-stu-id="e53d3-141">language</span></span>|<span data-ttu-id="e53d3-142">String</span><span class="sxs-lookup"><span data-stu-id="e53d3-142">String</span></span>|<span data-ttu-id="e53d3-143">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承したデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="e53d3-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e53d3-144">createdDateTime</span></span>|<span data-ttu-id="e53d3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53d3-145">DateTimeOffset</span></span>|<span data-ttu-id="e53d3-146">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="e53d3-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e53d3-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e53d3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53d3-148">DateTimeOffset</span></span>|<span data-ttu-id="e53d3-149">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="e53d3-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e53d3-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="e53d3-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e53d3-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="e53d3-152">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された、すぐに使える状態設定</span><span class="sxs-lookup"><span data-stu-id="e53d3-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e53d3-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="e53d3-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e53d3-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="e53d3-155">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="e53d3-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="e53d3-156">extractHardwareHash</span></span>|<span data-ttu-id="e53d3-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="e53d3-157">Boolean</span></span>|<span data-ttu-id="e53d3-158">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="e53d3-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="e53d3-159">deviceNameTemplate</span></span>|<span data-ttu-id="e53d3-160">String</span><span class="sxs-lookup"><span data-stu-id="e53d3-160">String</span></span>|<span data-ttu-id="e53d3-161">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="e53d3-162">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="e53d3-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="e53d3-163">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="e53d3-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="e53d3-164">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e53d3-165">enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="e53d3-165">enableWhiteGlove</span></span>|<span data-ttu-id="e53d3-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="e53d3-166">Boolean</span></span>|<span data-ttu-id="e53d3-167">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="e53d3-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="e53d3-168">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e53d3-169">応答</span><span class="sxs-lookup"><span data-stu-id="e53d3-169">Response</span></span>
<span data-ttu-id="e53d3-170">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e53d3-170">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e53d3-171">例</span><span class="sxs-lookup"><span data-stu-id="e53d3-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e53d3-172">要求</span><span class="sxs-lookup"><span data-stu-id="e53d3-172">Request</span></span>
<span data-ttu-id="e53d3-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e53d3-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1073

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="e53d3-174">応答</span><span class="sxs-lookup"><span data-stu-id="e53d3-174">Response</span></span>
<span data-ttu-id="e53d3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e53d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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




