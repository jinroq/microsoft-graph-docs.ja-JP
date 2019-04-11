---
title: intuneBrandingProfile リソースの種類
description: このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eae52bbb19eaca46c74d275ae7da3d16050a50e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799917"
---
# <a name="intunebrandingprofile-resource-type"></a><span data-ttu-id="952e4-103">intuneBrandingProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="952e4-103">intuneBrandingProfile resource type</span></span>

> <span data-ttu-id="952e4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="952e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="952e4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="952e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="952e4-106">このエンティティにはデータが含まれており、これを使用して、会社のポータルアプリケーションとエンドユーザーの web ポータルのテナントレベルの外観をカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="952e4-106">This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="methods"></a><span data-ttu-id="952e4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="952e4-107">Methods</span></span>
|<span data-ttu-id="952e4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="952e4-108">Method</span></span>|<span data-ttu-id="952e4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="952e4-109">Return Type</span></span>|<span data-ttu-id="952e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="952e4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="952e4-111">リスト intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="952e4-111">List intuneBrandingProfiles</span></span>](../api/intune-wip-intunebrandingprofile-list.md)|<span data-ttu-id="952e4-112">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="952e4-112">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) collection</span></span>|<span data-ttu-id="952e4-113">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="952e4-113">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>|
|[<span data-ttu-id="952e4-114">intuneBrandingProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="952e4-114">Get intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-get.md)|[<span data-ttu-id="952e4-115">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="952e4-115">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="952e4-116">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="952e4-116">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|
|[<span data-ttu-id="952e4-117">intuneBrandingProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="952e4-117">Create intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-create.md)|[<span data-ttu-id="952e4-118">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="952e4-118">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="952e4-119">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="952e4-119">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|
|[<span data-ttu-id="952e4-120">intuneBrandingProfile の削除</span><span class="sxs-lookup"><span data-stu-id="952e4-120">Delete intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-delete.md)|<span data-ttu-id="952e4-121">なし</span><span class="sxs-lookup"><span data-stu-id="952e4-121">None</span></span>|<span data-ttu-id="952e4-122">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="952e4-122">Deletes a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>|
|[<span data-ttu-id="952e4-123">intuneBrandingProfile の更新</span><span class="sxs-lookup"><span data-stu-id="952e4-123">Update intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-update.md)|[<span data-ttu-id="952e4-124">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="952e4-124">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="952e4-125">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="952e4-125">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|
|[<span data-ttu-id="952e4-126">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="952e4-126">assign action</span></span>](../api/intune-wip-intunebrandingprofile-assign.md)|<span data-ttu-id="952e4-127">なし</span><span class="sxs-lookup"><span data-stu-id="952e4-127">None</span></span>|<span data-ttu-id="952e4-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="952e4-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="952e4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="952e4-129">Properties</span></span>
|<span data-ttu-id="952e4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="952e4-130">Property</span></span>|<span data-ttu-id="952e4-131">型</span><span class="sxs-lookup"><span data-stu-id="952e4-131">Type</span></span>|<span data-ttu-id="952e4-132">説明</span><span class="sxs-lookup"><span data-stu-id="952e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952e4-133">id</span><span class="sxs-lookup"><span data-stu-id="952e4-133">id</span></span>|<span data-ttu-id="952e4-134">String</span><span class="sxs-lookup"><span data-stu-id="952e4-134">String</span></span>|<span data-ttu-id="952e4-135">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="952e4-135">Profile Key</span></span>|
|<span data-ttu-id="952e4-136">profileName</span><span class="sxs-lookup"><span data-stu-id="952e4-136">profileName</span></span>|<span data-ttu-id="952e4-137">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-137">String</span></span>|<span data-ttu-id="952e4-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="952e4-138">Name of the profile</span></span>|
|<span data-ttu-id="952e4-139">profiledescription</span><span class="sxs-lookup"><span data-stu-id="952e4-139">profileDescription</span></span>|<span data-ttu-id="952e4-140">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-140">String</span></span>|<span data-ttu-id="952e4-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="952e4-141">Description of the profile</span></span>|
|<span data-ttu-id="952e4-142">isdefaultprofile</span><span class="sxs-lookup"><span data-stu-id="952e4-142">isDefaultProfile</span></span>|<span data-ttu-id="952e4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="952e4-143">Boolean</span></span>|<span data-ttu-id="952e4-144">既定でプロファイルが使用されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="952e4-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="952e4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="952e4-145">createdDateTime</span></span>|<span data-ttu-id="952e4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952e4-146">DateTimeOffset</span></span>|<span data-ttu-id="952e4-147">BrandingProfile が作成されたとき。</span><span class="sxs-lookup"><span data-stu-id="952e4-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="952e4-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="952e4-148">lastModifiedDateTime</span></span>|<span data-ttu-id="952e4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952e4-149">DateTimeOffset</span></span>|<span data-ttu-id="952e4-150">BrandingProfile が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="952e4-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="952e4-151">displayName</span><span class="sxs-lookup"><span data-stu-id="952e4-151">displayName</span></span>|<span data-ttu-id="952e4-152">String</span><span class="sxs-lookup"><span data-stu-id="952e4-152">String</span></span>|<span data-ttu-id="952e4-153">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="952e4-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="952e4-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="952e4-154">contactITName</span></span>|<span data-ttu-id="952e4-155">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-155">String</span></span>|<span data-ttu-id="952e4-156">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="952e4-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="952e4-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="952e4-157">contactITPhoneNumber</span></span>|<span data-ttu-id="952e4-158">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-158">String</span></span>|<span data-ttu-id="952e4-159">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="952e4-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="952e4-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="952e4-160">contactITEmailAddress</span></span>|<span data-ttu-id="952e4-161">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-161">String</span></span>|<span data-ttu-id="952e4-162">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="952e4-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="952e4-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="952e4-163">contactITNotes</span></span>|<span data-ttu-id="952e4-164">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-164">String</span></span>|<span data-ttu-id="952e4-165">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="952e4-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="952e4-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="952e4-166">privacyUrl</span></span>|<span data-ttu-id="952e4-167">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-167">String</span></span>|<span data-ttu-id="952e4-168">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="952e4-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="952e4-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="952e4-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="952e4-170">文字列</span><span class="sxs-lookup"><span data-stu-id="952e4-170">String</span></span>|<span data-ttu-id="952e4-171">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="952e4-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="952e4-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="952e4-172">onlineSupportSiteName</span></span>|<span data-ttu-id="952e4-173">String</span><span class="sxs-lookup"><span data-stu-id="952e4-173">String</span></span>|<span data-ttu-id="952e4-174">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="952e4-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="952e4-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="952e4-175">themeColor</span></span>|[<span data-ttu-id="952e4-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="952e4-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="952e4-177">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="952e4-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="952e4-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="952e4-178">showLogo</span></span>|<span data-ttu-id="952e4-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="952e4-179">Boolean</span></span>|<span data-ttu-id="952e4-180">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="952e4-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="952e4-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="952e4-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="952e4-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="952e4-182">Boolean</span></span>|<span data-ttu-id="952e4-183">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="952e4-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="952e4-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="952e4-184">themeColorLogo</span></span>|[<span data-ttu-id="952e4-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="952e4-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="952e4-186">テーマの色の背景にある、ポータルサイトアプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="952e4-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="952e4-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="952e4-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="952e4-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="952e4-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="952e4-189">明るい背景上に会社のポータルアプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="952e4-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="952e4-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="952e4-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="952e4-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="952e4-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="952e4-192">会社のポータルアプリのランディングページに表示されるカスタマイズ画像</span><span class="sxs-lookup"><span data-stu-id="952e4-192">Customized image displayed in Company Portal apps landing page</span></span>|

## <a name="relationships"></a><span data-ttu-id="952e4-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="952e4-193">Relationships</span></span>
|<span data-ttu-id="952e4-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="952e4-194">Relationship</span></span>|<span data-ttu-id="952e4-195">型</span><span class="sxs-lookup"><span data-stu-id="952e4-195">Type</span></span>|<span data-ttu-id="952e4-196">説明</span><span class="sxs-lookup"><span data-stu-id="952e4-196">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952e4-197">assignments</span><span class="sxs-lookup"><span data-stu-id="952e4-197">assignments</span></span>|<span data-ttu-id="952e4-198">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="952e4-198">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="952e4-199">ブランド化プロファイルのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="952e4-199">The list of group assignments for the branding profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="952e4-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="952e4-200">JSON Representation</span></span>
<span data-ttu-id="952e4-201">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="952e4-201">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





