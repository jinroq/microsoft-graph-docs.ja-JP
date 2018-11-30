---
title: iosWebContentFilterSpecificWebsitesAccess リソースの種類
description: IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。 先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。
ms.openlocfilehash: c5e23905ab9e5b692500544161fc052dd606da5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070771"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="f6839-104">iosWebContentFilterSpecificWebsitesAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6839-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="f6839-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6839-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6839-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6839-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6839-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6839-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6839-108">IOS iOS の組み込みブラウザーに URL のブックマークをインストールする Web コンテンツのフィルター設定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="f6839-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="f6839-109">先生が受講者が、iOS デバイスと他のサイトへのアクセスなしで構成されているブラウザーのブックマークから web サイトを移動するようには教室では、シナリオの例です。</span><span class="sxs-lookup"><span data-stu-id="f6839-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>

<span data-ttu-id="f6839-110">[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f6839-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6839-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6839-111">Properties</span></span>
|<span data-ttu-id="f6839-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6839-112">Property</span></span>|<span data-ttu-id="f6839-113">型</span><span class="sxs-lookup"><span data-stu-id="f6839-113">Type</span></span>|<span data-ttu-id="f6839-114">説明</span><span class="sxs-lookup"><span data-stu-id="f6839-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6839-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="f6839-115">specificWebsitesOnly</span></span>|<span data-ttu-id="f6839-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6839-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="f6839-117">組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。</span><span class="sxs-lookup"><span data-stu-id="f6839-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="f6839-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f6839-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f6839-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="f6839-119">websiteList</span></span>|<span data-ttu-id="f6839-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6839-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="f6839-121">組み込みのブラウザーやユーザーにインストールされている URL のブックマークはブックマークから web サイトにアクセスのみ許可されます。</span><span class="sxs-lookup"><span data-stu-id="f6839-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="f6839-122">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f6839-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6839-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f6839-123">Relationships</span></span>
<span data-ttu-id="f6839-124">なし</span><span class="sxs-lookup"><span data-stu-id="f6839-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6839-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6839-125">JSON Representation</span></span>
<span data-ttu-id="f6839-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6839-126">Here is a JSON representation of the resource.</span></span>
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





