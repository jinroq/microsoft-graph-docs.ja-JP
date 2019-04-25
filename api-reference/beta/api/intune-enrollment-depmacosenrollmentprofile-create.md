---
title: depMacOSEnrollmentProfile を作成する
description: 新しい depMacOSEnrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 845f6af654b43140ec616267a4ce32e1b6a8c45e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534018"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="1fcab-103">depMacOSEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="1fcab-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="1fcab-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fcab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fcab-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1fcab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fcab-106">新しい[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fcab-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1fcab-107">Prerequisites</span></span>
<span data-ttu-id="1fcab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1fcab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fcab-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1fcab-110">Permission type</span></span>|<span data-ttu-id="1fcab-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1fcab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fcab-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1fcab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fcab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fcab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1fcab-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1fcab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fcab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fcab-115">Not supported.</span></span>|
|<span data-ttu-id="1fcab-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1fcab-116">Application</span></span>|<span data-ttu-id="1fcab-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fcab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fcab-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1fcab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1fcab-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fcab-119">Request headers</span></span>
|<span data-ttu-id="1fcab-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fcab-120">Header</span></span>|<span data-ttu-id="1fcab-121">値</span><span class="sxs-lookup"><span data-stu-id="1fcab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fcab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fcab-122">Authorization</span></span>|<span data-ttu-id="1fcab-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1fcab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fcab-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1fcab-124">Accept</span></span>|<span data-ttu-id="1fcab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fcab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fcab-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1fcab-126">Request body</span></span>
<span data-ttu-id="1fcab-127">要求本文で、depMacOSEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="1fcab-128">次の表に、depMacOSEnrollmentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="1fcab-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fcab-129">Property</span></span>|<span data-ttu-id="1fcab-130">型</span><span class="sxs-lookup"><span data-stu-id="1fcab-130">Type</span></span>|<span data-ttu-id="1fcab-131">説明</span><span class="sxs-lookup"><span data-stu-id="1fcab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fcab-132">id</span><span class="sxs-lookup"><span data-stu-id="1fcab-132">id</span></span>|<span data-ttu-id="1fcab-133">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-133">String</span></span>|<span data-ttu-id="1fcab-134">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="1fcab-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1fcab-135">displayName</span></span>|<span data-ttu-id="1fcab-136">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-136">String</span></span>|<span data-ttu-id="1fcab-137">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="1fcab-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-138">description</span><span class="sxs-lookup"><span data-stu-id="1fcab-138">description</span></span>|<span data-ttu-id="1fcab-139">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-139">String</span></span>|<span data-ttu-id="1fcab-140">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="1fcab-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="1fcab-141">requiresUserAuthentication</span></span>|<span data-ttu-id="1fcab-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-142">Boolean</span></span>|<span data-ttu-id="1fcab-143">プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-144">configurationendpointurl</span><span class="sxs-lookup"><span data-stu-id="1fcab-144">configurationEndpointUrl</span></span>|<span data-ttu-id="1fcab-145">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-145">String</span></span>|<span data-ttu-id="1fcab-146">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="1fcab-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="1fcab-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1fcab-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-148">Boolean</span></span>|<span data-ttu-id="1fcab-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1fcab-150">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="1fcab-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="1fcab-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-152">Boolean</span></span>|<span data-ttu-id="1fcab-153">[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fcab-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="1fcab-154">isDefault</span></span>|<span data-ttu-id="1fcab-155">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1fcab-155">Boolean</span></span>|<span data-ttu-id="1fcab-156">これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-157">supervisedModeEnabled</span></span>|<span data-ttu-id="1fcab-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-158">Boolean</span></span>|<span data-ttu-id="1fcab-159">監視モード、有効にする場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="1fcab-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1fcab-160">詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1fcab-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="1fcab-161">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-162">supportdepartment</span><span class="sxs-lookup"><span data-stu-id="1fcab-162">supportDepartment</span></span>|<span data-ttu-id="1fcab-163">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-163">String</span></span>|<span data-ttu-id="1fcab-164">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報</span><span class="sxs-lookup"><span data-stu-id="1fcab-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-165">pass codedisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-165">passCodeDisabled</span></span>|<span data-ttu-id="1fcab-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-166">Boolean</span></span>|<span data-ttu-id="1fcab-167">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-168">ismandatory</span><span class="sxs-lookup"><span data-stu-id="1fcab-168">isMandatory</span></span>|<span data-ttu-id="1fcab-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-169">Boolean</span></span>|<span data-ttu-id="1fcab-170">プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-171">locationdisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-171">locationDisabled</span></span>|<span data-ttu-id="1fcab-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-172">Boolean</span></span>|<span data-ttu-id="1fcab-173">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1fcab-174">supportPhoneNumber</span></span>|<span data-ttu-id="1fcab-175">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-175">String</span></span>|<span data-ttu-id="1fcab-176">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号</span><span class="sxs-lookup"><span data-stu-id="1fcab-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-177">profileRemovalDisabled</span></span>|<span data-ttu-id="1fcab-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-178">Boolean</span></span>|<span data-ttu-id="1fcab-179">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-180">restoreblocked</span><span class="sxs-lookup"><span data-stu-id="1fcab-180">restoreBlocked</span></span>|<span data-ttu-id="1fcab-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-181">Boolean</span></span>|<span data-ttu-id="1fcab-182">復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-183">りんご eiddisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-183">appleIdDisabled</span></span>|<span data-ttu-id="1fcab-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-184">Boolean</span></span>|<span data-ttu-id="1fcab-185">Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1fcab-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-187">Boolean</span></span>|<span data-ttu-id="1fcab-188">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-189">touchIdDisabled</span></span>|<span data-ttu-id="1fcab-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-190">Boolean</span></span>|<span data-ttu-id="1fcab-191">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-192">applePayDisabled</span></span>|<span data-ttu-id="1fcab-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-193">Boolean</span></span>|<span data-ttu-id="1fcab-194">Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-195">zoomDisabled</span></span>|<span data-ttu-id="1fcab-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-196">Boolean</span></span>|<span data-ttu-id="1fcab-197">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-198">siridisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-198">siriDisabled</span></span>|<span data-ttu-id="1fcab-199">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-199">Boolean</span></span>|<span data-ttu-id="1fcab-200">siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="1fcab-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-201">diagnosticsDisabled</span></span>|<span data-ttu-id="1fcab-202">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-202">Boolean</span></span>|<span data-ttu-id="1fcab-203">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="1fcab-205">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-205">Boolean</span></span>|<span data-ttu-id="1fcab-206">displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-207">privacyPaneDisabled</span></span>|<span data-ttu-id="1fcab-208">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-208">Boolean</span></span>|<span data-ttu-id="1fcab-209">プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="1fcab-210">deviceNameTemplate</span></span>|<span data-ttu-id="1fcab-211">String</span><span class="sxs-lookup"><span data-stu-id="1fcab-211">String</span></span>|<span data-ttu-id="1fcab-212">リテラルまたは名前のパターンを設定します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="1fcab-213">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1fcab-214">registrationdisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-214">registrationDisabled</span></span>|<span data-ttu-id="1fcab-215">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-215">Boolean</span></span>|<span data-ttu-id="1fcab-216">登録が無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="1fcab-217">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-217">fileVaultDisabled</span></span>|<span data-ttu-id="1fcab-218">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-218">Boolean</span></span>|<span data-ttu-id="1fcab-219">ファイルボルトが無効であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="1fcab-220">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="1fcab-221">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-221">Boolean</span></span>|<span data-ttu-id="1fcab-222">iCloud 分析画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="1fcab-223">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="1fcab-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="1fcab-224">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-224">Boolean</span></span>|<span data-ttu-id="1fcab-225">iCloud ドキュメントとデスクトップ画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="1fcab-226">[lockscreenを無効にする] を設定します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="1fcab-227">ブール値</span><span class="sxs-lookup"><span data-stu-id="1fcab-227">Boolean</span></span>|<span data-ttu-id="1fcab-228">iCloud ドキュメントとデスクトップ画面が無効かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="1fcab-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="1fcab-229">応答</span><span class="sxs-lookup"><span data-stu-id="1fcab-229">Response</span></span>
<span data-ttu-id="1fcab-230">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1fcab-230">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fcab-231">例</span><span class="sxs-lookup"><span data-stu-id="1fcab-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fcab-232">要求</span><span class="sxs-lookup"><span data-stu-id="1fcab-232">Request</span></span>
<span data-ttu-id="1fcab-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1fcab-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1fcab-234">応答</span><span class="sxs-lookup"><span data-stu-id="1fcab-234">Response</span></span>
<span data-ttu-id="1fcab-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1fcab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





