---
title: DepEnrollmentProfile を作成します。
description: 新しい depEnrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96a9b1256aa62e14140b533a7980774ace7ba115
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919044"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="65eac-103">DepEnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="65eac-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="65eac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65eac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65eac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65eac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65eac-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65eac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65eac-107">新しい[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65eac-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65eac-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="65eac-108">Prerequisites</span></span>
<span data-ttu-id="65eac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65eac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65eac-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65eac-111">Permission type</span></span>|<span data-ttu-id="65eac-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65eac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65eac-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65eac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65eac-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65eac-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65eac-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65eac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65eac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65eac-116">Not supported.</span></span>|
|<span data-ttu-id="65eac-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65eac-117">Application</span></span>|<span data-ttu-id="65eac-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65eac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65eac-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65eac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="65eac-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65eac-120">Request headers</span></span>
|<span data-ttu-id="65eac-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65eac-121">Header</span></span>|<span data-ttu-id="65eac-122">値</span><span class="sxs-lookup"><span data-stu-id="65eac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65eac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65eac-123">Authorization</span></span>|<span data-ttu-id="65eac-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="65eac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65eac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65eac-125">Accept</span></span>|<span data-ttu-id="65eac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65eac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65eac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="65eac-127">Request body</span></span>
<span data-ttu-id="65eac-128">要求の本文に depEnrollmentProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="65eac-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="65eac-129">次の表は、depEnrollmentProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="65eac-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="65eac-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65eac-130">Property</span></span>|<span data-ttu-id="65eac-131">種類</span><span class="sxs-lookup"><span data-stu-id="65eac-131">Type</span></span>|<span data-ttu-id="65eac-132">説明</span><span class="sxs-lookup"><span data-stu-id="65eac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65eac-133">ID</span><span class="sxs-lookup"><span data-stu-id="65eac-133">id</span></span>|<span data-ttu-id="65eac-134">String</span><span class="sxs-lookup"><span data-stu-id="65eac-134">String</span></span>|<span data-ttu-id="65eac-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="65eac-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="65eac-136">displayName</span></span>|<span data-ttu-id="65eac-137">String</span><span class="sxs-lookup"><span data-stu-id="65eac-137">String</span></span>|<span data-ttu-id="65eac-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="65eac-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-139">説明</span><span class="sxs-lookup"><span data-stu-id="65eac-139">description</span></span>|<span data-ttu-id="65eac-140">String</span><span class="sxs-lookup"><span data-stu-id="65eac-140">String</span></span>|<span data-ttu-id="65eac-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="65eac-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="65eac-142">requiresUserAuthentication</span></span>|<span data-ttu-id="65eac-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-143">Boolean</span></span>|<span data-ttu-id="65eac-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="65eac-145">configurationEndpointUrl</span></span>|<span data-ttu-id="65eac-146">String</span><span class="sxs-lookup"><span data-stu-id="65eac-146">String</span></span>|<span data-ttu-id="65eac-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="65eac-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="65eac-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="65eac-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-149">Boolean</span></span>|<span data-ttu-id="65eac-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="65eac-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="65eac-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="65eac-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="65eac-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="65eac-152">isDefault</span></span>|<span data-ttu-id="65eac-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-153">Boolean</span></span>|<span data-ttu-id="65eac-154">これは、既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="65eac-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="65eac-155">supervisedModeEnabled</span></span>|<span data-ttu-id="65eac-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-156">Boolean</span></span>|<span data-ttu-id="65eac-157">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="65eac-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="65eac-158">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="65eac-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="65eac-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="65eac-159">supportDepartment</span></span>|<span data-ttu-id="65eac-160">String</span><span class="sxs-lookup"><span data-stu-id="65eac-160">String</span></span>|<span data-ttu-id="65eac-161">サポート部門の情報</span><span class="sxs-lookup"><span data-stu-id="65eac-161">Support department information</span></span>|
|<span data-ttu-id="65eac-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-162">passCodeDisabled</span></span>|<span data-ttu-id="65eac-163">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-163">Boolean</span></span>|<span data-ttu-id="65eac-164">パスコードの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="65eac-165">isMandatory</span></span>|<span data-ttu-id="65eac-166">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-166">Boolean</span></span>|<span data-ttu-id="65eac-167">プロファイルが必須かどうかを</span><span class="sxs-lookup"><span data-stu-id="65eac-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="65eac-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-168">locationDisabled</span></span>|<span data-ttu-id="65eac-169">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-169">Boolean</span></span>|<span data-ttu-id="65eac-170">場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="65eac-171">supportPhoneNumber</span></span>|<span data-ttu-id="65eac-172">String</span><span class="sxs-lookup"><span data-stu-id="65eac-172">String</span></span>|<span data-ttu-id="65eac-173">サポート電話番号</span><span class="sxs-lookup"><span data-stu-id="65eac-173">Support phone number</span></span>|
|<span data-ttu-id="65eac-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="65eac-174">iTunesPairingMode</span></span>|[<span data-ttu-id="65eac-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="65eac-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="65eac-176">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="65eac-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="65eac-177">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="65eac-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="65eac-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-178">profileRemovalDisabled</span></span>|<span data-ttu-id="65eac-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-179">Boolean</span></span>|<span data-ttu-id="65eac-180">プロファイルの削除オプションが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="65eac-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="65eac-181">managementCertificates</span></span>|<span data-ttu-id="65eac-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65eac-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="65eac-183">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="65eac-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="65eac-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="65eac-184">restoreBlocked</span></span>|<span data-ttu-id="65eac-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-185">Boolean</span></span>|<span data-ttu-id="65eac-186">復元の設定] ウィンドウがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="65eac-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="65eac-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="65eac-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-188">Boolean</span></span>|<span data-ttu-id="65eac-189">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="65eac-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-190">appleIdDisabled</span></span>|<span data-ttu-id="65eac-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-191">Boolean</span></span>|<span data-ttu-id="65eac-192">Apple id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="65eac-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-194">Boolean</span></span>|<span data-ttu-id="65eac-195">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-196">touchIdDisabled</span></span>|<span data-ttu-id="65eac-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-197">Boolean</span></span>|<span data-ttu-id="65eac-198">タッチ id の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-199">applePayDisabled</span></span>|<span data-ttu-id="65eac-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-200">Boolean</span></span>|<span data-ttu-id="65eac-201">アップル支払設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-202">zoomDisabled</span></span>|<span data-ttu-id="65eac-203">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-203">Boolean</span></span>|<span data-ttu-id="65eac-204">ズームの設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-205">siriDisabled</span></span>|<span data-ttu-id="65eac-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-206">Boolean</span></span>|<span data-ttu-id="65eac-207">Siri の設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-208">diagnosticsDisabled</span></span>|<span data-ttu-id="65eac-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-209">Boolean</span></span>|<span data-ttu-id="65eac-210">診断設定] ウィンドウが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="65eac-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="65eac-212">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-212">Boolean</span></span>|<span data-ttu-id="65eac-213">Mac OS の登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="65eac-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="65eac-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="65eac-215">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-215">Boolean</span></span>|<span data-ttu-id="65eac-216">Mac OS ファイルのボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="65eac-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="65eac-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="65eac-218">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-218">Boolean</span></span>|<span data-ttu-id="65eac-219">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="65eac-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="65eac-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="65eac-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="65eac-221">Int32</span><span class="sxs-lookup"><span data-stu-id="65eac-221">Int32</span></span>|<span data-ttu-id="65eac-222">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="65eac-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="65eac-223">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="65eac-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="65eac-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="65eac-224">enableSharedIPad</span></span>|<span data-ttu-id="65eac-225">ブール型</span><span class="sxs-lookup"><span data-stu-id="65eac-225">Boolean</span></span>|<span data-ttu-id="65eac-226">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65eac-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="65eac-227">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="65eac-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="65eac-228">応答</span><span class="sxs-lookup"><span data-stu-id="65eac-228">Response</span></span>
<span data-ttu-id="65eac-229">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="65eac-229">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65eac-230">例</span><span class="sxs-lookup"><span data-stu-id="65eac-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="65eac-231">要求</span><span class="sxs-lookup"><span data-stu-id="65eac-231">Request</span></span>
<span data-ttu-id="65eac-232">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65eac-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1290

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="65eac-233">応答</span><span class="sxs-lookup"><span data-stu-id="65eac-233">Response</span></span>
<span data-ttu-id="65eac-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65eac-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





