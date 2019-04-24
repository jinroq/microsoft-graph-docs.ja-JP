---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: ios の組み込みブラウザーに URL ブックマークをインストールする、ios Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7d5b60af9a3b17923faac4dd0136ef6a9bc1591
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460472"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="b7595-104">iosWebContentFilterSpecificWebsitesAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7595-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="b7595-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7595-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7595-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7595-107">ios の組み込みブラウザーに URL ブックマークをインストールする、ios Web コンテンツフィルター設定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b7595-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="b7595-108">この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。</span><span class="sxs-lookup"><span data-stu-id="b7595-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="b7595-109">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b7595-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7595-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7595-110">Properties</span></span>
|<span data-ttu-id="b7595-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7595-111">Property</span></span>|<span data-ttu-id="b7595-112">型</span><span class="sxs-lookup"><span data-stu-id="b7595-112">Type</span></span>|<span data-ttu-id="b7595-113">説明</span><span class="sxs-lookup"><span data-stu-id="b7595-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7595-114">固有の webwebonly</span><span class="sxs-lookup"><span data-stu-id="b7595-114">specificWebsitesOnly</span></span>|<span data-ttu-id="b7595-115">[iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b7595-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b7595-116">組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b7595-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b7595-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b7595-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b7595-118">websiteList</span><span class="sxs-lookup"><span data-stu-id="b7595-118">websiteList</span></span>|<span data-ttu-id="b7595-119">[iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b7595-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b7595-120">組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b7595-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b7595-121">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b7595-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7595-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7595-122">Relationships</span></span>
<span data-ttu-id="b7595-123">なし</span><span class="sxs-lookup"><span data-stu-id="b7595-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7595-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7595-124">JSON Representation</span></span>
<span data-ttu-id="b7595-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7595-125">Here is a JSON representation of the resource.</span></span>
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





