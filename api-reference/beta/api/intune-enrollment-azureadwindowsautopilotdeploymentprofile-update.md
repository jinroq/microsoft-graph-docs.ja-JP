---
title: AzureADWindowsAutopilotDeploymentProfile を更新します。
description: AzureADWindowsAutopilotDeploymentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aa4e5674db7656961c75e7f095b1734505bc1aef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941241"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="2e3f2-103">AzureADWindowsAutopilotDeploymentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="2e3f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e3f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e3f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e3f2-107">[AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-107">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e3f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2e3f2-108">Prerequisites</span></span>
<span data-ttu-id="2e3f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e3f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e3f2-111">Permission type</span></span>|<span data-ttu-id="2e3f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e3f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e3f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e3f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e3f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e3f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e3f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e3f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-116">Not supported.</span></span>|
|<span data-ttu-id="2e3f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e3f2-117">Application</span></span>|<span data-ttu-id="2e3f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e3f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e3f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="2e3f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e3f2-120">Request headers</span></span>
|<span data-ttu-id="2e3f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e3f2-121">Header</span></span>|<span data-ttu-id="2e3f2-122">値</span><span class="sxs-lookup"><span data-stu-id="2e3f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e3f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e3f2-123">Authorization</span></span>|<span data-ttu-id="2e3f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e3f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e3f2-125">Accept</span></span>|<span data-ttu-id="2e3f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e3f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e3f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e3f2-127">Request body</span></span>
<span data-ttu-id="2e3f2-128">要求の本文に[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-128">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="2e3f2-129">[AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-129">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="2e3f2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e3f2-130">Property</span></span>|<span data-ttu-id="2e3f2-131">型</span><span class="sxs-lookup"><span data-stu-id="2e3f2-131">Type</span></span>|<span data-ttu-id="2e3f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="2e3f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3f2-133">ID</span><span class="sxs-lookup"><span data-stu-id="2e3f2-133">id</span></span>|<span data-ttu-id="2e3f2-134">String</span><span class="sxs-lookup"><span data-stu-id="2e3f2-134">String</span></span>|<span data-ttu-id="2e3f2-135">プロファイル キーは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e3f2-136">displayName</span></span>|<span data-ttu-id="2e3f2-137">String</span><span class="sxs-lookup"><span data-stu-id="2e3f2-137">String</span></span>|<span data-ttu-id="2e3f2-138">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="2e3f2-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-139">説明</span><span class="sxs-lookup"><span data-stu-id="2e3f2-139">description</span></span>|<span data-ttu-id="2e3f2-140">String</span><span class="sxs-lookup"><span data-stu-id="2e3f2-140">String</span></span>|<span data-ttu-id="2e3f2-141">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="2e3f2-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-142">language</span><span class="sxs-lookup"><span data-stu-id="2e3f2-142">language</span></span>|<span data-ttu-id="2e3f2-143">String</span><span class="sxs-lookup"><span data-stu-id="2e3f2-143">String</span></span>|<span data-ttu-id="2e3f2-144">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="2e3f2-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3f2-145">createdDateTime</span></span>|<span data-ttu-id="2e3f2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3f2-146">DateTimeOffset</span></span>|<span data-ttu-id="2e3f2-147">継承されるプロファイル作成時は、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="2e3f2-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3f2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2e3f2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3f2-149">DateTimeOffset</span></span>|<span data-ttu-id="2e3f2-150">プロファイルは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承の時間を最終更新日</span><span class="sxs-lookup"><span data-stu-id="2e3f2-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2e3f2-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="2e3f2-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2e3f2-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="2e3f2-153">ボックス発生[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2e3f2-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="2e3f2-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2e3f2-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="2e3f2-156">登録ステータス画面が[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="2e3f2-157">extractHardwareHash</span></span>|<span data-ttu-id="2e3f2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e3f2-158">Boolean</span></span>|<span data-ttu-id="2e3f2-159">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの HardwareHash の抽出</span><span class="sxs-lookup"><span data-stu-id="2e3f2-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2e3f2-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="2e3f2-160">deviceNameTemplate</span></span>|<span data-ttu-id="2e3f2-161">String</span><span class="sxs-lookup"><span data-stu-id="2e3f2-161">String</span></span>|<span data-ttu-id="2e3f2-162">自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="2e3f2-163">これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="2e3f2-164">テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="2e3f2-165">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2e3f2-166">応答</span><span class="sxs-lookup"><span data-stu-id="2e3f2-166">Response</span></span>
<span data-ttu-id="2e3f2-167">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-167">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e3f2-168">例</span><span class="sxs-lookup"><span data-stu-id="2e3f2-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e3f2-169">要求</span><span class="sxs-lookup"><span data-stu-id="2e3f2-169">Request</span></span>
<span data-ttu-id="2e3f2-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1021

{
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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

### <a name="response"></a><span data-ttu-id="2e3f2-171">応答</span><span class="sxs-lookup"><span data-stu-id="2e3f2-171">Response</span></span>
<span data-ttu-id="2e3f2-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2e3f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





