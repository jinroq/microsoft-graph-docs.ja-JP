---
title: intuneBrand リソース タイプ
description: intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec1db08ee3e6d6a669078800f2fab69950db14e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917707"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="21d45-103">intuneBrand リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="21d45-103">intuneBrand resource type</span></span>

> <span data-ttu-id="21d45-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="21d45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21d45-105">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="21d45-105">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="21d45-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21d45-106">Properties</span></span>
|<span data-ttu-id="21d45-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21d45-107">Property</span></span>|<span data-ttu-id="21d45-108">種類</span><span class="sxs-lookup"><span data-stu-id="21d45-108">Type</span></span>|<span data-ttu-id="21d45-109">説明</span><span class="sxs-lookup"><span data-stu-id="21d45-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d45-110">displayName</span><span class="sxs-lookup"><span data-stu-id="21d45-110">displayName</span></span>|<span data-ttu-id="21d45-111">String</span><span class="sxs-lookup"><span data-stu-id="21d45-111">String</span></span>|<span data-ttu-id="21d45-112">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="21d45-112">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="21d45-113">contactITName</span><span class="sxs-lookup"><span data-stu-id="21d45-113">contactITName</span></span>|<span data-ttu-id="21d45-114">String</span><span class="sxs-lookup"><span data-stu-id="21d45-114">String</span></span>|<span data-ttu-id="21d45-115">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="21d45-115">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="21d45-116">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="21d45-116">contactITPhoneNumber</span></span>|<span data-ttu-id="21d45-117">String</span><span class="sxs-lookup"><span data-stu-id="21d45-117">String</span></span>|<span data-ttu-id="21d45-118">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="21d45-118">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="21d45-119">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="21d45-119">contactITEmailAddress</span></span>|<span data-ttu-id="21d45-120">String</span><span class="sxs-lookup"><span data-stu-id="21d45-120">String</span></span>|<span data-ttu-id="21d45-121">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="21d45-121">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="21d45-122">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="21d45-122">contactITNotes</span></span>|<span data-ttu-id="21d45-123">String</span><span class="sxs-lookup"><span data-stu-id="21d45-123">String</span></span>|<span data-ttu-id="21d45-124">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="21d45-124">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="21d45-125">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="21d45-125">privacyUrl</span></span>|<span data-ttu-id="21d45-126">String</span><span class="sxs-lookup"><span data-stu-id="21d45-126">String</span></span>|<span data-ttu-id="21d45-127">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="21d45-127">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="21d45-128">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="21d45-128">onlineSupportSiteUrl</span></span>|<span data-ttu-id="21d45-129">String</span><span class="sxs-lookup"><span data-stu-id="21d45-129">String</span></span>|<span data-ttu-id="21d45-130">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="21d45-130">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="21d45-131">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="21d45-131">onlineSupportSiteName</span></span>|<span data-ttu-id="21d45-132">String</span><span class="sxs-lookup"><span data-stu-id="21d45-132">String</span></span>|<span data-ttu-id="21d45-133">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="21d45-133">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="21d45-134">themeColor</span><span class="sxs-lookup"><span data-stu-id="21d45-134">themeColor</span></span>|[<span data-ttu-id="21d45-135">rgbColor</span><span class="sxs-lookup"><span data-stu-id="21d45-135">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="21d45-136">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="21d45-136">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="21d45-137">showLogo</span><span class="sxs-lookup"><span data-stu-id="21d45-137">showLogo</span></span>|<span data-ttu-id="21d45-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="21d45-138">Boolean</span></span>|<span data-ttu-id="21d45-139">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="21d45-139">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="21d45-140">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="21d45-140">lightBackgroundLogo</span></span>|[<span data-ttu-id="21d45-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21d45-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21d45-142">ロゴの背景色が明るいポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="21d45-142">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="21d45-143">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="21d45-143">darkBackgroundLogo</span></span>|[<span data-ttu-id="21d45-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21d45-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21d45-145">ロゴの背景色が暗いポータル サイト アプリに表示されるロゴ画像。</span><span class="sxs-lookup"><span data-stu-id="21d45-145">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="21d45-146">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="21d45-146">showNameNextToLogo</span></span>|<span data-ttu-id="21d45-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="21d45-147">Boolean</span></span>|<span data-ttu-id="21d45-148">管理者が指定した名前がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="21d45-148">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="21d45-149">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="21d45-149">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="21d45-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="21d45-150">Boolean</span></span>|<span data-ttu-id="21d45-151">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="21d45-151">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d45-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21d45-152">Relationships</span></span>
<span data-ttu-id="21d45-153">なし</span><span class="sxs-lookup"><span data-stu-id="21d45-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21d45-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21d45-154">JSON Representation</span></span>
<span data-ttu-id="21d45-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21d45-155">Here is a JSON representation of the resource.</span></span>
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
  "showDisplayNameNextToLogo": true
}
```



