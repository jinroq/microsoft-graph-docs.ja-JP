---
title: DepIOSEnrollmentProfile を作成する
description: 新しい depIOSEnrollmentProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f18a1e8bba5446a505db7750aa7f238baba13fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908932"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="393b1-103">DepIOSEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="393b1-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="393b1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="393b1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="393b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="393b1-106">新しい[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="393b1-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="393b1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="393b1-107">Prerequisites</span></span>
<span data-ttu-id="393b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="393b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="393b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="393b1-110">Permission type</span></span>|<span data-ttu-id="393b1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="393b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="393b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="393b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="393b1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="393b1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="393b1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="393b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="393b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393b1-115">Not supported.</span></span>|
|<span data-ttu-id="393b1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="393b1-116">Application</span></span>|<span data-ttu-id="393b1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="393b1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="393b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="393b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="393b1-119">Request headers</span></span>
|<span data-ttu-id="393b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="393b1-120">Header</span></span>|<span data-ttu-id="393b1-121">値</span><span class="sxs-lookup"><span data-stu-id="393b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="393b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="393b1-122">Authorization</span></span>|<span data-ttu-id="393b1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="393b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="393b1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="393b1-124">Accept</span></span>|<span data-ttu-id="393b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="393b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="393b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="393b1-126">Request body</span></span>
<span data-ttu-id="393b1-127">要求本文で、depIOSEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="393b1-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="393b1-128">次の表に、depIOSEnrollmentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="393b1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="393b1-129">Property</span></span>|<span data-ttu-id="393b1-130">型</span><span class="sxs-lookup"><span data-stu-id="393b1-130">Type</span></span>|<span data-ttu-id="393b1-131">説明</span><span class="sxs-lookup"><span data-stu-id="393b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393b1-132">id</span><span class="sxs-lookup"><span data-stu-id="393b1-132">id</span></span>|<span data-ttu-id="393b1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="393b1-133">String</span></span>|<span data-ttu-id="393b1-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="393b1-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="393b1-135">displayName</span></span>|<span data-ttu-id="393b1-136">String</span><span class="sxs-lookup"><span data-stu-id="393b1-136">String</span></span>|<span data-ttu-id="393b1-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="393b1-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-138">description</span><span class="sxs-lookup"><span data-stu-id="393b1-138">description</span></span>|<span data-ttu-id="393b1-139">String</span><span class="sxs-lookup"><span data-stu-id="393b1-139">String</span></span>|<span data-ttu-id="393b1-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="393b1-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="393b1-141">requiresUserAuthentication</span></span>|<span data-ttu-id="393b1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-142">Boolean</span></span>|<span data-ttu-id="393b1-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="393b1-144">configurationEndpointUrl</span></span>|<span data-ttu-id="393b1-145">String</span><span class="sxs-lookup"><span data-stu-id="393b1-145">String</span></span>|<span data-ttu-id="393b1-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="393b1-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="393b1-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="393b1-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-148">Boolean</span></span>|<span data-ttu-id="393b1-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="393b1-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="393b1-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="393b1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-152">Boolean</span></span>|<span data-ttu-id="393b1-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="393b1-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="393b1-154">isDefault</span></span>|<span data-ttu-id="393b1-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="393b1-155">Boolean</span></span>|<span data-ttu-id="393b1-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="393b1-157">supervisedModeEnabled</span></span>|<span data-ttu-id="393b1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-158">Boolean</span></span>|<span data-ttu-id="393b1-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="393b1-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="393b1-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="393b1-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="393b1-161">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="393b1-162">supportDepartment</span></span>|<span data-ttu-id="393b1-163">String</span><span class="sxs-lookup"><span data-stu-id="393b1-163">String</span></span>|<span data-ttu-id="393b1-164">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="393b1-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-165">Pass Codedisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-165">passCodeDisabled</span></span>|<span data-ttu-id="393b1-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-166">Boolean</span></span>|<span data-ttu-id="393b1-167">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="393b1-168">isMandatory</span></span>|<span data-ttu-id="393b1-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-169">Boolean</span></span>|<span data-ttu-id="393b1-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-171">locationDisabled</span></span>|<span data-ttu-id="393b1-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-172">Boolean</span></span>|<span data-ttu-id="393b1-173">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="393b1-174">supportPhoneNumber</span></span>|<span data-ttu-id="393b1-175">String</span><span class="sxs-lookup"><span data-stu-id="393b1-175">String</span></span>|<span data-ttu-id="393b1-176">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="393b1-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-177">profileRemovalDisabled</span></span>|<span data-ttu-id="393b1-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-178">Boolean</span></span>|<span data-ttu-id="393b1-179">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="393b1-180">restoreBlocked</span></span>|<span data-ttu-id="393b1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-181">Boolean</span></span>|<span data-ttu-id="393b1-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-183">りんご Eiddisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-183">appleIdDisabled</span></span>|<span data-ttu-id="393b1-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-184">Boolean</span></span>|<span data-ttu-id="393b1-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="393b1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-187">Boolean</span></span>|<span data-ttu-id="393b1-188">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-189">touchIdDisabled</span></span>|<span data-ttu-id="393b1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-190">Boolean</span></span>|<span data-ttu-id="393b1-191">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-192">applePayDisabled</span></span>|<span data-ttu-id="393b1-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-193">Boolean</span></span>|<span data-ttu-id="393b1-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-195">zoomDisabled</span></span>|<span data-ttu-id="393b1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-196">Boolean</span></span>|<span data-ttu-id="393b1-197">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-198">siriDisabled</span></span>|<span data-ttu-id="393b1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-199">Boolean</span></span>|<span data-ttu-id="393b1-200">Siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="393b1-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-201">diagnosticsDisabled</span></span>|<span data-ttu-id="393b1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-202">Boolean</span></span>|<span data-ttu-id="393b1-203">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="393b1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-205">Boolean</span></span>|<span data-ttu-id="393b1-206">Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-207">privacyPaneDisabled</span></span>|<span data-ttu-id="393b1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-208">Boolean</span></span>|<span data-ttu-id="393b1-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="393b1-210">deviceNameTemplate</span></span>|<span data-ttu-id="393b1-211">String</span><span class="sxs-lookup"><span data-stu-id="393b1-211">String</span></span>|<span data-ttu-id="393b1-212">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="393b1-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="393b1-213">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="393b1-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="393b1-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="393b1-214">iTunesPairingMode</span></span>|[<span data-ttu-id="393b1-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="393b1-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="393b1-216">ITunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="393b1-217">可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="393b1-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="393b1-218">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="393b1-218">managementCertificates</span></span>|<span data-ttu-id="393b1-219">[Managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="393b1-220">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="393b1-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="393b1-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="393b1-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-222">Boolean</span></span>|<span data-ttu-id="393b1-223">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="393b1-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="393b1-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="393b1-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-225">Boolean</span></span>|<span data-ttu-id="393b1-226">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="393b1-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="393b1-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="393b1-228">Int32</span><span class="sxs-lookup"><span data-stu-id="393b1-228">Int32</span></span>|<span data-ttu-id="393b1-229">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="393b1-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="393b1-230">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="393b1-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="393b1-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="393b1-231">enableSharedIPad</span></span>|<span data-ttu-id="393b1-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-232">Boolean</span></span>|<span data-ttu-id="393b1-233">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="393b1-234">共有 Ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="393b1-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="393b1-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="393b1-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="393b1-236">String</span><span class="sxs-lookup"><span data-stu-id="393b1-236">String</span></span>|<span data-ttu-id="393b1-237">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="393b1-238">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="393b1-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="393b1-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="393b1-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="393b1-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-240">Boolean</span></span>|<span data-ttu-id="393b1-241">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="393b1-242">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="393b1-242">Default is false.</span></span> <span data-ttu-id="393b1-243">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="393b1-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="393b1-244">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="393b1-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="393b1-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-245">Boolean</span></span>|<span data-ttu-id="393b1-246">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="393b1-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="393b1-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-248">Boolean</span></span>|<span data-ttu-id="393b1-249">IMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="393b1-250">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="393b1-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-251">Boolean</span></span>|<span data-ttu-id="393b1-252">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="393b1-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="393b1-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-254">Boolean</span></span>|<span data-ttu-id="393b1-255">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="393b1-256">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="393b1-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="393b1-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-257">Boolean</span></span>|<span data-ttu-id="393b1-258">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="393b1-259">ソフトウェアの更新 Creendisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="393b1-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-260">Boolean</span></span>|<span data-ttu-id="393b1-261">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="393b1-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="393b1-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="393b1-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-263">Boolean</span></span>|<span data-ttu-id="393b1-264">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="393b1-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="393b1-265">応答</span><span class="sxs-lookup"><span data-stu-id="393b1-265">Response</span></span>
<span data-ttu-id="393b1-266">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="393b1-266">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="393b1-267">例</span><span class="sxs-lookup"><span data-stu-id="393b1-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="393b1-268">要求</span><span class="sxs-lookup"><span data-stu-id="393b1-268">Request</span></span>
<span data-ttu-id="393b1-269">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="393b1-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1791

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
  "deviceNameTemplate": "Device Name Template value",
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

### <a name="response"></a><span data-ttu-id="393b1-270">応答</span><span class="sxs-lookup"><span data-stu-id="393b1-270">Response</span></span>
<span data-ttu-id="393b1-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="393b1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1840

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
  "deviceNameTemplate": "Device Name Template value",
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




