---
title: DepMacOSEnrollmentProfile を更新します。
description: DepMacOSEnrollmentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f86e520160e988e72aaa2473b256613a997cae0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420116"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="bab1b-103">DepMacOSEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="bab1b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bab1b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bab1b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bab1b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bab1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bab1b-107">[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bab1b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bab1b-108">Prerequisites</span></span>
<span data-ttu-id="bab1b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bab1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bab1b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bab1b-111">Permission type</span></span>|<span data-ttu-id="bab1b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bab1b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bab1b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bab1b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bab1b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab1b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bab1b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bab1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab1b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab1b-116">Not supported.</span></span>|
|<span data-ttu-id="bab1b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bab1b-117">Application</span></span>|<span data-ttu-id="bab1b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab1b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bab1b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bab1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="bab1b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bab1b-120">Request headers</span></span>
|<span data-ttu-id="bab1b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bab1b-121">Header</span></span>|<span data-ttu-id="bab1b-122">値</span><span class="sxs-lookup"><span data-stu-id="bab1b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bab1b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab1b-123">Authorization</span></span>|<span data-ttu-id="bab1b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bab1b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bab1b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bab1b-125">Accept</span></span>|<span data-ttu-id="bab1b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bab1b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab1b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bab1b-127">Request body</span></span>
<span data-ttu-id="bab1b-128">要求の本文に[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="bab1b-129">[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="bab1b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bab1b-130">Property</span></span>|<span data-ttu-id="bab1b-131">型</span><span class="sxs-lookup"><span data-stu-id="bab1b-131">Type</span></span>|<span data-ttu-id="bab1b-132">説明</span><span class="sxs-lookup"><span data-stu-id="bab1b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bab1b-133">id</span><span class="sxs-lookup"><span data-stu-id="bab1b-133">id</span></span>|<span data-ttu-id="bab1b-134">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-134">String</span></span>|<span data-ttu-id="bab1b-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="bab1b-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bab1b-136">displayName</span></span>|<span data-ttu-id="bab1b-137">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-137">String</span></span>|<span data-ttu-id="bab1b-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="bab1b-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-139">説明</span><span class="sxs-lookup"><span data-stu-id="bab1b-139">description</span></span>|<span data-ttu-id="bab1b-140">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-140">String</span></span>|<span data-ttu-id="bab1b-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="bab1b-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="bab1b-142">requiresUserAuthentication</span></span>|<span data-ttu-id="bab1b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-143">Boolean</span></span>|<span data-ttu-id="bab1b-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="bab1b-145">configurationEndpointUrl</span></span>|<span data-ttu-id="bab1b-146">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-146">String</span></span>|<span data-ttu-id="bab1b-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="bab1b-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="bab1b-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="bab1b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-149">Boolean</span></span>|<span data-ttu-id="bab1b-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="bab1b-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="bab1b-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="bab1b-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-153">Boolean</span></span>|<span data-ttu-id="bab1b-154">継承セットアップ アシスタントが登録されているデバイスは、 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)からの会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="bab1b-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bab1b-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="bab1b-155">isDefault</span></span>|<span data-ttu-id="bab1b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-156">Boolean</span></span>|<span data-ttu-id="bab1b-157">これは、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承される既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-158">supervisedModeEnabled</span></span>|<span data-ttu-id="bab1b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-159">Boolean</span></span>|<span data-ttu-id="bab1b-160">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="bab1b-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="bab1b-161">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="bab1b-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="bab1b-162">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="bab1b-163">supportDepartment</span></span>|<span data-ttu-id="bab1b-164">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-164">String</span></span>|<span data-ttu-id="bab1b-165">継承のサポート部門については、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="bab1b-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-166">passCodeDisabled</span></span>|<span data-ttu-id="bab1b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-167">Boolean</span></span>|<span data-ttu-id="bab1b-168">パスコードの設定] ウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="bab1b-169">isMandatory</span></span>|<span data-ttu-id="bab1b-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-170">Boolean</span></span>|<span data-ttu-id="bab1b-171">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承が必須であるかを示す</span><span class="sxs-lookup"><span data-stu-id="bab1b-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-172">locationDisabled</span></span>|<span data-ttu-id="bab1b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-173">Boolean</span></span>|<span data-ttu-id="bab1b-174">サービス セットアップ] ウィンドウの場所が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="bab1b-175">supportPhoneNumber</span></span>|<span data-ttu-id="bab1b-176">String</span><span class="sxs-lookup"><span data-stu-id="bab1b-176">String</span></span>|<span data-ttu-id="bab1b-177">継承のサポート電話番号は、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="bab1b-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-178">profileRemovalDisabled</span></span>|<span data-ttu-id="bab1b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-179">Boolean</span></span>|<span data-ttu-id="bab1b-180">プロファイルの削除オプションが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bab1b-181">restoreBlocked</span></span>|<span data-ttu-id="bab1b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-182">Boolean</span></span>|<span data-ttu-id="bab1b-183">復元の設定] ウィンドウがブロックされていることを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-184">appleIdDisabled</span></span>|<span data-ttu-id="bab1b-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-185">Boolean</span></span>|<span data-ttu-id="bab1b-186">Id の設定] ウィンドウは、Apple が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="bab1b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-188">Boolean</span></span>|<span data-ttu-id="bab1b-189">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-190">touchIdDisabled</span></span>|<span data-ttu-id="bab1b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-191">Boolean</span></span>|<span data-ttu-id="bab1b-192">タッチ id の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-193">applePayDisabled</span></span>|<span data-ttu-id="bab1b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-194">Boolean</span></span>|<span data-ttu-id="bab1b-195">アップル支払設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-196">zoomDisabled</span></span>|<span data-ttu-id="bab1b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-197">Boolean</span></span>|<span data-ttu-id="bab1b-198">ズームの設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-199">siriDisabled</span></span>|<span data-ttu-id="bab1b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-200">Boolean</span></span>|<span data-ttu-id="bab1b-201">Siri の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-202">diagnosticsDisabled</span></span>|<span data-ttu-id="bab1b-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-203">Boolean</span></span>|<span data-ttu-id="bab1b-204">設定] ウィンドウは、診断が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="bab1b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-206">Boolean</span></span>|<span data-ttu-id="bab1b-207">Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-208">privacyPaneDisabled</span></span>|<span data-ttu-id="bab1b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-209">Boolean</span></span>|<span data-ttu-id="bab1b-210">プライバシー画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bab1b-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bab1b-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-211">registrationDisabled</span></span>|<span data-ttu-id="bab1b-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-212">Boolean</span></span>|<span data-ttu-id="bab1b-213">登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="bab1b-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-214">fileVaultDisabled</span></span>|<span data-ttu-id="bab1b-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-215">Boolean</span></span>|<span data-ttu-id="bab1b-216">ファイルボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="bab1b-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="bab1b-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="bab1b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="bab1b-218">Boolean</span></span>|<span data-ttu-id="bab1b-219">ICloud 分析画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="bab1b-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="bab1b-220">応答</span><span class="sxs-lookup"><span data-stu-id="bab1b-220">Response</span></span>
<span data-ttu-id="bab1b-221">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bab1b-221">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bab1b-222">例</span><span class="sxs-lookup"><span data-stu-id="bab1b-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="bab1b-223">要求</span><span class="sxs-lookup"><span data-stu-id="bab1b-223">Request</span></span>
<span data-ttu-id="bab1b-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bab1b-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1061

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="bab1b-225">応答</span><span class="sxs-lookup"><span data-stu-id="bab1b-225">Response</span></span>
<span data-ttu-id="bab1b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bab1b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```




