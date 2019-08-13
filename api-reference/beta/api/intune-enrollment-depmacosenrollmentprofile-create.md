---
title: DepMacOSEnrollmentProfile を作成する
description: 新しい depMacOSEnrollmentProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f02a4564c0d4ebb1471ea3b967c8afb371080c2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348236"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="06fdc-103">DepMacOSEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="06fdc-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="06fdc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06fdc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06fdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06fdc-106">新しい[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06fdc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="06fdc-107">Prerequisites</span></span>
<span data-ttu-id="06fdc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06fdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fdc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06fdc-110">Permission type</span></span>|<span data-ttu-id="06fdc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="06fdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06fdc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06fdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06fdc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fdc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06fdc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06fdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06fdc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fdc-115">Not supported.</span></span>|
|<span data-ttu-id="06fdc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06fdc-116">Application</span></span>|<span data-ttu-id="06fdc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fdc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06fdc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06fdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="06fdc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06fdc-119">Request headers</span></span>
|<span data-ttu-id="06fdc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06fdc-120">Header</span></span>|<span data-ttu-id="06fdc-121">値</span><span class="sxs-lookup"><span data-stu-id="06fdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06fdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06fdc-122">Authorization</span></span>|<span data-ttu-id="06fdc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="06fdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06fdc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="06fdc-124">Accept</span></span>|<span data-ttu-id="06fdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06fdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06fdc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="06fdc-126">Request body</span></span>
<span data-ttu-id="06fdc-127">要求本文で、depMacOSEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="06fdc-128">次の表に、depMacOSEnrollmentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="06fdc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06fdc-129">Property</span></span>|<span data-ttu-id="06fdc-130">型</span><span class="sxs-lookup"><span data-stu-id="06fdc-130">Type</span></span>|<span data-ttu-id="06fdc-131">説明</span><span class="sxs-lookup"><span data-stu-id="06fdc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fdc-132">id</span><span class="sxs-lookup"><span data-stu-id="06fdc-132">id</span></span>|<span data-ttu-id="06fdc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="06fdc-133">String</span></span>|<span data-ttu-id="06fdc-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="06fdc-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="06fdc-135">displayName</span></span>|<span data-ttu-id="06fdc-136">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-136">String</span></span>|<span data-ttu-id="06fdc-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="06fdc-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-138">description</span><span class="sxs-lookup"><span data-stu-id="06fdc-138">description</span></span>|<span data-ttu-id="06fdc-139">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-139">String</span></span>|<span data-ttu-id="06fdc-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="06fdc-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="06fdc-141">requiresUserAuthentication</span></span>|<span data-ttu-id="06fdc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-142">Boolean</span></span>|<span data-ttu-id="06fdc-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="06fdc-144">configurationEndpointUrl</span></span>|<span data-ttu-id="06fdc-145">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-145">String</span></span>|<span data-ttu-id="06fdc-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="06fdc-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="06fdc-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="06fdc-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-148">Boolean</span></span>|<span data-ttu-id="06fdc-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="06fdc-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="06fdc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="06fdc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-152">Boolean</span></span>|<span data-ttu-id="06fdc-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06fdc-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="06fdc-154">isDefault</span></span>|<span data-ttu-id="06fdc-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="06fdc-155">Boolean</span></span>|<span data-ttu-id="06fdc-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-157">supervisedModeEnabled</span></span>|<span data-ttu-id="06fdc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-158">Boolean</span></span>|<span data-ttu-id="06fdc-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="06fdc-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="06fdc-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06fdc-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="06fdc-161">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="06fdc-162">supportDepartment</span></span>|<span data-ttu-id="06fdc-163">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-163">String</span></span>|<span data-ttu-id="06fdc-164">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="06fdc-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-165">Pass Codedisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-165">passCodeDisabled</span></span>|<span data-ttu-id="06fdc-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-166">Boolean</span></span>|<span data-ttu-id="06fdc-167">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="06fdc-168">isMandatory</span></span>|<span data-ttu-id="06fdc-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-169">Boolean</span></span>|<span data-ttu-id="06fdc-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-171">locationDisabled</span></span>|<span data-ttu-id="06fdc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-172">Boolean</span></span>|<span data-ttu-id="06fdc-173">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="06fdc-174">supportPhoneNumber</span></span>|<span data-ttu-id="06fdc-175">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-175">String</span></span>|<span data-ttu-id="06fdc-176">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="06fdc-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-177">profileRemovalDisabled</span></span>|<span data-ttu-id="06fdc-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-178">Boolean</span></span>|<span data-ttu-id="06fdc-179">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="06fdc-180">restoreBlocked</span></span>|<span data-ttu-id="06fdc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-181">Boolean</span></span>|<span data-ttu-id="06fdc-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-183">りんご Eiddisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-183">appleIdDisabled</span></span>|<span data-ttu-id="06fdc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-184">Boolean</span></span>|<span data-ttu-id="06fdc-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="06fdc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-187">Boolean</span></span>|<span data-ttu-id="06fdc-188">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-189">touchIdDisabled</span></span>|<span data-ttu-id="06fdc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-190">Boolean</span></span>|<span data-ttu-id="06fdc-191">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-192">applePayDisabled</span></span>|<span data-ttu-id="06fdc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-193">Boolean</span></span>|<span data-ttu-id="06fdc-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-195">zoomDisabled</span></span>|<span data-ttu-id="06fdc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-196">Boolean</span></span>|<span data-ttu-id="06fdc-197">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-198">siriDisabled</span></span>|<span data-ttu-id="06fdc-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-199">Boolean</span></span>|<span data-ttu-id="06fdc-200">Siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="06fdc-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-201">diagnosticsDisabled</span></span>|<span data-ttu-id="06fdc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-202">Boolean</span></span>|<span data-ttu-id="06fdc-203">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="06fdc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-205">Boolean</span></span>|<span data-ttu-id="06fdc-206">Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-207">privacyPaneDisabled</span></span>|<span data-ttu-id="06fdc-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-208">Boolean</span></span>|<span data-ttu-id="06fdc-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="06fdc-210">deviceNameTemplate</span></span>|<span data-ttu-id="06fdc-211">String</span><span class="sxs-lookup"><span data-stu-id="06fdc-211">String</span></span>|<span data-ttu-id="06fdc-212">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="06fdc-213">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="06fdc-214">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-214">registrationDisabled</span></span>|<span data-ttu-id="06fdc-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-215">Boolean</span></span>|<span data-ttu-id="06fdc-216">登録が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="06fdc-217">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-217">fileVaultDisabled</span></span>|<span data-ttu-id="06fdc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-218">Boolean</span></span>|<span data-ttu-id="06fdc-219">ファイルボルトが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="06fdc-220">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="06fdc-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-221">Boolean</span></span>|<span data-ttu-id="06fdc-222">ICloud 分析画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="06fdc-223">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="06fdc-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="06fdc-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-224">Boolean</span></span>|<span data-ttu-id="06fdc-225">ICloud ドキュメントとデスクトップ画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="06fdc-226">[Lockscreenを無効にする] を設定します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="06fdc-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdc-227">Boolean</span></span>|<span data-ttu-id="06fdc-228">ICloud ドキュメントとデスクトップ画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="06fdc-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="06fdc-229">応答</span><span class="sxs-lookup"><span data-stu-id="06fdc-229">Response</span></span>
<span data-ttu-id="06fdc-230">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="06fdc-230">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06fdc-231">例</span><span class="sxs-lookup"><span data-stu-id="06fdc-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="06fdc-232">要求</span><span class="sxs-lookup"><span data-stu-id="06fdc-232">Request</span></span>
<span data-ttu-id="06fdc-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06fdc-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1191

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="06fdc-234">応答</span><span class="sxs-lookup"><span data-stu-id="06fdc-234">Response</span></span>
<span data-ttu-id="06fdc-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06fdc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1240

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```






