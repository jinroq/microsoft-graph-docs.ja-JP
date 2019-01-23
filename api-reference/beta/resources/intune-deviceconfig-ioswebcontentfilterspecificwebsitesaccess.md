---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。 先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424764"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="04c8e-104">iosWebContentFilterSpecificWebsitesAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04c8e-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="04c8e-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04c8e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04c8e-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04c8e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04c8e-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04c8e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04c8e-108">IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="04c8e-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="04c8e-109">先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。</span><span class="sxs-lookup"><span data-stu-id="04c8e-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="04c8e-110">[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="04c8e-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04c8e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04c8e-111">Properties</span></span>
|<span data-ttu-id="04c8e-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04c8e-112">Property</span></span>|<span data-ttu-id="04c8e-113">型</span><span class="sxs-lookup"><span data-stu-id="04c8e-113">Type</span></span>|<span data-ttu-id="04c8e-114">説明</span><span class="sxs-lookup"><span data-stu-id="04c8e-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c8e-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="04c8e-115">specificWebsitesOnly</span></span>|<span data-ttu-id="04c8e-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04c8e-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="04c8e-117">組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。</span><span class="sxs-lookup"><span data-stu-id="04c8e-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="04c8e-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="04c8e-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04c8e-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="04c8e-119">websiteList</span></span>|<span data-ttu-id="04c8e-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04c8e-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="04c8e-121">組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。</span><span class="sxs-lookup"><span data-stu-id="04c8e-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="04c8e-122">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="04c8e-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04c8e-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04c8e-123">Relationships</span></span>
<span data-ttu-id="04c8e-124">なし</span><span class="sxs-lookup"><span data-stu-id="04c8e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04c8e-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04c8e-125">JSON Representation</span></span>
<span data-ttu-id="04c8e-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04c8e-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```




