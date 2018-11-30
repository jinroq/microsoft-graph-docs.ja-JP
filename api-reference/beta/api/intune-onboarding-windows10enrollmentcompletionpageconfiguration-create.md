---
title: Windows10EnrollmentCompletionPageConfiguration を作成します。
description: 新しい windows10EnrollmentCompletionPageConfiguration オブジェクトを作成します。
ms.openlocfilehash: db276cefec8a764b2ad2ddcade93bae7a518f264
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067042"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="59696-103">Windows10EnrollmentCompletionPageConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="59696-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="59696-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59696-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59696-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59696-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59696-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59696-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59696-107">新しい[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="59696-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59696-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="59696-108">Prerequisites</span></span>
<span data-ttu-id="59696-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59696-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59696-111">Permission type</span></span>|<span data-ttu-id="59696-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="59696-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59696-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59696-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59696-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59696-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59696-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59696-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59696-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59696-116">Not supported.</span></span>|
|<span data-ttu-id="59696-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59696-117">Application</span></span>|<span data-ttu-id="59696-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59696-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59696-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59696-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="59696-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59696-120">Request headers</span></span>
|<span data-ttu-id="59696-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59696-121">Header</span></span>|<span data-ttu-id="59696-122">値</span><span class="sxs-lookup"><span data-stu-id="59696-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59696-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59696-123">Authorization</span></span>|<span data-ttu-id="59696-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="59696-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59696-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59696-125">Accept</span></span>|<span data-ttu-id="59696-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59696-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59696-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="59696-127">Request body</span></span>
<span data-ttu-id="59696-128">要求の本文に windows10EnrollmentCompletionPageConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="59696-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="59696-129">次の表は、windows10EnrollmentCompletionPageConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="59696-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="59696-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59696-130">Property</span></span>|<span data-ttu-id="59696-131">型</span><span class="sxs-lookup"><span data-stu-id="59696-131">Type</span></span>|<span data-ttu-id="59696-132">説明</span><span class="sxs-lookup"><span data-stu-id="59696-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59696-133">id</span><span class="sxs-lookup"><span data-stu-id="59696-133">id</span></span>|<span data-ttu-id="59696-134">String</span><span class="sxs-lookup"><span data-stu-id="59696-134">String</span></span>|<span data-ttu-id="59696-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-136">displayName</span><span class="sxs-lookup"><span data-stu-id="59696-136">displayName</span></span>|<span data-ttu-id="59696-137">String</span><span class="sxs-lookup"><span data-stu-id="59696-137">String</span></span>|<span data-ttu-id="59696-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-139">説明</span><span class="sxs-lookup"><span data-stu-id="59696-139">description</span></span>|<span data-ttu-id="59696-140">String</span><span class="sxs-lookup"><span data-stu-id="59696-140">String</span></span>|<span data-ttu-id="59696-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-142">priority</span><span class="sxs-lookup"><span data-stu-id="59696-142">priority</span></span>|<span data-ttu-id="59696-143">Int32</span><span class="sxs-lookup"><span data-stu-id="59696-143">Int32</span></span>|<span data-ttu-id="59696-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59696-145">createdDateTime</span></span>|<span data-ttu-id="59696-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59696-146">DateTimeOffset</span></span>|<span data-ttu-id="59696-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59696-148">lastModifiedDateTime</span></span>|<span data-ttu-id="59696-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59696-149">DateTimeOffset</span></span>|<span data-ttu-id="59696-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-151">version</span><span class="sxs-lookup"><span data-stu-id="59696-151">version</span></span>|<span data-ttu-id="59696-152">Int32</span><span class="sxs-lookup"><span data-stu-id="59696-152">Int32</span></span>|<span data-ttu-id="59696-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="59696-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="59696-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="59696-154">showInstallationProgress</span></span>|<span data-ttu-id="59696-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="59696-155">Boolean</span></span>|<span data-ttu-id="59696-156">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="59696-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="59696-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="59696-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="59696-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="59696-158">Boolean</span></span>|<span data-ttu-id="59696-159">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="59696-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="59696-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="59696-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="59696-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="59696-161">Boolean</span></span>|<span data-ttu-id="59696-162">許可またはブロック デバイスのインストールの失敗時にリセット</span><span class="sxs-lookup"><span data-stu-id="59696-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="59696-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="59696-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="59696-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="59696-164">Boolean</span></span>|<span data-ttu-id="59696-165">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="59696-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="59696-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="59696-166">customErrorMessage</span></span>|<span data-ttu-id="59696-167">String</span><span class="sxs-lookup"><span data-stu-id="59696-167">String</span></span>|<span data-ttu-id="59696-168">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="59696-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="59696-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="59696-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="59696-170">Int32</span><span class="sxs-lookup"><span data-stu-id="59696-170">Int32</span></span>|<span data-ttu-id="59696-171">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="59696-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="59696-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="59696-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="59696-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="59696-173">Boolean</span></span>|<span data-ttu-id="59696-174">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="59696-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="59696-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="59696-175">selectedMobileAppIds</span></span>|<span data-ttu-id="59696-176">String コレクション</span><span class="sxs-lookup"><span data-stu-id="59696-176">String collection</span></span>|<span data-ttu-id="59696-177">インストールのステータスを追跡するために選択したアプリケーション</span><span class="sxs-lookup"><span data-stu-id="59696-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="59696-178">応答</span><span class="sxs-lookup"><span data-stu-id="59696-178">Response</span></span>
<span data-ttu-id="59696-179">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="59696-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59696-180">例</span><span class="sxs-lookup"><span data-stu-id="59696-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="59696-181">要求</span><span class="sxs-lookup"><span data-stu-id="59696-181">Request</span></span>
<span data-ttu-id="59696-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59696-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="59696-183">応答</span><span class="sxs-lookup"><span data-stu-id="59696-183">Response</span></span>
<span data-ttu-id="59696-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="59696-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 755

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```





