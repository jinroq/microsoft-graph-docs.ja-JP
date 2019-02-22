---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3e899f418ea9214530ac3b70e493a15655ca873
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167383"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="8a31c-103">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8a31c-103">intuneBrand resource type</span></span>

> <span data-ttu-id="8a31c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a31c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a31c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a31c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a31c-106">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a31c-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="8a31c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a31c-107">Properties</span></span>
|<span data-ttu-id="8a31c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a31c-108">Property</span></span>|<span data-ttu-id="8a31c-109">型</span><span class="sxs-lookup"><span data-stu-id="8a31c-109">Type</span></span>|<span data-ttu-id="8a31c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a31c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a31c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8a31c-111">displayName</span></span>|<span data-ttu-id="8a31c-112">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-112">String</span></span>|<span data-ttu-id="8a31c-113">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="8a31c-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="8a31c-114">contactITName</span><span class="sxs-lookup"><span data-stu-id="8a31c-114">contactITName</span></span>|<span data-ttu-id="8a31c-115">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-115">String</span></span>|<span data-ttu-id="8a31c-116">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="8a31c-116">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="8a31c-117">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8a31c-117">contactITPhoneNumber</span></span>|<span data-ttu-id="8a31c-118">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-118">String</span></span>|<span data-ttu-id="8a31c-119">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="8a31c-119">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="8a31c-120">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8a31c-120">contactITEmailAddress</span></span>|<span data-ttu-id="8a31c-121">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-121">String</span></span>|<span data-ttu-id="8a31c-122">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8a31c-122">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="8a31c-123">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="8a31c-123">contactITNotes</span></span>|<span data-ttu-id="8a31c-124">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-124">String</span></span>|<span data-ttu-id="8a31c-125">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="8a31c-125">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="8a31c-126">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="8a31c-126">privacyUrl</span></span>|<span data-ttu-id="8a31c-127">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-127">String</span></span>|<span data-ttu-id="8a31c-128">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="8a31c-128">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="8a31c-129">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="8a31c-129">onlineSupportSiteUrl</span></span>|<span data-ttu-id="8a31c-130">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-130">String</span></span>|<span data-ttu-id="8a31c-131">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="8a31c-131">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="8a31c-132">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="8a31c-132">onlineSupportSiteName</span></span>|<span data-ttu-id="8a31c-133">String</span><span class="sxs-lookup"><span data-stu-id="8a31c-133">String</span></span>|<span data-ttu-id="8a31c-134">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="8a31c-134">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="8a31c-135">themeColor</span><span class="sxs-lookup"><span data-stu-id="8a31c-135">themeColor</span></span>|[<span data-ttu-id="8a31c-136">rgbColor</span><span class="sxs-lookup"><span data-stu-id="8a31c-136">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="8a31c-137">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="8a31c-137">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="8a31c-138">showLogo</span><span class="sxs-lookup"><span data-stu-id="8a31c-138">showLogo</span></span>|<span data-ttu-id="8a31c-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="8a31c-139">Boolean</span></span>|<span data-ttu-id="8a31c-140">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="8a31c-140">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="8a31c-141">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="8a31c-141">lightBackgroundLogo</span></span>|[<span data-ttu-id="8a31c-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a31c-142">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a31c-143">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="8a31c-143">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="8a31c-144">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="8a31c-144">darkBackgroundLogo</span></span>|[<span data-ttu-id="8a31c-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a31c-145">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a31c-146">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="8a31c-146">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="8a31c-147">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="8a31c-147">showNameNextToLogo</span></span>|<span data-ttu-id="8a31c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a31c-148">Boolean</span></span>|<span data-ttu-id="8a31c-149">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="8a31c-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="8a31c-150">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="8a31c-150">landingPageCustomizedImage</span></span>|[<span data-ttu-id="8a31c-151">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a31c-151">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a31c-152">[compnay ポータルアプリのランディングページに表示されるカスタマイズされた画像]</span><span class="sxs-lookup"><span data-stu-id="8a31c-152">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="8a31c-153">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="8a31c-153">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="8a31c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a31c-154">Boolean</span></span>|<span data-ttu-id="8a31c-155">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="8a31c-155">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a31c-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a31c-156">Relationships</span></span>
<span data-ttu-id="8a31c-157">なし</span><span class="sxs-lookup"><span data-stu-id="8a31c-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a31c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a31c-158">JSON Representation</span></span>
<span data-ttu-id="8a31c-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a31c-159">Here is a JSON representation of the resource.</span></span>
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




