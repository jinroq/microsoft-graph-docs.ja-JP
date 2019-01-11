---
title: intuneBrandingProfile リソースの種類
description: このエンティティには、会社のポータル アプリケーションとエンド ・ ユーザーの web ポータルのテナントのレベルの外観をカスタマイズするために使用するデータが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2ee2fee902b4aca542810dc058b7d16aaedb9c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820609"
---
# <a name="intunebrandingprofile-resource-type"></a><span data-ttu-id="1204d-103">intuneBrandingProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1204d-103">intuneBrandingProfile resource type</span></span>

> <span data-ttu-id="1204d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1204d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1204d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1204d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1204d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1204d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1204d-107">このエンティティには、会社のポータル アプリケーションとエンド ・ ユーザーの web ポータルのテナントのレベルの外観をカスタマイズするために使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1204d-107">This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="methods"></a><span data-ttu-id="1204d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1204d-108">Methods</span></span>
|<span data-ttu-id="1204d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1204d-109">Method</span></span>|<span data-ttu-id="1204d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1204d-110">Return Type</span></span>|<span data-ttu-id="1204d-111">説明</span><span class="sxs-lookup"><span data-stu-id="1204d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1204d-112">リスト intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="1204d-112">List intuneBrandingProfiles</span></span>](../api/intune-wip-intunebrandingprofile-list.md)|<span data-ttu-id="1204d-113">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1204d-113">[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) collection</span></span>|<span data-ttu-id="1204d-114">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1204d-114">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>|
|[<span data-ttu-id="1204d-115">IntuneBrandingProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="1204d-115">Get intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-get.md)|[<span data-ttu-id="1204d-116">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="1204d-116">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="1204d-117">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1204d-117">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|
|[<span data-ttu-id="1204d-118">IntuneBrandingProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="1204d-118">Create intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-create.md)|[<span data-ttu-id="1204d-119">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="1204d-119">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="1204d-120">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1204d-120">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|
|[<span data-ttu-id="1204d-121">IntuneBrandingProfile を削除します。</span><span class="sxs-lookup"><span data-stu-id="1204d-121">Delete intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-delete.md)|<span data-ttu-id="1204d-122">なし</span><span class="sxs-lookup"><span data-stu-id="1204d-122">None</span></span>|<span data-ttu-id="1204d-123">の[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1204d-123">Deletes a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>|
|[<span data-ttu-id="1204d-124">IntuneBrandingProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="1204d-124">Update intuneBrandingProfile</span></span>](../api/intune-wip-intunebrandingprofile-update.md)|[<span data-ttu-id="1204d-125">intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="1204d-125">intuneBrandingProfile</span></span>](../resources/intune-wip-intunebrandingprofile.md)|<span data-ttu-id="1204d-126">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1204d-126">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1204d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1204d-127">Properties</span></span>
|<span data-ttu-id="1204d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1204d-128">Property</span></span>|<span data-ttu-id="1204d-129">種類</span><span class="sxs-lookup"><span data-stu-id="1204d-129">Type</span></span>|<span data-ttu-id="1204d-130">説明</span><span class="sxs-lookup"><span data-stu-id="1204d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1204d-131">ID</span><span class="sxs-lookup"><span data-stu-id="1204d-131">id</span></span>|<span data-ttu-id="1204d-132">String</span><span class="sxs-lookup"><span data-stu-id="1204d-132">String</span></span>|<span data-ttu-id="1204d-133">プロファイル キー</span><span class="sxs-lookup"><span data-stu-id="1204d-133">Profile Key</span></span>|
|<span data-ttu-id="1204d-134">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="1204d-134">profileName</span></span>|<span data-ttu-id="1204d-135">String</span><span class="sxs-lookup"><span data-stu-id="1204d-135">String</span></span>|<span data-ttu-id="1204d-136">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="1204d-136">Name of the profile</span></span>|
|<span data-ttu-id="1204d-137">profileDescription</span><span class="sxs-lookup"><span data-stu-id="1204d-137">profileDescription</span></span>|<span data-ttu-id="1204d-138">String</span><span class="sxs-lookup"><span data-stu-id="1204d-138">String</span></span>|<span data-ttu-id="1204d-139">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="1204d-139">Description of the profile</span></span>|
|<span data-ttu-id="1204d-140">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="1204d-140">isDefaultProfile</span></span>|<span data-ttu-id="1204d-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="1204d-141">Boolean</span></span>|<span data-ttu-id="1204d-142">既定のプロファイルが使用される場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="1204d-142">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="1204d-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1204d-143">createdDateTime</span></span>|<span data-ttu-id="1204d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1204d-144">DateTimeOffset</span></span>|<span data-ttu-id="1204d-145">BrandingProfile が作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="1204d-145">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="1204d-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1204d-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1204d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1204d-147">DateTimeOffset</span></span>|<span data-ttu-id="1204d-148">BrandingProfile の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="1204d-148">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="1204d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="1204d-149">displayName</span></span>|<span data-ttu-id="1204d-150">String</span><span class="sxs-lookup"><span data-stu-id="1204d-150">String</span></span>|<span data-ttu-id="1204d-151">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="1204d-151">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="1204d-152">contactITName</span><span class="sxs-lookup"><span data-stu-id="1204d-152">contactITName</span></span>|<span data-ttu-id="1204d-153">String</span><span class="sxs-lookup"><span data-stu-id="1204d-153">String</span></span>|<span data-ttu-id="1204d-154">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="1204d-154">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1204d-155">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1204d-155">contactITPhoneNumber</span></span>|<span data-ttu-id="1204d-156">String</span><span class="sxs-lookup"><span data-stu-id="1204d-156">String</span></span>|<span data-ttu-id="1204d-157">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="1204d-157">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1204d-158">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1204d-158">contactITEmailAddress</span></span>|<span data-ttu-id="1204d-159">String</span><span class="sxs-lookup"><span data-stu-id="1204d-159">String</span></span>|<span data-ttu-id="1204d-160">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="1204d-160">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1204d-161">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="1204d-161">contactITNotes</span></span>|<span data-ttu-id="1204d-162">String</span><span class="sxs-lookup"><span data-stu-id="1204d-162">String</span></span>|<span data-ttu-id="1204d-163">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="1204d-163">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1204d-164">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="1204d-164">privacyUrl</span></span>|<span data-ttu-id="1204d-165">String</span><span class="sxs-lookup"><span data-stu-id="1204d-165">String</span></span>|<span data-ttu-id="1204d-166">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="1204d-166">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="1204d-167">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="1204d-167">onlineSupportSiteUrl</span></span>|<span data-ttu-id="1204d-168">String</span><span class="sxs-lookup"><span data-stu-id="1204d-168">String</span></span>|<span data-ttu-id="1204d-169">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="1204d-169">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1204d-170">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="1204d-170">onlineSupportSiteName</span></span>|<span data-ttu-id="1204d-171">String</span><span class="sxs-lookup"><span data-stu-id="1204d-171">String</span></span>|<span data-ttu-id="1204d-172">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="1204d-172">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1204d-173">themeColor</span><span class="sxs-lookup"><span data-stu-id="1204d-173">themeColor</span></span>|[<span data-ttu-id="1204d-174">rgbColor</span><span class="sxs-lookup"><span data-stu-id="1204d-174">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="1204d-175">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="1204d-175">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="1204d-176">showLogo</span><span class="sxs-lookup"><span data-stu-id="1204d-176">showLogo</span></span>|<span data-ttu-id="1204d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="1204d-177">Boolean</span></span>|<span data-ttu-id="1204d-178">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="1204d-178">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="1204d-179">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1204d-179">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="1204d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1204d-180">Boolean</span></span>|<span data-ttu-id="1204d-181">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="1204d-181">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="1204d-182">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="1204d-182">themeColorLogo</span></span>|[<span data-ttu-id="1204d-183">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1204d-183">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1204d-184">ロゴ イメージがテーマの背景色を会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="1204d-184">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="1204d-185">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1204d-185">lightBackgroundLogo</span></span>|[<span data-ttu-id="1204d-186">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1204d-186">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1204d-187">ロゴのイメージは明るい背景に会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="1204d-187">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="1204d-188">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="1204d-188">landingPageCustomizedImage</span></span>|[<span data-ttu-id="1204d-189">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1204d-189">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1204d-190">会社のポータル アプリケーションのランディング ページに表示されるカスタムのイメージ</span><span class="sxs-lookup"><span data-stu-id="1204d-190">Customized image displayed in Company Portal apps landing page</span></span>|

## <a name="relationships"></a><span data-ttu-id="1204d-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1204d-191">Relationships</span></span>
<span data-ttu-id="1204d-192">なし</span><span class="sxs-lookup"><span data-stu-id="1204d-192">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1204d-193">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1204d-193">JSON Representation</span></span>
<span data-ttu-id="1204d-194">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1204d-194">Here is a JSON representation of the resource.</span></span>
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





