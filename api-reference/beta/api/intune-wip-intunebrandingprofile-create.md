---
title: intuneBrandingProfile を作成する
description: 新しい intuneBrandingProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e92ad91bd5d981e987fb6d5abfd32494f6ce54de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541805"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="5d0b1-103">intuneBrandingProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="5d0b1-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="5d0b1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d0b1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d0b1-106">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d0b1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5d0b1-107">Prerequisites</span></span>
<span data-ttu-id="5d0b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d0b1-110">Permission type</span></span>|<span data-ttu-id="5d0b1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d0b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d0b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d0b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d0b1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d0b1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d0b1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d0b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d0b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-115">Not supported.</span></span>|
|<span data-ttu-id="5d0b1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d0b1-116">Application</span></span>|<span data-ttu-id="5d0b1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d0b1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d0b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5d0b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d0b1-119">Request headers</span></span>
|<span data-ttu-id="5d0b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d0b1-120">Header</span></span>|<span data-ttu-id="5d0b1-121">値</span><span class="sxs-lookup"><span data-stu-id="5d0b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d0b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0b1-122">Authorization</span></span>|<span data-ttu-id="5d0b1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d0b1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5d0b1-124">Accept</span></span>|<span data-ttu-id="5d0b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d0b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d0b1-126">Request body</span></span>
<span data-ttu-id="5d0b1-127">要求本文で、intuneBrandingProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="5d0b1-128">次の表に、intuneBrandingProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="5d0b1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d0b1-129">Property</span></span>|<span data-ttu-id="5d0b1-130">型</span><span class="sxs-lookup"><span data-stu-id="5d0b1-130">Type</span></span>|<span data-ttu-id="5d0b1-131">説明</span><span class="sxs-lookup"><span data-stu-id="5d0b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d0b1-132">id</span><span class="sxs-lookup"><span data-stu-id="5d0b1-132">id</span></span>|<span data-ttu-id="5d0b1-133">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-133">String</span></span>|<span data-ttu-id="5d0b1-134">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="5d0b1-134">Profile Key</span></span>|
|<span data-ttu-id="5d0b1-135">profileName</span><span class="sxs-lookup"><span data-stu-id="5d0b1-135">profileName</span></span>|<span data-ttu-id="5d0b1-136">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-136">String</span></span>|<span data-ttu-id="5d0b1-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="5d0b1-137">Name of the profile</span></span>|
|<span data-ttu-id="5d0b1-138">profiledescription</span><span class="sxs-lookup"><span data-stu-id="5d0b1-138">profileDescription</span></span>|<span data-ttu-id="5d0b1-139">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-139">String</span></span>|<span data-ttu-id="5d0b1-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="5d0b1-140">Description of the profile</span></span>|
|<span data-ttu-id="5d0b1-141">isdefaultprofile</span><span class="sxs-lookup"><span data-stu-id="5d0b1-141">isDefaultProfile</span></span>|<span data-ttu-id="5d0b1-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="5d0b1-142">Boolean</span></span>|<span data-ttu-id="5d0b1-143">既定でプロファイルが使用されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="5d0b1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d0b1-144">createdDateTime</span></span>|<span data-ttu-id="5d0b1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0b1-145">DateTimeOffset</span></span>|<span data-ttu-id="5d0b1-146">BrandingProfile が作成されたとき。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="5d0b1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d0b1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="5d0b1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0b1-148">DateTimeOffset</span></span>|<span data-ttu-id="5d0b1-149">BrandingProfile が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="5d0b1-150">displayName</span><span class="sxs-lookup"><span data-stu-id="5d0b1-150">displayName</span></span>|<span data-ttu-id="5d0b1-151">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-151">String</span></span>|<span data-ttu-id="5d0b1-152">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="5d0b1-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="5d0b1-153">contactITName</span></span>|<span data-ttu-id="5d0b1-154">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-154">String</span></span>|<span data-ttu-id="5d0b1-155">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5d0b1-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5d0b1-156">contactITPhoneNumber</span></span>|<span data-ttu-id="5d0b1-157">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-157">String</span></span>|<span data-ttu-id="5d0b1-158">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5d0b1-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5d0b1-159">contactITEmailAddress</span></span>|<span data-ttu-id="5d0b1-160">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-160">String</span></span>|<span data-ttu-id="5d0b1-161">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5d0b1-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="5d0b1-162">contactITNotes</span></span>|<span data-ttu-id="5d0b1-163">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-163">String</span></span>|<span data-ttu-id="5d0b1-164">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5d0b1-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="5d0b1-165">privacyUrl</span></span>|<span data-ttu-id="5d0b1-166">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-166">String</span></span>|<span data-ttu-id="5d0b1-167">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="5d0b1-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="5d0b1-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="5d0b1-169">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-169">String</span></span>|<span data-ttu-id="5d0b1-170">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="5d0b1-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="5d0b1-171">onlineSupportSiteName</span></span>|<span data-ttu-id="5d0b1-172">String</span><span class="sxs-lookup"><span data-stu-id="5d0b1-172">String</span></span>|<span data-ttu-id="5d0b1-173">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="5d0b1-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="5d0b1-174">themeColor</span></span>|[<span data-ttu-id="5d0b1-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="5d0b1-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="5d0b1-176">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="5d0b1-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="5d0b1-177">showLogo</span></span>|<span data-ttu-id="5d0b1-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="5d0b1-178">Boolean</span></span>|<span data-ttu-id="5d0b1-179">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="5d0b1-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="5d0b1-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="5d0b1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d0b1-181">Boolean</span></span>|<span data-ttu-id="5d0b1-182">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="5d0b1-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="5d0b1-183">themeColorLogo</span></span>|[<span data-ttu-id="5d0b1-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d0b1-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d0b1-185">テーマの色の背景にある、ポータルサイトアプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="5d0b1-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="5d0b1-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="5d0b1-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d0b1-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d0b1-188">明るい背景上に会社のポータルアプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="5d0b1-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="5d0b1-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="5d0b1-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d0b1-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d0b1-191">会社のポータルアプリのランディングページに表示されるカスタマイズ画像</span><span class="sxs-lookup"><span data-stu-id="5d0b1-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="5d0b1-192">応答</span><span class="sxs-lookup"><span data-stu-id="5d0b1-192">Response</span></span>
<span data-ttu-id="5d0b1-193">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-193">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0b1-194">例</span><span class="sxs-lookup"><span data-stu-id="5d0b1-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d0b1-195">要求</span><span class="sxs-lookup"><span data-stu-id="5d0b1-195">Request</span></span>
<span data-ttu-id="5d0b1-196">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1205

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
  }
}
```

### <a name="response"></a><span data-ttu-id="5d0b1-197">応答</span><span class="sxs-lookup"><span data-stu-id="5d0b1-197">Response</span></span>
<span data-ttu-id="5d0b1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5d0b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

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
  }
}
```





