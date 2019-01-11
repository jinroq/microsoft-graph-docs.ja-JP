---
title: Windows10EnrollmentCompletionPageConfiguration を作成します。
description: 新しい windows10EnrollmentCompletionPageConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa459255e48323c5f4e614dc9d12f8ae89d2f4e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862728"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="734ed-103">Windows10EnrollmentCompletionPageConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="734ed-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="734ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="734ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="734ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="734ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="734ed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="734ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="734ed-107">新しい[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="734ed-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="734ed-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="734ed-108">Prerequisites</span></span>
<span data-ttu-id="734ed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="734ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="734ed-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="734ed-111">Permission type</span></span>|<span data-ttu-id="734ed-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="734ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="734ed-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="734ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="734ed-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734ed-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="734ed-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="734ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="734ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="734ed-116">Not supported.</span></span>|
|<span data-ttu-id="734ed-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="734ed-117">Application</span></span>|<span data-ttu-id="734ed-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="734ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="734ed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="734ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="734ed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="734ed-120">Request headers</span></span>
|<span data-ttu-id="734ed-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="734ed-121">Header</span></span>|<span data-ttu-id="734ed-122">値</span><span class="sxs-lookup"><span data-stu-id="734ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="734ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="734ed-123">Authorization</span></span>|<span data-ttu-id="734ed-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="734ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="734ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="734ed-125">Accept</span></span>|<span data-ttu-id="734ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="734ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="734ed-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="734ed-127">Request body</span></span>
<span data-ttu-id="734ed-128">要求の本文に windows10EnrollmentCompletionPageConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="734ed-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="734ed-129">次の表は、windows10EnrollmentCompletionPageConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="734ed-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="734ed-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="734ed-130">Property</span></span>|<span data-ttu-id="734ed-131">種類</span><span class="sxs-lookup"><span data-stu-id="734ed-131">Type</span></span>|<span data-ttu-id="734ed-132">説明</span><span class="sxs-lookup"><span data-stu-id="734ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="734ed-133">ID</span><span class="sxs-lookup"><span data-stu-id="734ed-133">id</span></span>|<span data-ttu-id="734ed-134">String</span><span class="sxs-lookup"><span data-stu-id="734ed-134">String</span></span>|<span data-ttu-id="734ed-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="734ed-136">displayName</span></span>|<span data-ttu-id="734ed-137">String</span><span class="sxs-lookup"><span data-stu-id="734ed-137">String</span></span>|<span data-ttu-id="734ed-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-139">説明</span><span class="sxs-lookup"><span data-stu-id="734ed-139">description</span></span>|<span data-ttu-id="734ed-140">String</span><span class="sxs-lookup"><span data-stu-id="734ed-140">String</span></span>|<span data-ttu-id="734ed-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-142">priority</span><span class="sxs-lookup"><span data-stu-id="734ed-142">priority</span></span>|<span data-ttu-id="734ed-143">Int32</span><span class="sxs-lookup"><span data-stu-id="734ed-143">Int32</span></span>|<span data-ttu-id="734ed-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="734ed-145">createdDateTime</span></span>|<span data-ttu-id="734ed-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="734ed-146">DateTimeOffset</span></span>|<span data-ttu-id="734ed-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="734ed-148">lastModifiedDateTime</span></span>|<span data-ttu-id="734ed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="734ed-149">DateTimeOffset</span></span>|<span data-ttu-id="734ed-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-151">version</span><span class="sxs-lookup"><span data-stu-id="734ed-151">version</span></span>|<span data-ttu-id="734ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="734ed-152">Int32</span></span>|<span data-ttu-id="734ed-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="734ed-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="734ed-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="734ed-154">showInstallationProgress</span></span>|<span data-ttu-id="734ed-155">ブール型</span><span class="sxs-lookup"><span data-stu-id="734ed-155">Boolean</span></span>|<span data-ttu-id="734ed-156">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="734ed-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="734ed-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="734ed-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="734ed-158">ブール型</span><span class="sxs-lookup"><span data-stu-id="734ed-158">Boolean</span></span>|<span data-ttu-id="734ed-159">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="734ed-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="734ed-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="734ed-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="734ed-161">ブール型</span><span class="sxs-lookup"><span data-stu-id="734ed-161">Boolean</span></span>|<span data-ttu-id="734ed-162">許可またはブロック デバイスのインストールの失敗時にリセット</span><span class="sxs-lookup"><span data-stu-id="734ed-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="734ed-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="734ed-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="734ed-164">ブール型</span><span class="sxs-lookup"><span data-stu-id="734ed-164">Boolean</span></span>|<span data-ttu-id="734ed-165">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="734ed-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="734ed-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="734ed-166">customErrorMessage</span></span>|<span data-ttu-id="734ed-167">String</span><span class="sxs-lookup"><span data-stu-id="734ed-167">String</span></span>|<span data-ttu-id="734ed-168">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="734ed-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="734ed-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="734ed-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="734ed-170">Int32</span><span class="sxs-lookup"><span data-stu-id="734ed-170">Int32</span></span>|<span data-ttu-id="734ed-171">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="734ed-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="734ed-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="734ed-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="734ed-173">ブール型</span><span class="sxs-lookup"><span data-stu-id="734ed-173">Boolean</span></span>|<span data-ttu-id="734ed-174">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="734ed-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="734ed-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="734ed-175">selectedMobileAppIds</span></span>|<span data-ttu-id="734ed-176">String コレクション</span><span class="sxs-lookup"><span data-stu-id="734ed-176">String collection</span></span>|<span data-ttu-id="734ed-177">インストールのステータスを追跡するために選択したアプリケーション</span><span class="sxs-lookup"><span data-stu-id="734ed-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="734ed-178">応答</span><span class="sxs-lookup"><span data-stu-id="734ed-178">Response</span></span>
<span data-ttu-id="734ed-179">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="734ed-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="734ed-180">例</span><span class="sxs-lookup"><span data-stu-id="734ed-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="734ed-181">要求</span><span class="sxs-lookup"><span data-stu-id="734ed-181">Request</span></span>
<span data-ttu-id="734ed-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="734ed-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="734ed-183">応答</span><span class="sxs-lookup"><span data-stu-id="734ed-183">Response</span></span>
<span data-ttu-id="734ed-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="734ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





