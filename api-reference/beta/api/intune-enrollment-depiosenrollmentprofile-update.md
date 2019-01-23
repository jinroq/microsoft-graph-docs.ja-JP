---
title: DepIOSEnrollmentProfile を更新します。
description: DepIOSEnrollmentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e36951d69f3047c69ccfc0d1e0a72247a0715db9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400593"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="b0685-103">DepIOSEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="b0685-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="b0685-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0685-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b0685-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0685-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0685-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0685-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0685-107">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b0685-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0685-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b0685-108">Prerequisites</span></span>
<span data-ttu-id="b0685-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0685-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0685-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0685-111">Permission type</span></span>|<span data-ttu-id="b0685-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0685-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0685-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0685-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0685-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0685-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0685-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0685-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0685-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0685-116">Not supported.</span></span>|
|<span data-ttu-id="b0685-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0685-117">Application</span></span>|<span data-ttu-id="b0685-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0685-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0685-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0685-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="b0685-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0685-120">Request headers</span></span>
|<span data-ttu-id="b0685-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0685-121">Header</span></span>|<span data-ttu-id="b0685-122">値</span><span class="sxs-lookup"><span data-stu-id="b0685-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0685-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0685-123">Authorization</span></span>|<span data-ttu-id="b0685-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b0685-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0685-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0685-125">Accept</span></span>|<span data-ttu-id="b0685-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0685-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0685-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0685-127">Request body</span></span>
<span data-ttu-id="b0685-128">要求の本文に[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0685-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="b0685-129">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="b0685-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0685-130">Property</span></span>|<span data-ttu-id="b0685-131">型</span><span class="sxs-lookup"><span data-stu-id="b0685-131">Type</span></span>|<span data-ttu-id="b0685-132">説明</span><span class="sxs-lookup"><span data-stu-id="b0685-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0685-133">id</span><span class="sxs-lookup"><span data-stu-id="b0685-133">id</span></span>|<span data-ttu-id="b0685-134">String</span><span class="sxs-lookup"><span data-stu-id="b0685-134">String</span></span>|<span data-ttu-id="b0685-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="b0685-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b0685-136">displayName</span></span>|<span data-ttu-id="b0685-137">String</span><span class="sxs-lookup"><span data-stu-id="b0685-137">String</span></span>|<span data-ttu-id="b0685-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="b0685-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-139">説明</span><span class="sxs-lookup"><span data-stu-id="b0685-139">description</span></span>|<span data-ttu-id="b0685-140">String</span><span class="sxs-lookup"><span data-stu-id="b0685-140">String</span></span>|<span data-ttu-id="b0685-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="b0685-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b0685-142">requiresUserAuthentication</span></span>|<span data-ttu-id="b0685-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-143">Boolean</span></span>|<span data-ttu-id="b0685-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b0685-145">configurationEndpointUrl</span></span>|<span data-ttu-id="b0685-146">String</span><span class="sxs-lookup"><span data-stu-id="b0685-146">String</span></span>|<span data-ttu-id="b0685-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="b0685-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b0685-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b0685-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-149">Boolean</span></span>|<span data-ttu-id="b0685-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="b0685-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b0685-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b0685-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-153">Boolean</span></span>|<span data-ttu-id="b0685-154">継承セットアップ アシスタントが登録されているデバイスは、 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)からの会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0685-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="b0685-155">isDefault</span></span>|<span data-ttu-id="b0685-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-156">Boolean</span></span>|<span data-ttu-id="b0685-157">これは、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承される既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="b0685-158">supervisedModeEnabled</span></span>|<span data-ttu-id="b0685-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-159">Boolean</span></span>|<span data-ttu-id="b0685-160">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="b0685-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="b0685-161">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="b0685-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="b0685-162">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="b0685-163">supportDepartment</span></span>|<span data-ttu-id="b0685-164">String</span><span class="sxs-lookup"><span data-stu-id="b0685-164">String</span></span>|<span data-ttu-id="b0685-165">継承のサポート部門については、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="b0685-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-166">passCodeDisabled</span></span>|<span data-ttu-id="b0685-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-167">Boolean</span></span>|<span data-ttu-id="b0685-168">パスコードの設定] ウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="b0685-169">isMandatory</span></span>|<span data-ttu-id="b0685-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-170">Boolean</span></span>|<span data-ttu-id="b0685-171">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承が必須であるかを示す</span><span class="sxs-lookup"><span data-stu-id="b0685-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-172">locationDisabled</span></span>|<span data-ttu-id="b0685-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-173">Boolean</span></span>|<span data-ttu-id="b0685-174">サービス セットアップ] ウィンドウの場所が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b0685-175">supportPhoneNumber</span></span>|<span data-ttu-id="b0685-176">String</span><span class="sxs-lookup"><span data-stu-id="b0685-176">String</span></span>|<span data-ttu-id="b0685-177">継承のサポート電話番号は、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="b0685-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-178">profileRemovalDisabled</span></span>|<span data-ttu-id="b0685-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-179">Boolean</span></span>|<span data-ttu-id="b0685-180">プロファイルの削除オプションが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0685-181">restoreBlocked</span></span>|<span data-ttu-id="b0685-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-182">Boolean</span></span>|<span data-ttu-id="b0685-183">復元の設定] ウィンドウがブロックされていることを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-184">appleIdDisabled</span></span>|<span data-ttu-id="b0685-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-185">Boolean</span></span>|<span data-ttu-id="b0685-186">Id の設定] ウィンドウは、Apple が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="b0685-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-188">Boolean</span></span>|<span data-ttu-id="b0685-189">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-190">touchIdDisabled</span></span>|<span data-ttu-id="b0685-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-191">Boolean</span></span>|<span data-ttu-id="b0685-192">タッチ id の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-193">applePayDisabled</span></span>|<span data-ttu-id="b0685-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-194">Boolean</span></span>|<span data-ttu-id="b0685-195">アップル支払設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-196">zoomDisabled</span></span>|<span data-ttu-id="b0685-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-197">Boolean</span></span>|<span data-ttu-id="b0685-198">ズームの設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-199">siriDisabled</span></span>|<span data-ttu-id="b0685-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-200">Boolean</span></span>|<span data-ttu-id="b0685-201">Siri の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-202">diagnosticsDisabled</span></span>|<span data-ttu-id="b0685-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-203">Boolean</span></span>|<span data-ttu-id="b0685-204">設定] ウィンドウは、診断が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="b0685-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-206">Boolean</span></span>|<span data-ttu-id="b0685-207">Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-208">privacyPaneDisabled</span></span>|<span data-ttu-id="b0685-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-209">Boolean</span></span>|<span data-ttu-id="b0685-210">プライバシー画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b0685-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0685-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="b0685-211">iTunesPairingMode</span></span>|[<span data-ttu-id="b0685-212">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="b0685-212">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="b0685-213">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-213">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="b0685-214">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="b0685-214">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="b0685-215">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="b0685-215">managementCertificates</span></span>|<span data-ttu-id="b0685-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b0685-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="b0685-217">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="b0685-217">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="b0685-218">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-218">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="b0685-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-219">Boolean</span></span>|<span data-ttu-id="b0685-220">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-220">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="b0685-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="b0685-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="b0685-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-222">Boolean</span></span>|<span data-ttu-id="b0685-223">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="b0685-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="b0685-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="b0685-225">Int32</span><span class="sxs-lookup"><span data-stu-id="b0685-225">Int32</span></span>|<span data-ttu-id="b0685-226">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0685-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="b0685-227">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="b0685-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="b0685-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="b0685-228">enableSharedIPad</span></span>|<span data-ttu-id="b0685-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-229">Boolean</span></span>|<span data-ttu-id="b0685-230">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="b0685-231">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="b0685-231">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="b0685-232">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="b0685-232">companyPortalVppTokenId</span></span>|<span data-ttu-id="b0685-233">String</span><span class="sxs-lookup"><span data-stu-id="b0685-233">String</span></span>|<span data-ttu-id="b0685-234">場合設定、デバイスのライセンスと企業ポータルを展開するどの Vpp トークンを使用する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-234">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="b0685-235">'enableAuthenticationViaCompanyPortal' は、このプロパティを設定するために設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0685-235">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="b0685-236">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="b0685-236">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="b0685-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-237">Boolean</span></span>|<span data-ttu-id="b0685-238">1 つのアプリケーション モードを有効にして、登録時にアプリケーション ロックを適用するデバイスを指示します。</span><span class="sxs-lookup"><span data-stu-id="b0685-238">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="b0685-239">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0685-239">Default is false.</span></span> <span data-ttu-id="b0685-240">'enableAuthenticationViaCompanyPortal' と 'companyPortalVppTokenId' は、このプロパティを設定するのに設定してください。</span><span class="sxs-lookup"><span data-stu-id="b0685-240">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="b0685-241">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-241">homeButtonScreenDisabled</span></span>|<span data-ttu-id="b0685-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-242">Boolean</span></span>|<span data-ttu-id="b0685-243">感度画面の [ホーム] ボタンが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-243">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="b0685-244">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-244">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="b0685-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-245">Boolean</span></span>|<span data-ttu-id="b0685-246">場合 iMessage、FaceTime の画面が無効になります</span><span class="sxs-lookup"><span data-stu-id="b0685-246">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="b0685-247">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-247">onBoardingScreenDisabled</span></span>|<span data-ttu-id="b0685-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-248">Boolean</span></span>|<span data-ttu-id="b0685-249">契約時のセットアップ画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-249">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="b0685-250">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-250">screenTimeScreenDisabled</span></span>|<span data-ttu-id="b0685-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-251">Boolean</span></span>|<span data-ttu-id="b0685-252">画面のタイムアウトの設定が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-252">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="b0685-253">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-253">simSetupScreenDisabled</span></span>|<span data-ttu-id="b0685-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-254">Boolean</span></span>|<span data-ttu-id="b0685-255">SIMSetup 画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-255">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="b0685-256">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-256">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="b0685-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-257">Boolean</span></span>|<span data-ttu-id="b0685-258">必須のソフトウェアの更新] 画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-258">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="b0685-259">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b0685-259">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="b0685-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0685-260">Boolean</span></span>|<span data-ttu-id="b0685-261">ウォッチ移行] 画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b0685-261">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="b0685-262">応答</span><span class="sxs-lookup"><span data-stu-id="b0685-262">Response</span></span>
<span data-ttu-id="b0685-263">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b0685-263">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0685-264">例</span><span class="sxs-lookup"><span data-stu-id="b0685-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0685-265">要求</span><span class="sxs-lookup"><span data-stu-id="b0685-265">Request</span></span>
<span data-ttu-id="b0685-266">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0685-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1736

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="b0685-267">応答</span><span class="sxs-lookup"><span data-stu-id="b0685-267">Response</span></span>
<span data-ttu-id="b0685-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0685-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1785

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




