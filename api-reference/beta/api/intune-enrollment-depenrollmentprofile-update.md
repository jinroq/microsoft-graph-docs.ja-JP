---
title: DepEnrollmentProfile の更新
description: DepEnrollmentProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff10fda496fd640454ae37bda6e673da4b0a68a6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979033"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="15576-103">DepEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="15576-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="15576-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15576-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15576-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15576-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15576-106">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15576-106">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15576-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="15576-107">Prerequisites</span></span>
<span data-ttu-id="15576-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15576-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15576-110">Permission type</span></span>|<span data-ttu-id="15576-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15576-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15576-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15576-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15576-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15576-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15576-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15576-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15576-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15576-115">Not supported.</span></span>|
|<span data-ttu-id="15576-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15576-116">Application</span></span>|<span data-ttu-id="15576-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15576-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15576-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15576-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="15576-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15576-119">Request headers</span></span>
|<span data-ttu-id="15576-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15576-120">Header</span></span>|<span data-ttu-id="15576-121">値</span><span class="sxs-lookup"><span data-stu-id="15576-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15576-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15576-122">Authorization</span></span>|<span data-ttu-id="15576-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="15576-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15576-124">承諾</span><span class="sxs-lookup"><span data-stu-id="15576-124">Accept</span></span>|<span data-ttu-id="15576-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15576-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15576-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="15576-126">Request body</span></span>
<span data-ttu-id="15576-127">要求本文で、 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="15576-127">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="15576-128">次の表に、 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-128">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="15576-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15576-129">Property</span></span>|<span data-ttu-id="15576-130">型</span><span class="sxs-lookup"><span data-stu-id="15576-130">Type</span></span>|<span data-ttu-id="15576-131">説明</span><span class="sxs-lookup"><span data-stu-id="15576-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15576-132">id</span><span class="sxs-lookup"><span data-stu-id="15576-132">id</span></span>|<span data-ttu-id="15576-133">文字列</span><span class="sxs-lookup"><span data-stu-id="15576-133">String</span></span>|<span data-ttu-id="15576-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="15576-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-135">displayName</span><span class="sxs-lookup"><span data-stu-id="15576-135">displayName</span></span>|<span data-ttu-id="15576-136">String</span><span class="sxs-lookup"><span data-stu-id="15576-136">String</span></span>|<span data-ttu-id="15576-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="15576-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-138">description</span><span class="sxs-lookup"><span data-stu-id="15576-138">description</span></span>|<span data-ttu-id="15576-139">String</span><span class="sxs-lookup"><span data-stu-id="15576-139">String</span></span>|<span data-ttu-id="15576-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="15576-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="15576-141">requiresUserAuthentication</span></span>|<span data-ttu-id="15576-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-142">Boolean</span></span>|<span data-ttu-id="15576-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="15576-144">configurationEndpointUrl</span></span>|<span data-ttu-id="15576-145">String</span><span class="sxs-lookup"><span data-stu-id="15576-145">String</span></span>|<span data-ttu-id="15576-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="15576-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="15576-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="15576-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-148">Boolean</span></span>|<span data-ttu-id="15576-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="15576-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="15576-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="15576-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="15576-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-152">Boolean</span></span>|<span data-ttu-id="15576-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15576-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="15576-154">isDefault</span></span>|<span data-ttu-id="15576-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="15576-155">Boolean</span></span>|<span data-ttu-id="15576-156">これが既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="15576-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="15576-157">supervisedModeEnabled</span></span>|<span data-ttu-id="15576-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-158">Boolean</span></span>|<span data-ttu-id="15576-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="15576-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="15576-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15576-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="15576-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="15576-161">supportDepartment</span></span>|<span data-ttu-id="15576-162">String</span><span class="sxs-lookup"><span data-stu-id="15576-162">String</span></span>|<span data-ttu-id="15576-163">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="15576-163">Support department information</span></span>|
|<span data-ttu-id="15576-164">Pass Codedisabled</span><span class="sxs-lookup"><span data-stu-id="15576-164">passCodeDisabled</span></span>|<span data-ttu-id="15576-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-165">Boolean</span></span>|<span data-ttu-id="15576-166">パスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="15576-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="15576-167">isMandatory</span></span>|<span data-ttu-id="15576-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-168">Boolean</span></span>|<span data-ttu-id="15576-169">プロファイルが必須であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="15576-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-170">locationDisabled</span></span>|<span data-ttu-id="15576-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-171">Boolean</span></span>|<span data-ttu-id="15576-172">場所サービスの設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="15576-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="15576-173">supportPhoneNumber</span></span>|<span data-ttu-id="15576-174">String</span><span class="sxs-lookup"><span data-stu-id="15576-174">String</span></span>|<span data-ttu-id="15576-175">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="15576-175">Support phone number</span></span>|
|<span data-ttu-id="15576-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="15576-176">iTunesPairingMode</span></span>|[<span data-ttu-id="15576-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="15576-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="15576-178">ITunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="15576-179">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="15576-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="15576-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-180">profileRemovalDisabled</span></span>|<span data-ttu-id="15576-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-181">Boolean</span></span>|<span data-ttu-id="15576-182">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="15576-183">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="15576-183">managementCertificates</span></span>|<span data-ttu-id="15576-184">[Managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15576-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="15576-185">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="15576-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="15576-186">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="15576-186">restoreBlocked</span></span>|<span data-ttu-id="15576-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-187">Boolean</span></span>|<span data-ttu-id="15576-188">セットアップウィンドウの復元がブロックされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="15576-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="15576-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-190">Boolean</span></span>|<span data-ttu-id="15576-191">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="15576-192">りんご Eiddisabled</span><span class="sxs-lookup"><span data-stu-id="15576-192">appleIdDisabled</span></span>|<span data-ttu-id="15576-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-193">Boolean</span></span>|<span data-ttu-id="15576-194">Apple id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="15576-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="15576-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-196">Boolean</span></span>|<span data-ttu-id="15576-197">[使用条件] セットアップウィンドウが無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="15576-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-198">touchIdDisabled</span></span>|<span data-ttu-id="15576-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-199">Boolean</span></span>|<span data-ttu-id="15576-200">タッチ id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="15576-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-201">applePayDisabled</span></span>|<span data-ttu-id="15576-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-202">Boolean</span></span>|<span data-ttu-id="15576-203">Apple の支払い設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="15576-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-204">zoomDisabled</span></span>|<span data-ttu-id="15576-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-205">Boolean</span></span>|<span data-ttu-id="15576-206">ズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="15576-207">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-207">siriDisabled</span></span>|<span data-ttu-id="15576-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-208">Boolean</span></span>|<span data-ttu-id="15576-209">Siri セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="15576-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-210">diagnosticsDisabled</span></span>|<span data-ttu-id="15576-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-211">Boolean</span></span>|<span data-ttu-id="15576-212">診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="15576-213">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="15576-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-214">Boolean</span></span>|<span data-ttu-id="15576-215">Mac OS 登録が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="15576-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="15576-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="15576-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-217">Boolean</span></span>|<span data-ttu-id="15576-218">Mac OS ファイルボルトが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="15576-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="15576-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="15576-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-220">Boolean</span></span>|<span data-ttu-id="15576-221">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="15576-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="15576-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="15576-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="15576-223">Int32</span><span class="sxs-lookup"><span data-stu-id="15576-223">Int32</span></span>|<span data-ttu-id="15576-224">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="15576-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="15576-225">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="15576-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="15576-226">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="15576-226">enableSharedIPad</span></span>|<span data-ttu-id="15576-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="15576-227">Boolean</span></span>|<span data-ttu-id="15576-228">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15576-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="15576-229">共有 Ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="15576-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="15576-230">応答</span><span class="sxs-lookup"><span data-stu-id="15576-230">Response</span></span>
<span data-ttu-id="15576-231">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15576-231">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15576-232">例</span><span class="sxs-lookup"><span data-stu-id="15576-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="15576-233">要求</span><span class="sxs-lookup"><span data-stu-id="15576-233">Request</span></span>
<span data-ttu-id="15576-234">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15576-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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

### <a name="response"></a><span data-ttu-id="15576-235">応答</span><span class="sxs-lookup"><span data-stu-id="15576-235">Response</span></span>
<span data-ttu-id="15576-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15576-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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





