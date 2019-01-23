---
title: DepEnrollmentProfile を更新します。
description: DepEnrollmentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f8bb392eba1ca79815d72baf9f89e790cb16d95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419528"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="0eb8f-103">DepEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="0eb8f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0eb8f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0eb8f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eb8f-107">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb8f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0eb8f-108">Prerequisites</span></span>
<span data-ttu-id="0eb8f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0eb8f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0eb8f-111">Permission type</span></span>|<span data-ttu-id="0eb8f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0eb8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eb8f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0eb8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0eb8f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb8f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0eb8f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0eb8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eb8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-116">Not supported.</span></span>|
|<span data-ttu-id="0eb8f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0eb8f-117">Application</span></span>|<span data-ttu-id="0eb8f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eb8f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0eb8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0eb8f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0eb8f-120">Request headers</span></span>
|<span data-ttu-id="0eb8f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0eb8f-121">Header</span></span>|<span data-ttu-id="0eb8f-122">値</span><span class="sxs-lookup"><span data-stu-id="0eb8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eb8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eb8f-123">Authorization</span></span>|<span data-ttu-id="0eb8f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eb8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0eb8f-125">Accept</span></span>|<span data-ttu-id="0eb8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb8f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0eb8f-127">Request body</span></span>
<span data-ttu-id="0eb8f-128">要求の本文に[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0eb8f-129">[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="0eb8f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0eb8f-130">Property</span></span>|<span data-ttu-id="0eb8f-131">型</span><span class="sxs-lookup"><span data-stu-id="0eb8f-131">Type</span></span>|<span data-ttu-id="0eb8f-132">説明</span><span class="sxs-lookup"><span data-stu-id="0eb8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eb8f-133">id</span><span class="sxs-lookup"><span data-stu-id="0eb8f-133">id</span></span>|<span data-ttu-id="0eb8f-134">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-134">String</span></span>|<span data-ttu-id="0eb8f-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="0eb8f-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0eb8f-136">displayName</span></span>|<span data-ttu-id="0eb8f-137">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-137">String</span></span>|<span data-ttu-id="0eb8f-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="0eb8f-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-139">説明</span><span class="sxs-lookup"><span data-stu-id="0eb8f-139">description</span></span>|<span data-ttu-id="0eb8f-140">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-140">String</span></span>|<span data-ttu-id="0eb8f-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="0eb8f-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="0eb8f-142">requiresUserAuthentication</span></span>|<span data-ttu-id="0eb8f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-143">Boolean</span></span>|<span data-ttu-id="0eb8f-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="0eb8f-145">configurationEndpointUrl</span></span>|<span data-ttu-id="0eb8f-146">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-146">String</span></span>|<span data-ttu-id="0eb8f-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="0eb8f-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0eb8f-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0eb8f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-149">Boolean</span></span>|<span data-ttu-id="0eb8f-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="0eb8f-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="0eb8f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="0eb8f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-153">Boolean</span></span>|<span data-ttu-id="0eb8f-154">継承セットアップ アシスタントが登録されているデバイスは、 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)からの会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0eb8f-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="0eb8f-155">isDefault</span></span>|<span data-ttu-id="0eb8f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-156">Boolean</span></span>|<span data-ttu-id="0eb8f-157">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="0eb8f-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-158">supervisedModeEnabled</span></span>|<span data-ttu-id="0eb8f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-159">Boolean</span></span>|<span data-ttu-id="0eb8f-160">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="0eb8f-161">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="0eb8f-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="0eb8f-162">supportDepartment</span></span>|<span data-ttu-id="0eb8f-163">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-163">String</span></span>|<span data-ttu-id="0eb8f-164">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="0eb8f-164">Support department information</span></span>|
|<span data-ttu-id="0eb8f-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-165">passCodeDisabled</span></span>|<span data-ttu-id="0eb8f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-166">Boolean</span></span>|<span data-ttu-id="0eb8f-167">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="0eb8f-168">isMandatory</span></span>|<span data-ttu-id="0eb8f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-169">Boolean</span></span>|<span data-ttu-id="0eb8f-170">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="0eb8f-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="0eb8f-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-171">locationDisabled</span></span>|<span data-ttu-id="0eb8f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-172">Boolean</span></span>|<span data-ttu-id="0eb8f-173">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0eb8f-174">supportPhoneNumber</span></span>|<span data-ttu-id="0eb8f-175">String</span><span class="sxs-lookup"><span data-stu-id="0eb8f-175">String</span></span>|<span data-ttu-id="0eb8f-176">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="0eb8f-176">Support phone number</span></span>|
|<span data-ttu-id="0eb8f-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="0eb8f-177">iTunesPairingMode</span></span>|[<span data-ttu-id="0eb8f-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="0eb8f-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="0eb8f-179">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="0eb8f-180">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="0eb8f-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-181">profileRemovalDisabled</span></span>|<span data-ttu-id="0eb8f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-182">Boolean</span></span>|<span data-ttu-id="0eb8f-183">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="0eb8f-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="0eb8f-184">managementCertificates</span></span>|<span data-ttu-id="0eb8f-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0eb8f-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="0eb8f-186">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="0eb8f-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="0eb8f-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="0eb8f-187">restoreBlocked</span></span>|<span data-ttu-id="0eb8f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-188">Boolean</span></span>|<span data-ttu-id="0eb8f-189">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="0eb8f-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="0eb8f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-191">Boolean</span></span>|<span data-ttu-id="0eb8f-192">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="0eb8f-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-193">appleIdDisabled</span></span>|<span data-ttu-id="0eb8f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-194">Boolean</span></span>|<span data-ttu-id="0eb8f-195">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="0eb8f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-197">Boolean</span></span>|<span data-ttu-id="0eb8f-198">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-199">touchIdDisabled</span></span>|<span data-ttu-id="0eb8f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-200">Boolean</span></span>|<span data-ttu-id="0eb8f-201">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-202">applePayDisabled</span></span>|<span data-ttu-id="0eb8f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-203">Boolean</span></span>|<span data-ttu-id="0eb8f-204">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-205">zoomDisabled</span></span>|<span data-ttu-id="0eb8f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-206">Boolean</span></span>|<span data-ttu-id="0eb8f-207">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-208">siriDisabled</span></span>|<span data-ttu-id="0eb8f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-209">Boolean</span></span>|<span data-ttu-id="0eb8f-210">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-211">diagnosticsDisabled</span></span>|<span data-ttu-id="0eb8f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-212">Boolean</span></span>|<span data-ttu-id="0eb8f-213">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="0eb8f-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="0eb8f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-215">Boolean</span></span>|<span data-ttu-id="0eb8f-216">Mac OS の登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="0eb8f-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="0eb8f-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="0eb8f-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-218">Boolean</span></span>|<span data-ttu-id="0eb8f-219">Mac OS ファイルのボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="0eb8f-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="0eb8f-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="0eb8f-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-221">Boolean</span></span>|<span data-ttu-id="0eb8f-222">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0eb8f-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="0eb8f-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="0eb8f-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="0eb8f-224">Int32</span><span class="sxs-lookup"><span data-stu-id="0eb8f-224">Int32</span></span>|<span data-ttu-id="0eb8f-225">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="0eb8f-226">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="0eb8f-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="0eb8f-227">enableSharedIPad</span></span>|<span data-ttu-id="0eb8f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb8f-228">Boolean</span></span>|<span data-ttu-id="0eb8f-229">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="0eb8f-230">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="0eb8f-231">応答</span><span class="sxs-lookup"><span data-stu-id="0eb8f-231">Response</span></span>
<span data-ttu-id="0eb8f-232">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb8f-233">例</span><span class="sxs-lookup"><span data-stu-id="0eb8f-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eb8f-234">要求</span><span class="sxs-lookup"><span data-stu-id="0eb8f-234">Request</span></span>
<span data-ttu-id="0eb8f-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0eb8f-236">応答</span><span class="sxs-lookup"><span data-stu-id="0eb8f-236">Response</span></span>
<span data-ttu-id="0eb8f-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0eb8f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




