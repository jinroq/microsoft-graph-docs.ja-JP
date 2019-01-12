---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab8465390b6b0a9e4f35e8a713f082dfb9325eb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957684"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="28a94-103">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="28a94-103">intuneBrand resource type</span></span>

> <span data-ttu-id="28a94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28a94-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28a94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28a94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28a94-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28a94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28a94-107">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="28a94-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="28a94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28a94-108">Properties</span></span>
|<span data-ttu-id="28a94-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28a94-109">Property</span></span>|<span data-ttu-id="28a94-110">種類</span><span class="sxs-lookup"><span data-stu-id="28a94-110">Type</span></span>|<span data-ttu-id="28a94-111">説明</span><span class="sxs-lookup"><span data-stu-id="28a94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a94-112">displayName</span><span class="sxs-lookup"><span data-stu-id="28a94-112">displayName</span></span>|<span data-ttu-id="28a94-113">String</span><span class="sxs-lookup"><span data-stu-id="28a94-113">String</span></span>|<span data-ttu-id="28a94-114">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="28a94-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="28a94-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="28a94-115">contactITName</span></span>|<span data-ttu-id="28a94-116">String</span><span class="sxs-lookup"><span data-stu-id="28a94-116">String</span></span>|<span data-ttu-id="28a94-117">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="28a94-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28a94-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="28a94-118">contactITPhoneNumber</span></span>|<span data-ttu-id="28a94-119">String</span><span class="sxs-lookup"><span data-stu-id="28a94-119">String</span></span>|<span data-ttu-id="28a94-120">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="28a94-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28a94-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="28a94-121">contactITEmailAddress</span></span>|<span data-ttu-id="28a94-122">String</span><span class="sxs-lookup"><span data-stu-id="28a94-122">String</span></span>|<span data-ttu-id="28a94-123">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="28a94-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28a94-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="28a94-124">contactITNotes</span></span>|<span data-ttu-id="28a94-125">String</span><span class="sxs-lookup"><span data-stu-id="28a94-125">String</span></span>|<span data-ttu-id="28a94-126">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="28a94-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="28a94-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="28a94-127">privacyUrl</span></span>|<span data-ttu-id="28a94-128">String</span><span class="sxs-lookup"><span data-stu-id="28a94-128">String</span></span>|<span data-ttu-id="28a94-129">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="28a94-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="28a94-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="28a94-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="28a94-131">String</span><span class="sxs-lookup"><span data-stu-id="28a94-131">String</span></span>|<span data-ttu-id="28a94-132">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="28a94-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="28a94-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="28a94-133">onlineSupportSiteName</span></span>|<span data-ttu-id="28a94-134">String</span><span class="sxs-lookup"><span data-stu-id="28a94-134">String</span></span>|<span data-ttu-id="28a94-135">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="28a94-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="28a94-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="28a94-136">themeColor</span></span>|[<span data-ttu-id="28a94-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="28a94-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="28a94-138">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="28a94-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="28a94-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="28a94-139">showLogo</span></span>|<span data-ttu-id="28a94-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="28a94-140">Boolean</span></span>|<span data-ttu-id="28a94-141">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="28a94-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="28a94-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="28a94-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="28a94-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28a94-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28a94-144">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="28a94-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="28a94-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="28a94-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="28a94-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28a94-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28a94-147">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="28a94-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="28a94-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="28a94-148">showNameNextToLogo</span></span>|<span data-ttu-id="28a94-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="28a94-149">Boolean</span></span>|<span data-ttu-id="28a94-150">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="28a94-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="28a94-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="28a94-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="28a94-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28a94-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28a94-153">Compnay ポータル アプリケーションのランディング ・ ページに表示されるイメージをカスタマイズしました。</span><span class="sxs-lookup"><span data-stu-id="28a94-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="28a94-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="28a94-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="28a94-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="28a94-155">Boolean</span></span>|<span data-ttu-id="28a94-156">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="28a94-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a94-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28a94-157">Relationships</span></span>
<span data-ttu-id="28a94-158">なし</span><span class="sxs-lookup"><span data-stu-id="28a94-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28a94-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28a94-159">JSON Representation</span></span>
<span data-ttu-id="28a94-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28a94-160">Here is a JSON representation of the resource.</span></span>
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





