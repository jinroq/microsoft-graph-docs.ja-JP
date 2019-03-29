---
title: depIOSEnrollmentProfile を作成する
description: 新しい depIOSEnrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 446fccbcba1563f17e9de349386544e907b34140
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963724"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="7c79a-103">depIOSEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="7c79a-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="7c79a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c79a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c79a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c79a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c79a-106">新しい[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c79a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c79a-107">Prerequisites</span></span>
<span data-ttu-id="7c79a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c79a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c79a-110">Permission type</span></span>|<span data-ttu-id="7c79a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c79a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c79a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c79a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c79a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c79a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c79a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c79a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c79a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c79a-115">Not supported.</span></span>|
|<span data-ttu-id="7c79a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c79a-116">Application</span></span>|<span data-ttu-id="7c79a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c79a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c79a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c79a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="7c79a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c79a-119">Request headers</span></span>
|<span data-ttu-id="7c79a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c79a-120">Header</span></span>|<span data-ttu-id="7c79a-121">値</span><span class="sxs-lookup"><span data-stu-id="7c79a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c79a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c79a-122">Authorization</span></span>|<span data-ttu-id="7c79a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c79a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c79a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7c79a-124">Accept</span></span>|<span data-ttu-id="7c79a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c79a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c79a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c79a-126">Request body</span></span>
<span data-ttu-id="7c79a-127">要求本文で、depIOSEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="7c79a-128">次の表に、depIOSEnrollmentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="7c79a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c79a-129">Property</span></span>|<span data-ttu-id="7c79a-130">型</span><span class="sxs-lookup"><span data-stu-id="7c79a-130">Type</span></span>|<span data-ttu-id="7c79a-131">説明</span><span class="sxs-lookup"><span data-stu-id="7c79a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c79a-132">id</span><span class="sxs-lookup"><span data-stu-id="7c79a-132">id</span></span>|<span data-ttu-id="7c79a-133">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-133">String</span></span>|<span data-ttu-id="7c79a-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="7c79a-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7c79a-135">displayName</span></span>|<span data-ttu-id="7c79a-136">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-136">String</span></span>|<span data-ttu-id="7c79a-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="7c79a-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-138">description</span><span class="sxs-lookup"><span data-stu-id="7c79a-138">description</span></span>|<span data-ttu-id="7c79a-139">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-139">String</span></span>|<span data-ttu-id="7c79a-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="7c79a-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="7c79a-141">requiresUserAuthentication</span></span>|<span data-ttu-id="7c79a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-142">Boolean</span></span>|<span data-ttu-id="7c79a-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="7c79a-144">configurationEndpointUrl</span></span>|<span data-ttu-id="7c79a-145">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-145">String</span></span>|<span data-ttu-id="7c79a-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="7c79a-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="7c79a-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="7c79a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-148">Boolean</span></span>|<span data-ttu-id="7c79a-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="7c79a-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="7c79a-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="7c79a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-152">Boolean</span></span>|<span data-ttu-id="7c79a-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="7c79a-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="7c79a-154">isDefault</span></span>|<span data-ttu-id="7c79a-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="7c79a-155">Boolean</span></span>|<span data-ttu-id="7c79a-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-157">supervisedModeEnabled</span></span>|<span data-ttu-id="7c79a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-158">Boolean</span></span>|<span data-ttu-id="7c79a-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="7c79a-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="7c79a-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c79a-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="7c79a-161">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="7c79a-162">supportDepartment</span></span>|<span data-ttu-id="7c79a-163">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-163">String</span></span>|<span data-ttu-id="7c79a-164">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="7c79a-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-165">passCodeDisabled</span></span>|<span data-ttu-id="7c79a-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-166">Boolean</span></span>|<span data-ttu-id="7c79a-167">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="7c79a-168">isMandatory</span></span>|<span data-ttu-id="7c79a-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-169">Boolean</span></span>|<span data-ttu-id="7c79a-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-171">locationDisabled</span></span>|<span data-ttu-id="7c79a-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-172">Boolean</span></span>|<span data-ttu-id="7c79a-173">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="7c79a-174">supportPhoneNumber</span></span>|<span data-ttu-id="7c79a-175">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-175">String</span></span>|<span data-ttu-id="7c79a-176">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="7c79a-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-177">profileRemovalDisabled</span></span>|<span data-ttu-id="7c79a-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-178">Boolean</span></span>|<span data-ttu-id="7c79a-179">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-180">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="7c79a-180">restoreBlocked</span></span>|<span data-ttu-id="7c79a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-181">Boolean</span></span>|<span data-ttu-id="7c79a-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-183">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-183">appleIdDisabled</span></span>|<span data-ttu-id="7c79a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-184">Boolean</span></span>|<span data-ttu-id="7c79a-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="7c79a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-187">Boolean</span></span>|<span data-ttu-id="7c79a-188">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-189">touchIdDisabled</span></span>|<span data-ttu-id="7c79a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-190">Boolean</span></span>|<span data-ttu-id="7c79a-191">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-192">applePayDisabled</span></span>|<span data-ttu-id="7c79a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-193">Boolean</span></span>|<span data-ttu-id="7c79a-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-195">zoomDisabled</span></span>|<span data-ttu-id="7c79a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-196">Boolean</span></span>|<span data-ttu-id="7c79a-197">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-198">siridisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-198">siriDisabled</span></span>|<span data-ttu-id="7c79a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-199">Boolean</span></span>|<span data-ttu-id="7c79a-200">siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="7c79a-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-201">diagnosticsDisabled</span></span>|<span data-ttu-id="7c79a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-202">Boolean</span></span>|<span data-ttu-id="7c79a-203">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="7c79a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-205">Boolean</span></span>|<span data-ttu-id="7c79a-206">displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-207">privacyPaneDisabled</span></span>|<span data-ttu-id="7c79a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-208">Boolean</span></span>|<span data-ttu-id="7c79a-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="7c79a-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="7c79a-210">iTunesPairingMode</span></span>|[<span data-ttu-id="7c79a-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="7c79a-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="7c79a-212">iTunes ペアリングモードを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="7c79a-213">使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="7c79a-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="7c79a-214">managementcertificates</span><span class="sxs-lookup"><span data-stu-id="7c79a-214">managementCertificates</span></span>|<span data-ttu-id="7c79a-215">[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7c79a-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="7c79a-216">Apple Configurator の管理証明書</span><span class="sxs-lookup"><span data-stu-id="7c79a-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="7c79a-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="7c79a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-218">Boolean</span></span>|<span data-ttu-id="7c79a-219">Android からの復元が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="7c79a-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="7c79a-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="7c79a-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-221">Boolean</span></span>|<span data-ttu-id="7c79a-222">構成済みの確認をデバイスが待機する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="7c79a-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="7c79a-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="7c79a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="7c79a-224">Int32</span></span>|<span data-ttu-id="7c79a-225">これにより、共有 iPad を使用できるユーザーの最大数が指定されます。</span><span class="sxs-lookup"><span data-stu-id="7c79a-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="7c79a-226">共有 iPad モードでのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7c79a-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="7c79a-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="7c79a-227">enableSharedIPad</span></span>|<span data-ttu-id="7c79a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-228">Boolean</span></span>|<span data-ttu-id="7c79a-229">これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="7c79a-230">共有 ipad にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7c79a-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="7c79a-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="7c79a-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="7c79a-232">String</span><span class="sxs-lookup"><span data-stu-id="7c79a-232">String</span></span>|<span data-ttu-id="7c79a-233">設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="7c79a-234">このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c79a-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="7c79a-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="7c79a-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="7c79a-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-236">Boolean</span></span>|<span data-ttu-id="7c79a-237">デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="7c79a-238">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="7c79a-238">Default is false.</span></span> <span data-ttu-id="7c79a-239">このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c79a-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="7c79a-240">ホームボタンの無効化</span><span class="sxs-lookup"><span data-stu-id="7c79a-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="7c79a-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-241">Boolean</span></span>|<span data-ttu-id="7c79a-242">[ホームボタンの感度] 画面を無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="7c79a-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="7c79a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-244">Boolean</span></span>|<span data-ttu-id="7c79a-245">iMessage および FaceTime の画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="7c79a-246">onboardingscreendisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="7c79a-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-247">Boolean</span></span>|<span data-ttu-id="7c79a-248">オンボードのセットアップ画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="7c79a-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="7c79a-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-250">Boolean</span></span>|<span data-ttu-id="7c79a-251">画面のタイムアウト設定を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="7c79a-252">シムの設定を無効にする</span><span class="sxs-lookup"><span data-stu-id="7c79a-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="7c79a-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-253">Boolean</span></span>|<span data-ttu-id="7c79a-254">[シム] セットアップ画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="7c79a-255">ソフトウェアの更新 creendisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="7c79a-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-256">Boolean</span></span>|<span data-ttu-id="7c79a-257">必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="7c79a-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="7c79a-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="7c79a-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c79a-259">Boolean</span></span>|<span data-ttu-id="7c79a-260">[移行の監視] 画面が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7c79a-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="7c79a-261">応答</span><span class="sxs-lookup"><span data-stu-id="7c79a-261">Response</span></span>
<span data-ttu-id="7c79a-262">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c79a-262">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c79a-263">例</span><span class="sxs-lookup"><span data-stu-id="7c79a-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c79a-264">要求</span><span class="sxs-lookup"><span data-stu-id="7c79a-264">Request</span></span>
<span data-ttu-id="7c79a-265">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c79a-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="7c79a-266">応答</span><span class="sxs-lookup"><span data-stu-id="7c79a-266">Response</span></span>
<span data-ttu-id="7c79a-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c79a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




