---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4e1e4a4a4042b9a4dd9382f1310d737ac1c9678
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398605"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="29a5a-103">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="29a5a-103">intuneBrand resource type</span></span>

> <span data-ttu-id="29a5a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29a5a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29a5a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29a5a-107">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29a5a-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="29a5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29a5a-108">Properties</span></span>
|<span data-ttu-id="29a5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29a5a-109">Property</span></span>|<span data-ttu-id="29a5a-110">型</span><span class="sxs-lookup"><span data-stu-id="29a5a-110">Type</span></span>|<span data-ttu-id="29a5a-111">説明</span><span class="sxs-lookup"><span data-stu-id="29a5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a5a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="29a5a-112">displayName</span></span>|<span data-ttu-id="29a5a-113">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-113">String</span></span>|<span data-ttu-id="29a5a-114">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="29a5a-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="29a5a-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="29a5a-115">contactITName</span></span>|<span data-ttu-id="29a5a-116">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-116">String</span></span>|<span data-ttu-id="29a5a-117">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="29a5a-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="29a5a-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="29a5a-118">contactITPhoneNumber</span></span>|<span data-ttu-id="29a5a-119">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-119">String</span></span>|<span data-ttu-id="29a5a-120">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="29a5a-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="29a5a-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="29a5a-121">contactITEmailAddress</span></span>|<span data-ttu-id="29a5a-122">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-122">String</span></span>|<span data-ttu-id="29a5a-123">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="29a5a-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="29a5a-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="29a5a-124">contactITNotes</span></span>|<span data-ttu-id="29a5a-125">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-125">String</span></span>|<span data-ttu-id="29a5a-126">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="29a5a-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="29a5a-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="29a5a-127">privacyUrl</span></span>|<span data-ttu-id="29a5a-128">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-128">String</span></span>|<span data-ttu-id="29a5a-129">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="29a5a-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="29a5a-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="29a5a-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="29a5a-131">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-131">String</span></span>|<span data-ttu-id="29a5a-132">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="29a5a-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="29a5a-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="29a5a-133">onlineSupportSiteName</span></span>|<span data-ttu-id="29a5a-134">String</span><span class="sxs-lookup"><span data-stu-id="29a5a-134">String</span></span>|<span data-ttu-id="29a5a-135">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="29a5a-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="29a5a-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="29a5a-136">themeColor</span></span>|[<span data-ttu-id="29a5a-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="29a5a-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="29a5a-138">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="29a5a-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="29a5a-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="29a5a-139">showLogo</span></span>|<span data-ttu-id="29a5a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="29a5a-140">Boolean</span></span>|<span data-ttu-id="29a5a-141">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="29a5a-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="29a5a-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="29a5a-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="29a5a-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29a5a-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29a5a-144">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="29a5a-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="29a5a-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="29a5a-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="29a5a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29a5a-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29a5a-147">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="29a5a-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="29a5a-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="29a5a-148">showNameNextToLogo</span></span>|<span data-ttu-id="29a5a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="29a5a-149">Boolean</span></span>|<span data-ttu-id="29a5a-150">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="29a5a-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="29a5a-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="29a5a-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="29a5a-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29a5a-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29a5a-153">Compnay ポータル アプリケーションのランディング ・ ページに表示されるイメージをカスタマイズしました。</span><span class="sxs-lookup"><span data-stu-id="29a5a-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="29a5a-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="29a5a-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="29a5a-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="29a5a-155">Boolean</span></span>|<span data-ttu-id="29a5a-156">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="29a5a-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29a5a-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29a5a-157">Relationships</span></span>
<span data-ttu-id="29a5a-158">なし</span><span class="sxs-lookup"><span data-stu-id="29a5a-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29a5a-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29a5a-159">JSON Representation</span></span>
<span data-ttu-id="29a5a-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29a5a-160">Here is a JSON representation of the resource.</span></span>
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
  "showDisplayNameNextToLogo": true
}
```




