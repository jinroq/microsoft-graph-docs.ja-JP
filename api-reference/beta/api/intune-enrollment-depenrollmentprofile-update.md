---
title: DepEnrollmentProfile を更新します。
description: DepEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a25f9604f0fd7808cb938dc1720e137db825ab4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983185"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="120df-103">DepEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="120df-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="120df-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="120df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="120df-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="120df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="120df-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="120df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="120df-107">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="120df-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="120df-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="120df-108">Prerequisites</span></span>
<span data-ttu-id="120df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="120df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="120df-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="120df-111">Permission type</span></span>|<span data-ttu-id="120df-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="120df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="120df-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="120df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="120df-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="120df-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="120df-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="120df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="120df-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="120df-116">Not supported.</span></span>|
|<span data-ttu-id="120df-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="120df-117">Application</span></span>|<span data-ttu-id="120df-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="120df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="120df-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="120df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="120df-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="120df-120">Request headers</span></span>
|<span data-ttu-id="120df-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="120df-121">Header</span></span>|<span data-ttu-id="120df-122">値</span><span class="sxs-lookup"><span data-stu-id="120df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="120df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="120df-123">Authorization</span></span>|<span data-ttu-id="120df-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="120df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="120df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="120df-125">Accept</span></span>|<span data-ttu-id="120df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="120df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="120df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="120df-127">Request body</span></span>
<span data-ttu-id="120df-128">要求の本文に[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="120df-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="120df-129">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="120df-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="120df-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="120df-130">Property</span></span>|<span data-ttu-id="120df-131">種類</span><span class="sxs-lookup"><span data-stu-id="120df-131">Type</span></span>|<span data-ttu-id="120df-132">説明</span><span class="sxs-lookup"><span data-stu-id="120df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120df-133">ID</span><span class="sxs-lookup"><span data-stu-id="120df-133">id</span></span>|<span data-ttu-id="120df-134">String</span><span class="sxs-lookup"><span data-stu-id="120df-134">String</span></span>|<span data-ttu-id="120df-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="120df-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-136">displayName</span><span class="sxs-lookup"><span data-stu-id="120df-136">displayName</span></span>|<span data-ttu-id="120df-137">String</span><span class="sxs-lookup"><span data-stu-id="120df-137">String</span></span>|<span data-ttu-id="120df-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="120df-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-139">説明</span><span class="sxs-lookup"><span data-stu-id="120df-139">description</span></span>|<span data-ttu-id="120df-140">String</span><span class="sxs-lookup"><span data-stu-id="120df-140">String</span></span>|<span data-ttu-id="120df-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="120df-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="120df-142">requiresUserAuthentication</span></span>|<span data-ttu-id="120df-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-143">Boolean</span></span>|<span data-ttu-id="120df-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="120df-145">configurationEndpointUrl</span></span>|<span data-ttu-id="120df-146">String</span><span class="sxs-lookup"><span data-stu-id="120df-146">String</span></span>|<span data-ttu-id="120df-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="120df-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="120df-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="120df-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-149">Boolean</span></span>|<span data-ttu-id="120df-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="120df-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="120df-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="120df-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="120df-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="120df-152">isDefault</span></span>|<span data-ttu-id="120df-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-153">Boolean</span></span>|<span data-ttu-id="120df-154">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="120df-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="120df-155">supervisedModeEnabled</span></span>|<span data-ttu-id="120df-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-156">Boolean</span></span>|<span data-ttu-id="120df-157">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="120df-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="120df-158">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="120df-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="120df-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="120df-159">supportDepartment</span></span>|<span data-ttu-id="120df-160">String</span><span class="sxs-lookup"><span data-stu-id="120df-160">String</span></span>|<span data-ttu-id="120df-161">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="120df-161">Support department information</span></span>|
|<span data-ttu-id="120df-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-162">passCodeDisabled</span></span>|<span data-ttu-id="120df-163">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-163">Boolean</span></span>|<span data-ttu-id="120df-164">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="120df-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="120df-165">isMandatory</span></span>|<span data-ttu-id="120df-166">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-166">Boolean</span></span>|<span data-ttu-id="120df-167">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="120df-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="120df-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-168">locationDisabled</span></span>|<span data-ttu-id="120df-169">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-169">Boolean</span></span>|<span data-ttu-id="120df-170">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="120df-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="120df-171">supportPhoneNumber</span></span>|<span data-ttu-id="120df-172">String</span><span class="sxs-lookup"><span data-stu-id="120df-172">String</span></span>|<span data-ttu-id="120df-173">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="120df-173">Support phone number</span></span>|
|<span data-ttu-id="120df-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="120df-174">iTunesPairingMode</span></span>|[<span data-ttu-id="120df-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="120df-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="120df-176">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="120df-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="120df-177">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="120df-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="120df-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-178">profileRemovalDisabled</span></span>|<span data-ttu-id="120df-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-179">Boolean</span></span>|<span data-ttu-id="120df-180">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="120df-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="120df-181">managementCertificates</span></span>|<span data-ttu-id="120df-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="120df-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="120df-183">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="120df-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="120df-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-184">restoreBlocked</span></span>|<span data-ttu-id="120df-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-185">Boolean</span></span>|<span data-ttu-id="120df-186">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="120df-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="120df-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="120df-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-188">Boolean</span></span>|<span data-ttu-id="120df-189">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="120df-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-190">appleIdDisabled</span></span>|<span data-ttu-id="120df-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-191">Boolean</span></span>|<span data-ttu-id="120df-192">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="120df-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="120df-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-194">Boolean</span></span>|<span data-ttu-id="120df-195">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="120df-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-196">touchIdDisabled</span></span>|<span data-ttu-id="120df-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-197">Boolean</span></span>|<span data-ttu-id="120df-198">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="120df-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-199">applePayDisabled</span></span>|<span data-ttu-id="120df-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-200">Boolean</span></span>|<span data-ttu-id="120df-201">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="120df-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-202">zoomDisabled</span></span>|<span data-ttu-id="120df-203">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-203">Boolean</span></span>|<span data-ttu-id="120df-204">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="120df-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-205">siriDisabled</span></span>|<span data-ttu-id="120df-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-206">Boolean</span></span>|<span data-ttu-id="120df-207">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="120df-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-208">diagnosticsDisabled</span></span>|<span data-ttu-id="120df-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-209">Boolean</span></span>|<span data-ttu-id="120df-210">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="120df-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="120df-212">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-212">Boolean</span></span>|<span data-ttu-id="120df-213">Mac OS の登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="120df-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="120df-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="120df-215">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-215">Boolean</span></span>|<span data-ttu-id="120df-216">Mac OS ファイルのボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="120df-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="120df-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="120df-218">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-218">Boolean</span></span>|<span data-ttu-id="120df-219">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="120df-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="120df-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="120df-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="120df-221">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-221">Int32</span></span>|<span data-ttu-id="120df-222">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="120df-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="120df-223">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="120df-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="120df-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="120df-224">enableSharedIPad</span></span>|<span data-ttu-id="120df-225">ブール型</span><span class="sxs-lookup"><span data-stu-id="120df-225">Boolean</span></span>|<span data-ttu-id="120df-226">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="120df-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="120df-227">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="120df-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="120df-228">応答</span><span class="sxs-lookup"><span data-stu-id="120df-228">Response</span></span>
<span data-ttu-id="120df-229">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="120df-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="120df-230">例</span><span class="sxs-lookup"><span data-stu-id="120df-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="120df-231">要求</span><span class="sxs-lookup"><span data-stu-id="120df-231">Request</span></span>
<span data-ttu-id="120df-232">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="120df-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1231

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a><span data-ttu-id="120df-233">応答</span><span class="sxs-lookup"><span data-stu-id="120df-233">Response</span></span>
<span data-ttu-id="120df-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="120df-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```





