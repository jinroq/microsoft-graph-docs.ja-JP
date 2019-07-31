---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d921ffbaca07a790060011a9970b4b02b0e8472
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010701"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="9c724-103">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="9c724-103">intuneBrand resource type</span></span>

> <span data-ttu-id="9c724-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c724-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c724-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c724-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c724-106">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9c724-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="9c724-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c724-107">Properties</span></span>
|<span data-ttu-id="9c724-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c724-108">Property</span></span>|<span data-ttu-id="9c724-109">型</span><span class="sxs-lookup"><span data-stu-id="9c724-109">Type</span></span>|<span data-ttu-id="9c724-110">説明</span><span class="sxs-lookup"><span data-stu-id="9c724-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c724-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9c724-111">displayName</span></span>|<span data-ttu-id="9c724-112">String</span><span class="sxs-lookup"><span data-stu-id="9c724-112">String</span></span>|<span data-ttu-id="9c724-113">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="9c724-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="9c724-114">contactITName</span><span class="sxs-lookup"><span data-stu-id="9c724-114">contactITName</span></span>|<span data-ttu-id="9c724-115">String</span><span class="sxs-lookup"><span data-stu-id="9c724-115">String</span></span>|<span data-ttu-id="9c724-116">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="9c724-116">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9c724-117">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9c724-117">contactITPhoneNumber</span></span>|<span data-ttu-id="9c724-118">String</span><span class="sxs-lookup"><span data-stu-id="9c724-118">String</span></span>|<span data-ttu-id="9c724-119">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="9c724-119">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9c724-120">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9c724-120">contactITEmailAddress</span></span>|<span data-ttu-id="9c724-121">String</span><span class="sxs-lookup"><span data-stu-id="9c724-121">String</span></span>|<span data-ttu-id="9c724-122">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="9c724-122">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9c724-123">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="9c724-123">contactITNotes</span></span>|<span data-ttu-id="9c724-124">String</span><span class="sxs-lookup"><span data-stu-id="9c724-124">String</span></span>|<span data-ttu-id="9c724-125">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="9c724-125">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9c724-126">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="9c724-126">privacyUrl</span></span>|<span data-ttu-id="9c724-127">String</span><span class="sxs-lookup"><span data-stu-id="9c724-127">String</span></span>|<span data-ttu-id="9c724-128">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="9c724-128">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="9c724-129">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="9c724-129">onlineSupportSiteUrl</span></span>|<span data-ttu-id="9c724-130">String</span><span class="sxs-lookup"><span data-stu-id="9c724-130">String</span></span>|<span data-ttu-id="9c724-131">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="9c724-131">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="9c724-132">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="9c724-132">onlineSupportSiteName</span></span>|<span data-ttu-id="9c724-133">String</span><span class="sxs-lookup"><span data-stu-id="9c724-133">String</span></span>|<span data-ttu-id="9c724-134">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="9c724-134">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="9c724-135">themeColor</span><span class="sxs-lookup"><span data-stu-id="9c724-135">themeColor</span></span>|[<span data-ttu-id="9c724-136">rgbColor</span><span class="sxs-lookup"><span data-stu-id="9c724-136">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="9c724-137">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="9c724-137">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="9c724-138">showLogo</span><span class="sxs-lookup"><span data-stu-id="9c724-138">showLogo</span></span>|<span data-ttu-id="9c724-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c724-139">Boolean</span></span>|<span data-ttu-id="9c724-140">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="9c724-140">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="9c724-141">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="9c724-141">lightBackgroundLogo</span></span>|[<span data-ttu-id="9c724-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9c724-142">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9c724-143">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="9c724-143">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="9c724-144">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="9c724-144">darkBackgroundLogo</span></span>|[<span data-ttu-id="9c724-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9c724-145">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9c724-146">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="9c724-146">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="9c724-147">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="9c724-147">showNameNextToLogo</span></span>|<span data-ttu-id="9c724-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c724-148">Boolean</span></span>|<span data-ttu-id="9c724-149">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="9c724-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="9c724-150">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="9c724-150">landingPageCustomizedImage</span></span>|[<span data-ttu-id="9c724-151">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9c724-151">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9c724-152">会社のポータルアプリのランディングページに表示されるカスタマイズ画像</span><span class="sxs-lookup"><span data-stu-id="9c724-152">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="9c724-153">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="9c724-153">customPrivacyMessage</span></span>|<span data-ttu-id="9c724-154">String</span><span class="sxs-lookup"><span data-stu-id="9c724-154">String</span></span>|<span data-ttu-id="9c724-155">カスタムプライバシーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="9c724-155">Custom privacy message.</span></span>|
|<span data-ttu-id="9c724-156">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="9c724-156">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="9c724-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c724-157">Boolean</span></span>|<span data-ttu-id="9c724-158">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="9c724-158">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c724-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c724-159">Relationships</span></span>
<span data-ttu-id="9c724-160">なし</span><span class="sxs-lookup"><span data-stu-id="9c724-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c724-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c724-161">JSON Representation</span></span>
<span data-ttu-id="9c724-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c724-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
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
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "customPrivacyMessage": "String",
  "showDisplayNameNextToLogo": true
}
```





