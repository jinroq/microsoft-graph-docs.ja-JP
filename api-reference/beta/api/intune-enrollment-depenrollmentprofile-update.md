---
title: DepEnrollmentProfile を更新します。
description: DepEnrollmentProfile オブジェクトのプロパティを更新します。
ms.openlocfilehash: 1026abe11bec1a766b7fda2907612d77af077bd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071890"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="62613-103">DepEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="62613-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="62613-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="62613-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62613-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62613-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62613-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="62613-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62613-107">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62613-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62613-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="62613-108">Prerequisites</span></span>
<span data-ttu-id="62613-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62613-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62613-111">Permission type</span></span>|<span data-ttu-id="62613-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62613-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62613-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62613-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62613-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62613-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="62613-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62613-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62613-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62613-116">Not supported.</span></span>|
|<span data-ttu-id="62613-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62613-117">Application</span></span>|<span data-ttu-id="62613-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62613-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62613-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62613-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="62613-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62613-120">Request headers</span></span>
|<span data-ttu-id="62613-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62613-121">Header</span></span>|<span data-ttu-id="62613-122">値</span><span class="sxs-lookup"><span data-stu-id="62613-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62613-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62613-123">Authorization</span></span>|<span data-ttu-id="62613-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="62613-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62613-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62613-125">Accept</span></span>|<span data-ttu-id="62613-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62613-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62613-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="62613-127">Request body</span></span>
<span data-ttu-id="62613-128">要求の本文に[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="62613-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="62613-129">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="62613-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="62613-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62613-130">Property</span></span>|<span data-ttu-id="62613-131">型</span><span class="sxs-lookup"><span data-stu-id="62613-131">Type</span></span>|<span data-ttu-id="62613-132">説明</span><span class="sxs-lookup"><span data-stu-id="62613-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62613-133">id</span><span class="sxs-lookup"><span data-stu-id="62613-133">id</span></span>|<span data-ttu-id="62613-134">String</span><span class="sxs-lookup"><span data-stu-id="62613-134">String</span></span>|<span data-ttu-id="62613-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="62613-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-136">displayName</span><span class="sxs-lookup"><span data-stu-id="62613-136">displayName</span></span>|<span data-ttu-id="62613-137">String</span><span class="sxs-lookup"><span data-stu-id="62613-137">String</span></span>|<span data-ttu-id="62613-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="62613-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-139">説明</span><span class="sxs-lookup"><span data-stu-id="62613-139">description</span></span>|<span data-ttu-id="62613-140">String</span><span class="sxs-lookup"><span data-stu-id="62613-140">String</span></span>|<span data-ttu-id="62613-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="62613-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="62613-142">requiresUserAuthentication</span></span>|<span data-ttu-id="62613-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-143">Boolean</span></span>|<span data-ttu-id="62613-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="62613-145">configurationEndpointUrl</span></span>|<span data-ttu-id="62613-146">String</span><span class="sxs-lookup"><span data-stu-id="62613-146">String</span></span>|<span data-ttu-id="62613-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="62613-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="62613-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="62613-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-149">Boolean</span></span>|<span data-ttu-id="62613-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="62613-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="62613-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="62613-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62613-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="62613-152">isDefault</span></span>|<span data-ttu-id="62613-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-153">Boolean</span></span>|<span data-ttu-id="62613-154">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="62613-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="62613-155">supervisedModeEnabled</span></span>|<span data-ttu-id="62613-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-156">Boolean</span></span>|<span data-ttu-id="62613-157">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="62613-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="62613-158">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="62613-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="62613-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="62613-159">supportDepartment</span></span>|<span data-ttu-id="62613-160">String</span><span class="sxs-lookup"><span data-stu-id="62613-160">String</span></span>|<span data-ttu-id="62613-161">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="62613-161">Support department information</span></span>|
|<span data-ttu-id="62613-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-162">passCodeDisabled</span></span>|<span data-ttu-id="62613-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-163">Boolean</span></span>|<span data-ttu-id="62613-164">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="62613-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="62613-165">isMandatory</span></span>|<span data-ttu-id="62613-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-166">Boolean</span></span>|<span data-ttu-id="62613-167">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="62613-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="62613-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-168">locationDisabled</span></span>|<span data-ttu-id="62613-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-169">Boolean</span></span>|<span data-ttu-id="62613-170">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="62613-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="62613-171">supportPhoneNumber</span></span>|<span data-ttu-id="62613-172">String</span><span class="sxs-lookup"><span data-stu-id="62613-172">String</span></span>|<span data-ttu-id="62613-173">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="62613-173">Support phone number</span></span>|
|<span data-ttu-id="62613-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="62613-174">iTunesPairingMode</span></span>|[<span data-ttu-id="62613-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="62613-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="62613-176">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="62613-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="62613-177">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="62613-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="62613-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-178">profileRemovalDisabled</span></span>|<span data-ttu-id="62613-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-179">Boolean</span></span>|<span data-ttu-id="62613-180">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="62613-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="62613-181">managementCertificates</span></span>|<span data-ttu-id="62613-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62613-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="62613-183">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="62613-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="62613-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="62613-184">restoreBlocked</span></span>|<span data-ttu-id="62613-185">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-185">Boolean</span></span>|<span data-ttu-id="62613-186">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="62613-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="62613-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="62613-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-188">Boolean</span></span>|<span data-ttu-id="62613-189">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="62613-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-190">appleIdDisabled</span></span>|<span data-ttu-id="62613-191">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-191">Boolean</span></span>|<span data-ttu-id="62613-192">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="62613-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="62613-194">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-194">Boolean</span></span>|<span data-ttu-id="62613-195">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="62613-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-196">touchIdDisabled</span></span>|<span data-ttu-id="62613-197">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-197">Boolean</span></span>|<span data-ttu-id="62613-198">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="62613-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-199">applePayDisabled</span></span>|<span data-ttu-id="62613-200">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-200">Boolean</span></span>|<span data-ttu-id="62613-201">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="62613-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-202">zoomDisabled</span></span>|<span data-ttu-id="62613-203">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-203">Boolean</span></span>|<span data-ttu-id="62613-204">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="62613-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-205">siriDisabled</span></span>|<span data-ttu-id="62613-206">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-206">Boolean</span></span>|<span data-ttu-id="62613-207">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="62613-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-208">diagnosticsDisabled</span></span>|<span data-ttu-id="62613-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-209">Boolean</span></span>|<span data-ttu-id="62613-210">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="62613-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="62613-212">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-212">Boolean</span></span>|<span data-ttu-id="62613-213">Mac OS の登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="62613-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="62613-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="62613-215">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-215">Boolean</span></span>|<span data-ttu-id="62613-216">Mac OS ファイルのボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="62613-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="62613-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="62613-218">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-218">Boolean</span></span>|<span data-ttu-id="62613-219">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="62613-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="62613-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="62613-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="62613-221">Int32</span><span class="sxs-lookup"><span data-stu-id="62613-221">Int32</span></span>|<span data-ttu-id="62613-222">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="62613-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="62613-223">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="62613-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="62613-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="62613-224">enableSharedIPad</span></span>|<span data-ttu-id="62613-225">ブール値</span><span class="sxs-lookup"><span data-stu-id="62613-225">Boolean</span></span>|<span data-ttu-id="62613-226">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62613-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="62613-227">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="62613-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="62613-228">応答</span><span class="sxs-lookup"><span data-stu-id="62613-228">Response</span></span>
<span data-ttu-id="62613-229">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="62613-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62613-230">例</span><span class="sxs-lookup"><span data-stu-id="62613-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="62613-231">要求</span><span class="sxs-lookup"><span data-stu-id="62613-231">Request</span></span>
<span data-ttu-id="62613-232">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62613-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62613-233">応答</span><span class="sxs-lookup"><span data-stu-id="62613-233">Response</span></span>
<span data-ttu-id="62613-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62613-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





