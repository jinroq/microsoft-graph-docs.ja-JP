---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: Ios の組み込みブラウザーに URL ブックマークをインストールする、iOS Web コンテンツフィルター設定の種類を表します。 この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32cf57ba7ab96a68914ceeaf0693162ef9ab8e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001055"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="b02c3-104">iosWebContentFilterSpecificWebsitesAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b02c3-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="b02c3-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b02c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b02c3-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b02c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b02c3-107">Ios の組み込みブラウザーに URL ブックマークをインストールする、iOS Web コンテンツフィルター設定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b02c3-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="b02c3-108">この例は、教師が iOS デバイスで構成されているブラウザーのブックマークを使用して web サイトにアクセスして、他のサイトにアクセスできないようにするための教室のクラスです。</span><span class="sxs-lookup"><span data-stu-id="b02c3-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="b02c3-109">[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b02c3-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b02c3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b02c3-110">Properties</span></span>
|<span data-ttu-id="b02c3-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b02c3-111">Property</span></span>|<span data-ttu-id="b02c3-112">型</span><span class="sxs-lookup"><span data-stu-id="b02c3-112">Type</span></span>|<span data-ttu-id="b02c3-113">説明</span><span class="sxs-lookup"><span data-stu-id="b02c3-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b02c3-114">固有の Webwebonly</span><span class="sxs-lookup"><span data-stu-id="b02c3-114">specificWebsitesOnly</span></span>|<span data-ttu-id="b02c3-115">[Iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b02c3-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b02c3-116">組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b02c3-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b02c3-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b02c3-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b02c3-118">websiteList</span><span class="sxs-lookup"><span data-stu-id="b02c3-118">websiteList</span></span>|<span data-ttu-id="b02c3-119">[Iosbookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b02c3-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b02c3-120">組み込みのブラウザーとユーザーにインストールされる URL ブックマークは、ブックマークを介して web サイトにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b02c3-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b02c3-121">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b02c3-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b02c3-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b02c3-122">Relationships</span></span>
<span data-ttu-id="b02c3-123">なし</span><span class="sxs-lookup"><span data-stu-id="b02c3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b02c3-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b02c3-124">JSON Representation</span></span>
<span data-ttu-id="b02c3-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b02c3-125">Here is a JSON representation of the resource.</span></span>
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





