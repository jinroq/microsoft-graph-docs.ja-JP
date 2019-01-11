---
title: DepMacOSEnrollmentProfile を作成します。
description: 新しい depMacOSEnrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e17a5798f35301691c0f475866d8ffe06cd020d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807050"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="5f3cd-103">DepMacOSEnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="5f3cd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f3cd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f3cd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f3cd-107">新しい[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f3cd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f3cd-108">Prerequisites</span></span>
<span data-ttu-id="5f3cd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f3cd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f3cd-111">Permission type</span></span>|<span data-ttu-id="5f3cd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f3cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f3cd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f3cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f3cd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f3cd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f3cd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f3cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f3cd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-116">Not supported.</span></span>|
|<span data-ttu-id="5f3cd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f3cd-117">Application</span></span>|<span data-ttu-id="5f3cd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f3cd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f3cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5f3cd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f3cd-120">Request headers</span></span>
|<span data-ttu-id="5f3cd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f3cd-121">Header</span></span>|<span data-ttu-id="5f3cd-122">値</span><span class="sxs-lookup"><span data-stu-id="5f3cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f3cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f3cd-123">Authorization</span></span>|<span data-ttu-id="5f3cd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f3cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f3cd-125">Accept</span></span>|<span data-ttu-id="5f3cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f3cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f3cd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f3cd-127">Request body</span></span>
<span data-ttu-id="5f3cd-128">要求の本文に depMacOSEnrollmentProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="5f3cd-129">次の表は、depMacOSEnrollmentProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="5f3cd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3cd-130">Property</span></span>|<span data-ttu-id="5f3cd-131">種類</span><span class="sxs-lookup"><span data-stu-id="5f3cd-131">Type</span></span>|<span data-ttu-id="5f3cd-132">説明</span><span class="sxs-lookup"><span data-stu-id="5f3cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f3cd-133">ID</span><span class="sxs-lookup"><span data-stu-id="5f3cd-133">id</span></span>|<span data-ttu-id="5f3cd-134">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-134">String</span></span>|<span data-ttu-id="5f3cd-135">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="5f3cd-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5f3cd-136">displayName</span></span>|<span data-ttu-id="5f3cd-137">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-137">String</span></span>|<span data-ttu-id="5f3cd-138">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="5f3cd-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-139">説明</span><span class="sxs-lookup"><span data-stu-id="5f3cd-139">description</span></span>|<span data-ttu-id="5f3cd-140">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-140">String</span></span>|<span data-ttu-id="5f3cd-141">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="5f3cd-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="5f3cd-142">requiresUserAuthentication</span></span>|<span data-ttu-id="5f3cd-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-143">Boolean</span></span>|<span data-ttu-id="5f3cd-144">プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="5f3cd-145">configurationEndpointUrl</span></span>|<span data-ttu-id="5f3cd-146">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-146">String</span></span>|<span data-ttu-id="5f3cd-147">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="5f3cd-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="5f3cd-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="5f3cd-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-149">Boolean</span></span>|<span data-ttu-id="5f3cd-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="5f3cd-151">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="5f3cd-152">isDefault</span></span>|<span data-ttu-id="5f3cd-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-153">Boolean</span></span>|<span data-ttu-id="5f3cd-154">これは、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承される既定のプロファイルであるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-155">supervisedModeEnabled</span></span>|<span data-ttu-id="5f3cd-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-156">Boolean</span></span>|<span data-ttu-id="5f3cd-157">コールを管理モードを有効にする、false それ以外の場合は True です。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="5f3cd-158">参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="5f3cd-159">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="5f3cd-160">supportDepartment</span></span>|<span data-ttu-id="5f3cd-161">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-161">String</span></span>|<span data-ttu-id="5f3cd-162">継承のサポート部門については、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="5f3cd-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-163">passCodeDisabled</span></span>|<span data-ttu-id="5f3cd-164">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-164">Boolean</span></span>|<span data-ttu-id="5f3cd-165">パスコードの設定] ウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="5f3cd-166">isMandatory</span></span>|<span data-ttu-id="5f3cd-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-167">Boolean</span></span>|<span data-ttu-id="5f3cd-168">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承が必須であるかを示す</span><span class="sxs-lookup"><span data-stu-id="5f3cd-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-169">locationDisabled</span></span>|<span data-ttu-id="5f3cd-170">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-170">Boolean</span></span>|<span data-ttu-id="5f3cd-171">サービス セットアップ] ウィンドウの場所が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5f3cd-172">supportPhoneNumber</span></span>|<span data-ttu-id="5f3cd-173">String</span><span class="sxs-lookup"><span data-stu-id="5f3cd-173">String</span></span>|<span data-ttu-id="5f3cd-174">継承のサポート電話番号は、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="5f3cd-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-175">profileRemovalDisabled</span></span>|<span data-ttu-id="5f3cd-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-176">Boolean</span></span>|<span data-ttu-id="5f3cd-177">プロファイルの削除オプションが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5f3cd-178">restoreBlocked</span></span>|<span data-ttu-id="5f3cd-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-179">Boolean</span></span>|<span data-ttu-id="5f3cd-180">復元の設定] ウィンドウがブロックされていることを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-181">appleIdDisabled</span></span>|<span data-ttu-id="5f3cd-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-182">Boolean</span></span>|<span data-ttu-id="5f3cd-183">Id の設定] ウィンドウは、Apple が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="5f3cd-185">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-185">Boolean</span></span>|<span data-ttu-id="5f3cd-186">'条項および条件' の設定ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-187">touchIdDisabled</span></span>|<span data-ttu-id="5f3cd-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-188">Boolean</span></span>|<span data-ttu-id="5f3cd-189">タッチ id の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-190">applePayDisabled</span></span>|<span data-ttu-id="5f3cd-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-191">Boolean</span></span>|<span data-ttu-id="5f3cd-192">アップル支払設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-193">zoomDisabled</span></span>|<span data-ttu-id="5f3cd-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-194">Boolean</span></span>|<span data-ttu-id="5f3cd-195">ズームの設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-196">siriDisabled</span></span>|<span data-ttu-id="5f3cd-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-197">Boolean</span></span>|<span data-ttu-id="5f3cd-198">Siri の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-199">diagnosticsDisabled</span></span>|<span data-ttu-id="5f3cd-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-200">Boolean</span></span>|<span data-ttu-id="5f3cd-201">設定] ウィンドウは、診断が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="5f3cd-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-202">registrationDisabled</span></span>|<span data-ttu-id="5f3cd-203">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-203">Boolean</span></span>|<span data-ttu-id="5f3cd-204">登録が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="5f3cd-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-205">fileVaultDisabled</span></span>|<span data-ttu-id="5f3cd-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-206">Boolean</span></span>|<span data-ttu-id="5f3cd-207">ファイルボルトが無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="5f3cd-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5f3cd-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="5f3cd-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="5f3cd-209">Boolean</span></span>|<span data-ttu-id="5f3cd-210">ICloud 分析画面が無効になっているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="5f3cd-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="5f3cd-211">応答</span><span class="sxs-lookup"><span data-stu-id="5f3cd-211">Response</span></span>
<span data-ttu-id="5f3cd-212">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-212">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f3cd-213">例</span><span class="sxs-lookup"><span data-stu-id="5f3cd-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f3cd-214">要求</span><span class="sxs-lookup"><span data-stu-id="5f3cd-214">Request</span></span>
<span data-ttu-id="5f3cd-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="5f3cd-216">応答</span><span class="sxs-lookup"><span data-stu-id="5f3cd-216">Response</span></span>
<span data-ttu-id="5f3cd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f3cd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```





