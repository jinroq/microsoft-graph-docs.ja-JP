---
title: depEnrollmentProfile の更新
description: depEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70690403a2c7d2855ce94ac0c58f99d214a7bf7f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969422"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="8b345-103">depEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="8b345-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="8b345-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b345-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b345-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b345-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b345-106">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8b345-106">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b345-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b345-107">Prerequisites</span></span>
<span data-ttu-id="8b345-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b345-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b345-110">Permission type</span></span>|<span data-ttu-id="8b345-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b345-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b345-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b345-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b345-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b345-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b345-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b345-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b345-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b345-115">Not supported.</span></span>|
|<span data-ttu-id="8b345-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b345-116">Application</span></span>|<span data-ttu-id="8b345-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b345-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b345-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b345-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8b345-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b345-119">Request headers</span></span>
|<span data-ttu-id="8b345-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b345-120">Header</span></span>|<span data-ttu-id="8b345-121">値</span><span class="sxs-lookup"><span data-stu-id="8b345-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b345-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b345-122">Authorization</span></span>|<span data-ttu-id="8b345-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b345-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b345-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8b345-124">Accept</span></span>|<span data-ttu-id="8b345-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b345-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b345-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b345-126">Request body</span></span>
<span data-ttu-id="8b345-127">要求本文で、 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b345-127">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8b345-128">次の表に、 [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-128">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="8b345-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b345-129">Property</span></span>|<span data-ttu-id="8b345-130">型</span><span class="sxs-lookup"><span data-stu-id="8b345-130">Type</span></span>|<span data-ttu-id="8b345-131">説明</span><span class="sxs-lookup"><span data-stu-id="8b345-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b345-132">id</span><span class="sxs-lookup"><span data-stu-id="8b345-132">id</span></span>|<span data-ttu-id="8b345-133">String</span><span class="sxs-lookup"><span data-stu-id="8b345-133">String</span></span>|<span data-ttu-id="8b345-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="8b345-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8b345-135">displayName</span></span>|<span data-ttu-id="8b345-136">String</span><span class="sxs-lookup"><span data-stu-id="8b345-136">String</span></span>|<span data-ttu-id="8b345-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="8b345-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-138">description</span><span class="sxs-lookup"><span data-stu-id="8b345-138">description</span></span>|<span data-ttu-id="8b345-139">String</span><span class="sxs-lookup"><span data-stu-id="8b345-139">String</span></span>|<span data-ttu-id="8b345-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="8b345-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8b345-141">requiresUserAuthentication</span></span>|<span data-ttu-id="8b345-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-142">Boolean</span></span>|<span data-ttu-id="8b345-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="8b345-144">configurationEndpointUrl</span></span>|<span data-ttu-id="8b345-145">String</span><span class="sxs-lookup"><span data-stu-id="8b345-145">String</span></span>|<span data-ttu-id="8b345-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="8b345-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="8b345-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8b345-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-148">Boolean</span></span>|<span data-ttu-id="8b345-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="8b345-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8b345-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="8b345-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="8b345-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-152">Boolean</span></span>|<span data-ttu-id="8b345-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b345-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="8b345-154">isDefault</span></span>|<span data-ttu-id="8b345-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8b345-155">Boolean</span></span>|<span data-ttu-id="8b345-156">これが既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="8b345-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="8b345-157">supervisedModeEnabled</span></span>|<span data-ttu-id="8b345-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-158">Boolean</span></span>|<span data-ttu-id="8b345-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="8b345-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="8b345-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b345-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="8b345-161">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="8b345-161">supportDepartment</span></span>|<span data-ttu-id="8b345-162">String</span><span class="sxs-lookup"><span data-stu-id="8b345-162">String</span></span>|<span data-ttu-id="8b345-163">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="8b345-163">Support department information</span></span>|
|<span data-ttu-id="8b345-164">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-164">passCodeDisabled</span></span>|<span data-ttu-id="8b345-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-165">Boolean</span></span>|<span data-ttu-id="8b345-166">パスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-167">ismandatory</span><span class="sxs-lookup"><span data-stu-id="8b345-167">isMandatory</span></span>|<span data-ttu-id="8b345-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-168">Boolean</span></span>|<span data-ttu-id="8b345-169">プロファイルが必須であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="8b345-170">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-170">locationDisabled</span></span>|<span data-ttu-id="8b345-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-171">Boolean</span></span>|<span data-ttu-id="8b345-172">場所サービスの設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8b345-173">supportPhoneNumber</span></span>|<span data-ttu-id="8b345-174">String</span><span class="sxs-lookup"><span data-stu-id="8b345-174">String</span></span>|<span data-ttu-id="8b345-175">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="8b345-175">Support phone number</span></span>|
|<span data-ttu-id="8b345-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8b345-176">iTunesPairingMode</span></span>|[<span data-ttu-id="8b345-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8b345-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="8b345-178">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="8b345-179">使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="8b345-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="8b345-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-180">profileRemovalDisabled</span></span>|<span data-ttu-id="8b345-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-181">Boolean</span></span>|<span data-ttu-id="8b345-182">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="8b345-183">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="8b345-183">managementCertificates</span></span>|<span data-ttu-id="8b345-184">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8b345-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="8b345-185">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="8b345-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="8b345-186">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="8b345-186">restoreBlocked</span></span>|<span data-ttu-id="8b345-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-187">Boolean</span></span>|<span data-ttu-id="8b345-188">セットアップウィンドウの復元がブロックされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="8b345-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="8b345-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-190">Boolean</span></span>|<span data-ttu-id="8b345-191">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="8b345-192">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-192">appleIdDisabled</span></span>|<span data-ttu-id="8b345-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-193">Boolean</span></span>|<span data-ttu-id="8b345-194">Apple id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="8b345-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-196">Boolean</span></span>|<span data-ttu-id="8b345-197">[使用条件] セットアップウィンドウが無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-198">touchIdDisabled</span></span>|<span data-ttu-id="8b345-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-199">Boolean</span></span>|<span data-ttu-id="8b345-200">タッチ id のセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-201">applePayDisabled</span></span>|<span data-ttu-id="8b345-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-202">Boolean</span></span>|<span data-ttu-id="8b345-203">Apple の支払い設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-204">zoomDisabled</span></span>|<span data-ttu-id="8b345-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-205">Boolean</span></span>|<span data-ttu-id="8b345-206">ズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-207">siridisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-207">siriDisabled</span></span>|<span data-ttu-id="8b345-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-208">Boolean</span></span>|<span data-ttu-id="8b345-209">siri セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-210">diagnosticsDisabled</span></span>|<span data-ttu-id="8b345-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-211">Boolean</span></span>|<span data-ttu-id="8b345-212">診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="8b345-213">macosregistrationdisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="8b345-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-214">Boolean</span></span>|<span data-ttu-id="8b345-215">Mac OS 登録が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="8b345-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="8b345-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="8b345-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-217">Boolean</span></span>|<span data-ttu-id="8b345-218">Mac OS ファイルボルトが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="8b345-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="8b345-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="8b345-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-220">Boolean</span></span>|<span data-ttu-id="8b345-221">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b345-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="8b345-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="8b345-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="8b345-223">Int32</span><span class="sxs-lookup"><span data-stu-id="8b345-223">Int32</span></span>|<span data-ttu-id="8b345-224">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="8b345-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="8b345-225">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8b345-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="8b345-226">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="8b345-226">enableSharedIPad</span></span>|<span data-ttu-id="8b345-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b345-227">Boolean</span></span>|<span data-ttu-id="8b345-228">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8b345-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="8b345-229">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8b345-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="8b345-230">応答</span><span class="sxs-lookup"><span data-stu-id="8b345-230">Response</span></span>
<span data-ttu-id="8b345-231">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8b345-231">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b345-232">例</span><span class="sxs-lookup"><span data-stu-id="8b345-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b345-233">要求</span><span class="sxs-lookup"><span data-stu-id="8b345-233">Request</span></span>
<span data-ttu-id="8b345-234">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b345-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b345-235">応答</span><span class="sxs-lookup"><span data-stu-id="8b345-235">Response</span></span>
<span data-ttu-id="8b345-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b345-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




