---
title: IntuneBrandingProfile を作成する
description: 新しい intuneBrandingProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98245e618ef6c821502109164e2c726657477b91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350182"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="05b4b-103">IntuneBrandingProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="05b4b-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="05b4b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05b4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05b4b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05b4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b4b-106">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05b4b-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05b4b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="05b4b-107">Prerequisites</span></span>
<span data-ttu-id="05b4b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05b4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b4b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05b4b-110">Permission type</span></span>|<span data-ttu-id="05b4b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05b4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05b4b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05b4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05b4b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b4b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05b4b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05b4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05b4b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05b4b-115">Not supported.</span></span>|
|<span data-ttu-id="05b4b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05b4b-116">Application</span></span>|<span data-ttu-id="05b4b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b4b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05b4b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05b4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="05b4b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05b4b-119">Request headers</span></span>
|<span data-ttu-id="05b4b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05b4b-120">Header</span></span>|<span data-ttu-id="05b4b-121">値</span><span class="sxs-lookup"><span data-stu-id="05b4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05b4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05b4b-122">Authorization</span></span>|<span data-ttu-id="05b4b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="05b4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05b4b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="05b4b-124">Accept</span></span>|<span data-ttu-id="05b4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05b4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05b4b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="05b4b-126">Request body</span></span>
<span data-ttu-id="05b4b-127">要求本文で、intuneBrandingProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05b4b-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="05b4b-128">次の表に、intuneBrandingProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05b4b-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="05b4b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05b4b-129">Property</span></span>|<span data-ttu-id="05b4b-130">型</span><span class="sxs-lookup"><span data-stu-id="05b4b-130">Type</span></span>|<span data-ttu-id="05b4b-131">説明</span><span class="sxs-lookup"><span data-stu-id="05b4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b4b-132">id</span><span class="sxs-lookup"><span data-stu-id="05b4b-132">id</span></span>|<span data-ttu-id="05b4b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="05b4b-133">String</span></span>|<span data-ttu-id="05b4b-134">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="05b4b-134">Profile Key</span></span>|
|<span data-ttu-id="05b4b-135">profileName</span><span class="sxs-lookup"><span data-stu-id="05b4b-135">profileName</span></span>|<span data-ttu-id="05b4b-136">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-136">String</span></span>|<span data-ttu-id="05b4b-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="05b4b-137">Name of the profile</span></span>|
|<span data-ttu-id="05b4b-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="05b4b-138">profileDescription</span></span>|<span data-ttu-id="05b4b-139">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-139">String</span></span>|<span data-ttu-id="05b4b-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="05b4b-140">Description of the profile</span></span>|
|<span data-ttu-id="05b4b-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="05b4b-141">isDefaultProfile</span></span>|<span data-ttu-id="05b4b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b4b-142">Boolean</span></span>|<span data-ttu-id="05b4b-143">プロファイルが既定として使用されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="05b4b-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="05b4b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05b4b-144">createdDateTime</span></span>|<span data-ttu-id="05b4b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b4b-145">DateTimeOffset</span></span>|<span data-ttu-id="05b4b-146">BrandingProfile が作成された時刻</span><span class="sxs-lookup"><span data-stu-id="05b4b-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="05b4b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05b4b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="05b4b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b4b-148">DateTimeOffset</span></span>|<span data-ttu-id="05b4b-149">BrandingProfile が最後に変更された時刻</span><span class="sxs-lookup"><span data-stu-id="05b4b-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="05b4b-150">displayName</span><span class="sxs-lookup"><span data-stu-id="05b4b-150">displayName</span></span>|<span data-ttu-id="05b4b-151">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-151">String</span></span>|<span data-ttu-id="05b4b-152">エンドユーザーに表示される会社名または組織名</span><span class="sxs-lookup"><span data-stu-id="05b4b-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="05b4b-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="05b4b-153">contactITName</span></span>|<span data-ttu-id="05b4b-154">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-154">String</span></span>|<span data-ttu-id="05b4b-155">IT サポートを担当する個人または組織の名前</span><span class="sxs-lookup"><span data-stu-id="05b4b-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="05b4b-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="05b4b-156">contactITPhoneNumber</span></span>|<span data-ttu-id="05b4b-157">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-157">String</span></span>|<span data-ttu-id="05b4b-158">IT サポートを担当する個人または組織の電話番号</span><span class="sxs-lookup"><span data-stu-id="05b4b-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="05b4b-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="05b4b-159">contactITEmailAddress</span></span>|<span data-ttu-id="05b4b-160">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-160">String</span></span>|<span data-ttu-id="05b4b-161">IT サポートを担当する個人または組織の電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="05b4b-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="05b4b-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="05b4b-162">contactITNotes</span></span>|<span data-ttu-id="05b4b-163">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-163">String</span></span>|<span data-ttu-id="05b4b-164">IT サポートを担当する個人または組織に関するテキストコメント</span><span class="sxs-lookup"><span data-stu-id="05b4b-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="05b4b-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="05b4b-165">privacyUrl</span></span>|<span data-ttu-id="05b4b-166">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-166">String</span></span>|<span data-ttu-id="05b4b-167">会社/組織のプライバシーポリシーの URL</span><span class="sxs-lookup"><span data-stu-id="05b4b-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="05b4b-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="05b4b-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="05b4b-169">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-169">String</span></span>|<span data-ttu-id="05b4b-170">会社または組織の IT ヘルプデスクサイトへの URL</span><span class="sxs-lookup"><span data-stu-id="05b4b-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="05b4b-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="05b4b-171">onlineSupportSiteName</span></span>|<span data-ttu-id="05b4b-172">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-172">String</span></span>|<span data-ttu-id="05b4b-173">会社/組織の IT ヘルプデスクサイトの表示名</span><span class="sxs-lookup"><span data-stu-id="05b4b-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="05b4b-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="05b4b-174">themeColor</span></span>|[<span data-ttu-id="05b4b-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="05b4b-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="05b4b-176">会社のポータルアプリケーションと web ポータルで使用される主要なテーマの色</span><span class="sxs-lookup"><span data-stu-id="05b4b-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="05b4b-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="05b4b-177">showLogo</span></span>|<span data-ttu-id="05b4b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b4b-178">Boolean</span></span>|<span data-ttu-id="05b4b-179">管理者が指定したロゴ画像が表示されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="05b4b-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="05b4b-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="05b4b-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="05b4b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b4b-181">Boolean</span></span>|<span data-ttu-id="05b4b-182">管理者が指定した表示名がロゴ画像の隣に表示されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="05b4b-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="05b4b-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="05b4b-183">themeColorLogo</span></span>|[<span data-ttu-id="05b4b-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05b4b-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05b4b-185">ロゴの背景色がテーマになっている、ポータルサイトアプリに表示されるロゴ画像</span><span class="sxs-lookup"><span data-stu-id="05b4b-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="05b4b-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="05b4b-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="05b4b-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05b4b-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05b4b-188">ロゴの背景が明るい、ポータルサイトアプリに表示されるロゴ画像</span><span class="sxs-lookup"><span data-stu-id="05b4b-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="05b4b-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="05b4b-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="05b4b-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05b4b-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05b4b-191">会社のポータルアプリのランディングページに表示されるカスタマイズ画像</span><span class="sxs-lookup"><span data-stu-id="05b4b-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="05b4b-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="05b4b-192">customPrivacyMessage</span></span>|<span data-ttu-id="05b4b-193">String</span><span class="sxs-lookup"><span data-stu-id="05b4b-193">String</span></span>|<span data-ttu-id="05b4b-194">デバイスで管理者がアクセスできる内容に関するテキストコメント</span><span class="sxs-lookup"><span data-stu-id="05b4b-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="05b4b-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="05b4b-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="05b4b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b4b-196">Boolean</span></span>|<span data-ttu-id="05b4b-197">Adminsistrator が企業所有のデバイスで [デバイスの削除] アクションを無効にしているかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="05b4b-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="05b4b-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="05b4b-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="05b4b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b4b-199">Boolean</span></span>|<span data-ttu-id="05b4b-200">Adminsistrator が企業所有のデバイスで "出荷時のリセット" アクションを無効にしているかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="05b4b-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|



## <a name="response"></a><span data-ttu-id="05b4b-201">応答</span><span class="sxs-lookup"><span data-stu-id="05b4b-201">Response</span></span>
<span data-ttu-id="05b4b-202">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05b4b-202">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05b4b-203">例</span><span class="sxs-lookup"><span data-stu-id="05b4b-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="05b4b-204">要求</span><span class="sxs-lookup"><span data-stu-id="05b4b-204">Request</span></span>
<span data-ttu-id="05b4b-205">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05b4b-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="05b4b-206">応答</span><span class="sxs-lookup"><span data-stu-id="05b4b-206">Response</span></span>
<span data-ttu-id="05b4b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05b4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```






