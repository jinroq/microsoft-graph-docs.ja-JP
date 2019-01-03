---
title: DepIOSEnrollmentProfile を更新します。
description: DepIOSEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 4c492955c17e20948b6088e8f87ed260bf6b07fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358640"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="742f4-103">DepIOSEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="742f4-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="742f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="742f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="742f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="742f4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="742f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="742f4-107">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="742f4-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="742f4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="742f4-108">Prerequisites</span></span>
<span data-ttu-id="742f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="742f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="742f4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="742f4-111">Permission type</span></span>|<span data-ttu-id="742f4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="742f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="742f4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="742f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="742f4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="742f4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="742f4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="742f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="742f4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742f4-116">Not supported.</span></span>|
|<span data-ttu-id="742f4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="742f4-117">Application</span></span>|<span data-ttu-id="742f4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="742f4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="742f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="742f4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="742f4-120">Request headers</span></span>
|<span data-ttu-id="742f4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="742f4-121">Header</span></span>|<span data-ttu-id="742f4-122">値</span><span class="sxs-lookup"><span data-stu-id="742f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="742f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="742f4-123">Authorization</span></span>|<span data-ttu-id="742f4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="742f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="742f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="742f4-125">Accept</span></span>|<span data-ttu-id="742f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="742f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="742f4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="742f4-127">Request body</span></span>
<span data-ttu-id="742f4-128">要求の本文に[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="742f4-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="742f4-129">[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="742f4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="742f4-130">Property</span></span>|<span data-ttu-id="742f4-131">種類</span><span class="sxs-lookup"><span data-stu-id="742f4-131">Type</span></span>|<span data-ttu-id="742f4-132">説明</span><span class="sxs-lookup"><span data-stu-id="742f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="742f4-133">ID</span><span class="sxs-lookup"><span data-stu-id="742f4-133">id</span></span>|<span data-ttu-id="742f4-134">String</span><span class="sxs-lookup"><span data-stu-id="742f4-134">String</span></span>|<span data-ttu-id="742f4-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="742f4-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="742f4-136">displayName</span></span>|<span data-ttu-id="742f4-137">String</span><span class="sxs-lookup"><span data-stu-id="742f4-137">String</span></span>|<span data-ttu-id="742f4-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="742f4-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-139">説明</span><span class="sxs-lookup"><span data-stu-id="742f4-139">description</span></span>|<span data-ttu-id="742f4-140">String</span><span class="sxs-lookup"><span data-stu-id="742f4-140">String</span></span>|<span data-ttu-id="742f4-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="742f4-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="742f4-142">requiresUserAuthentication</span></span>|<span data-ttu-id="742f4-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-143">Boolean</span></span>|<span data-ttu-id="742f4-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="742f4-145">configurationEndpointUrl</span></span>|<span data-ttu-id="742f4-146">String</span><span class="sxs-lookup"><span data-stu-id="742f4-146">String</span></span>|<span data-ttu-id="742f4-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="742f4-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="742f4-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="742f4-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-149">Boolean</span></span>|<span data-ttu-id="742f4-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="742f4-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="742f4-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="742f4-152">isDefault</span></span>|<span data-ttu-id="742f4-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-153">Boolean</span></span>|<span data-ttu-id="742f4-154">これは、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承される既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="742f4-155">supervisedModeEnabled</span></span>|<span data-ttu-id="742f4-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-156">Boolean</span></span>|<span data-ttu-id="742f4-157">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="742f4-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="742f4-158">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="742f4-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="742f4-159">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="742f4-160">supportDepartment</span></span>|<span data-ttu-id="742f4-161">String</span><span class="sxs-lookup"><span data-stu-id="742f4-161">String</span></span>|<span data-ttu-id="742f4-162">継承のサポート部門については、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="742f4-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-163">passCodeDisabled</span></span>|<span data-ttu-id="742f4-164">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-164">Boolean</span></span>|<span data-ttu-id="742f4-165">パスコードの設定] ウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="742f4-166">isMandatory</span></span>|<span data-ttu-id="742f4-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-167">Boolean</span></span>|<span data-ttu-id="742f4-168">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承が必須であるかを示す</span><span class="sxs-lookup"><span data-stu-id="742f4-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-169">locationDisabled</span></span>|<span data-ttu-id="742f4-170">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-170">Boolean</span></span>|<span data-ttu-id="742f4-171">サービス セットアップ] ウィンドウの場所が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="742f4-172">supportPhoneNumber</span></span>|<span data-ttu-id="742f4-173">String</span><span class="sxs-lookup"><span data-stu-id="742f4-173">String</span></span>|<span data-ttu-id="742f4-174">継承のサポート電話番号は、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="742f4-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-175">profileRemovalDisabled</span></span>|<span data-ttu-id="742f4-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-176">Boolean</span></span>|<span data-ttu-id="742f4-177">プロファイルの削除オプションが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="742f4-178">restoreBlocked</span></span>|<span data-ttu-id="742f4-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-179">Boolean</span></span>|<span data-ttu-id="742f4-180">復元の設定] ウィンドウがブロックされていることを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-181">appleIdDisabled</span></span>|<span data-ttu-id="742f4-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-182">Boolean</span></span>|<span data-ttu-id="742f4-183">Id の設定] ウィンドウは、Apple が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="742f4-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-185">Boolean</span></span>|<span data-ttu-id="742f4-186">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-187">touchIdDisabled</span></span>|<span data-ttu-id="742f4-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-188">Boolean</span></span>|<span data-ttu-id="742f4-189">タッチ id の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-190">applePayDisabled</span></span>|<span data-ttu-id="742f4-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-191">Boolean</span></span>|<span data-ttu-id="742f4-192">アップル支払設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-193">zoomDisabled</span></span>|<span data-ttu-id="742f4-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-194">Boolean</span></span>|<span data-ttu-id="742f4-195">ズームの設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-196">siriDisabled</span></span>|<span data-ttu-id="742f4-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-197">Boolean</span></span>|<span data-ttu-id="742f4-198">Siri の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="742f4-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-199">diagnosticsDisabled</span></span>|<span data-ttu-id="742f4-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-200">Boolean</span></span>|<span data-ttu-id="742f4-201">設定] ウィンドウは、診断が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="742f4-202">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="742f4-202">iTunesPairingMode</span></span>|[<span data-ttu-id="742f4-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="742f4-203">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="742f4-204">ITunes のペアリング モードを示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="742f4-205">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="742f4-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="742f4-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="742f4-206">managementCertificates</span></span>|<span data-ttu-id="742f4-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="742f4-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="742f4-208">Apple Configurator の証明書を管理</span><span class="sxs-lookup"><span data-stu-id="742f4-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="742f4-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="742f4-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="742f4-210">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-210">Boolean</span></span>|<span data-ttu-id="742f4-211">Android からの復元が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="742f4-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="742f4-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="742f4-213">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-213">Boolean</span></span>|<span data-ttu-id="742f4-214">デバイスが構成されている確認メッセージを待機する必要がかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="742f4-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="742f4-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="742f4-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="742f4-216">Int32</span><span class="sxs-lookup"><span data-stu-id="742f4-216">Int32</span></span>|<span data-ttu-id="742f4-217">共有の iPad を使用できるユーザーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="742f4-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="742f4-218">IPad を共有モードでのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="742f4-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="742f4-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="742f4-219">enableSharedIPad</span></span>|<span data-ttu-id="742f4-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-220">Boolean</span></span>|<span data-ttu-id="742f4-221">これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="742f4-222">共有台もの Ipad でのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="742f4-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="742f4-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="742f4-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="742f4-224">String</span><span class="sxs-lookup"><span data-stu-id="742f4-224">String</span></span>|<span data-ttu-id="742f4-225">場合設定、デバイスのライセンスと企業ポータルを展開するどの Vpp トークンを使用する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="742f4-226">'enableAuthenticationViaCompanyPortal' は、このプロパティを設定するために設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="742f4-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="742f4-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="742f4-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="742f4-228">ブール型</span><span class="sxs-lookup"><span data-stu-id="742f4-228">Boolean</span></span>|<span data-ttu-id="742f4-229">1 つのアプリケーション モードを有効にして、登録時にアプリケーション ロックを適用するデバイスを指示します。</span><span class="sxs-lookup"><span data-stu-id="742f4-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="742f4-230">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="742f4-230">Default is false.</span></span> <span data-ttu-id="742f4-231">'enableAuthenticationViaCompanyPortal' と 'companyPortalVppTokenId' は、このプロパティを設定するのに設定してください。</span><span class="sxs-lookup"><span data-stu-id="742f4-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="742f4-232">応答</span><span class="sxs-lookup"><span data-stu-id="742f4-232">Response</span></span>
<span data-ttu-id="742f4-233">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="742f4-233">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="742f4-234">例</span><span class="sxs-lookup"><span data-stu-id="742f4-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="742f4-235">要求</span><span class="sxs-lookup"><span data-stu-id="742f4-235">Request</span></span>
<span data-ttu-id="742f4-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="742f4-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1267

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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
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
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a><span data-ttu-id="742f4-237">応答</span><span class="sxs-lookup"><span data-stu-id="742f4-237">Response</span></span>
<span data-ttu-id="742f4-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="742f4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
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
  "enableSingleAppEnrollmentMode": true
}
```




