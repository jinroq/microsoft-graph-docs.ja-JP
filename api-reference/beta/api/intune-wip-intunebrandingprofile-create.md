---
title: IntuneBrandingProfile を作成する
description: 新しい intuneBrandingProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec5e863d171c952c07acfb0ecf2c312dcd89a366
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990667"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="1d1c5-103">IntuneBrandingProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="1d1c5-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="1d1c5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d1c5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d1c5-106">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d1c5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d1c5-107">Prerequisites</span></span>
<span data-ttu-id="1d1c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d1c5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d1c5-110">Permission type</span></span>|<span data-ttu-id="1d1c5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d1c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d1c5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d1c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d1c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d1c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d1c5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d1c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d1c5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-115">Not supported.</span></span>|
|<span data-ttu-id="1d1c5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d1c5-116">Application</span></span>|<span data-ttu-id="1d1c5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d1c5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d1c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1d1c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d1c5-119">Request headers</span></span>
|<span data-ttu-id="1d1c5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d1c5-120">Header</span></span>|<span data-ttu-id="1d1c5-121">値</span><span class="sxs-lookup"><span data-stu-id="1d1c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d1c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d1c5-122">Authorization</span></span>|<span data-ttu-id="1d1c5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d1c5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1d1c5-124">Accept</span></span>|<span data-ttu-id="1d1c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d1c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d1c5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d1c5-126">Request body</span></span>
<span data-ttu-id="1d1c5-127">要求本文で、intuneBrandingProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="1d1c5-128">次の表に、intuneBrandingProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="1d1c5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d1c5-129">Property</span></span>|<span data-ttu-id="1d1c5-130">型</span><span class="sxs-lookup"><span data-stu-id="1d1c5-130">Type</span></span>|<span data-ttu-id="1d1c5-131">説明</span><span class="sxs-lookup"><span data-stu-id="1d1c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d1c5-132">id</span><span class="sxs-lookup"><span data-stu-id="1d1c5-132">id</span></span>|<span data-ttu-id="1d1c5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1d1c5-133">String</span></span>|<span data-ttu-id="1d1c5-134">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="1d1c5-134">Profile Key</span></span>|
|<span data-ttu-id="1d1c5-135">profileName</span><span class="sxs-lookup"><span data-stu-id="1d1c5-135">profileName</span></span>|<span data-ttu-id="1d1c5-136">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-136">String</span></span>|<span data-ttu-id="1d1c5-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="1d1c5-137">Name of the profile</span></span>|
|<span data-ttu-id="1d1c5-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="1d1c5-138">profileDescription</span></span>|<span data-ttu-id="1d1c5-139">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-139">String</span></span>|<span data-ttu-id="1d1c5-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="1d1c5-140">Description of the profile</span></span>|
|<span data-ttu-id="1d1c5-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="1d1c5-141">isDefaultProfile</span></span>|<span data-ttu-id="1d1c5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d1c5-142">Boolean</span></span>|<span data-ttu-id="1d1c5-143">プロファイルが既定として使用されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="1d1c5-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="1d1c5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d1c5-144">createdDateTime</span></span>|<span data-ttu-id="1d1c5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d1c5-145">DateTimeOffset</span></span>|<span data-ttu-id="1d1c5-146">BrandingProfile が作成された時刻</span><span class="sxs-lookup"><span data-stu-id="1d1c5-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="1d1c5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d1c5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1d1c5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d1c5-148">DateTimeOffset</span></span>|<span data-ttu-id="1d1c5-149">BrandingProfile が最後に変更された時刻</span><span class="sxs-lookup"><span data-stu-id="1d1c5-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="1d1c5-150">displayName</span><span class="sxs-lookup"><span data-stu-id="1d1c5-150">displayName</span></span>|<span data-ttu-id="1d1c5-151">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-151">String</span></span>|<span data-ttu-id="1d1c5-152">エンドユーザーに表示される会社名または組織名</span><span class="sxs-lookup"><span data-stu-id="1d1c5-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="1d1c5-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="1d1c5-153">contactITName</span></span>|<span data-ttu-id="1d1c5-154">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-154">String</span></span>|<span data-ttu-id="1d1c5-155">IT サポートを担当する個人または組織の名前</span><span class="sxs-lookup"><span data-stu-id="1d1c5-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="1d1c5-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1d1c5-156">contactITPhoneNumber</span></span>|<span data-ttu-id="1d1c5-157">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-157">String</span></span>|<span data-ttu-id="1d1c5-158">IT サポートを担当する個人または組織の電話番号</span><span class="sxs-lookup"><span data-stu-id="1d1c5-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="1d1c5-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1d1c5-159">contactITEmailAddress</span></span>|<span data-ttu-id="1d1c5-160">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-160">String</span></span>|<span data-ttu-id="1d1c5-161">IT サポートを担当する個人または組織の電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="1d1c5-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="1d1c5-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="1d1c5-162">contactITNotes</span></span>|<span data-ttu-id="1d1c5-163">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-163">String</span></span>|<span data-ttu-id="1d1c5-164">IT サポートを担当する個人または組織に関するテキストコメント</span><span class="sxs-lookup"><span data-stu-id="1d1c5-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="1d1c5-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="1d1c5-165">privacyUrl</span></span>|<span data-ttu-id="1d1c5-166">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-166">String</span></span>|<span data-ttu-id="1d1c5-167">会社/組織のプライバシーポリシーの URL</span><span class="sxs-lookup"><span data-stu-id="1d1c5-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="1d1c5-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="1d1c5-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="1d1c5-169">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-169">String</span></span>|<span data-ttu-id="1d1c5-170">会社または組織の IT ヘルプデスクサイトへの URL</span><span class="sxs-lookup"><span data-stu-id="1d1c5-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="1d1c5-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="1d1c5-171">onlineSupportSiteName</span></span>|<span data-ttu-id="1d1c5-172">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-172">String</span></span>|<span data-ttu-id="1d1c5-173">会社/組織の IT ヘルプデスクサイトの表示名</span><span class="sxs-lookup"><span data-stu-id="1d1c5-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="1d1c5-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="1d1c5-174">themeColor</span></span>|[<span data-ttu-id="1d1c5-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="1d1c5-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="1d1c5-176">会社のポータルアプリケーションと web ポータルで使用される主要なテーマの色</span><span class="sxs-lookup"><span data-stu-id="1d1c5-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="1d1c5-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="1d1c5-177">showLogo</span></span>|<span data-ttu-id="1d1c5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d1c5-178">Boolean</span></span>|<span data-ttu-id="1d1c5-179">管理者が指定したロゴ画像が表示されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="1d1c5-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="1d1c5-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1d1c5-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="1d1c5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d1c5-181">Boolean</span></span>|<span data-ttu-id="1d1c5-182">管理者が指定した表示名がロゴ画像の隣に表示されるかどうかを表すブール値</span><span class="sxs-lookup"><span data-stu-id="1d1c5-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="1d1c5-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="1d1c5-183">themeColorLogo</span></span>|[<span data-ttu-id="1d1c5-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d1c5-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d1c5-185">ロゴの背景色がテーマになっている、ポータルサイトアプリに表示されるロゴ画像</span><span class="sxs-lookup"><span data-stu-id="1d1c5-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="1d1c5-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1d1c5-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="1d1c5-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d1c5-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d1c5-188">ロゴの背景が明るい、ポータルサイトアプリに表示されるロゴ画像</span><span class="sxs-lookup"><span data-stu-id="1d1c5-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="1d1c5-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="1d1c5-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="1d1c5-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d1c5-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d1c5-191">会社のポータルアプリのランディングページに表示されるカスタマイズ画像</span><span class="sxs-lookup"><span data-stu-id="1d1c5-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="1d1c5-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="1d1c5-192">customPrivacyMessage</span></span>|<span data-ttu-id="1d1c5-193">String</span><span class="sxs-lookup"><span data-stu-id="1d1c5-193">String</span></span>|<span data-ttu-id="1d1c5-194">デバイスで管理者がアクセスできる内容に関するテキストコメント</span><span class="sxs-lookup"><span data-stu-id="1d1c5-194">Text comments regarding what the admin has access to on the device</span></span>|



## <a name="response"></a><span data-ttu-id="1d1c5-195">応答</span><span class="sxs-lookup"><span data-stu-id="1d1c5-195">Response</span></span>
<span data-ttu-id="1d1c5-196">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-196">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d1c5-197">例</span><span class="sxs-lookup"><span data-stu-id="1d1c5-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d1c5-198">要求</span><span class="sxs-lookup"><span data-stu-id="1d1c5-198">Request</span></span>
<span data-ttu-id="1d1c5-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1264

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```

### <a name="response"></a><span data-ttu-id="1d1c5-200">応答</span><span class="sxs-lookup"><span data-stu-id="1d1c5-200">Response</span></span>
<span data-ttu-id="1d1c5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d1c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```





