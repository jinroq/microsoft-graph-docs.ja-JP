---
title: iosWebContentFilterAutoFilter リソースの種類
description: '[IOS Web コンテンツフィルターの設定] の種類を表します。これにより、iOS 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6bf2da4320c228123e24ae67bd21b13f2c21eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946071"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="3da18-104">iosWebContentFilterAutoFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3da18-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="3da18-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3da18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3da18-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3da18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da18-107">[IOS Web コンテンツフィルターの設定] の種類を表します。これにより、iOS 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。</span><span class="sxs-lookup"><span data-stu-id="3da18-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="3da18-108">プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。</span><span class="sxs-lookup"><span data-stu-id="3da18-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="3da18-109">[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3da18-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3da18-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3da18-110">Properties</span></span>
|<span data-ttu-id="3da18-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3da18-111">Property</span></span>|<span data-ttu-id="3da18-112">型</span><span class="sxs-lookup"><span data-stu-id="3da18-112">Type</span></span>|<span data-ttu-id="3da18-113">説明</span><span class="sxs-lookup"><span data-stu-id="3da18-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da18-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="3da18-114">allowedUrls</span></span>|<span data-ttu-id="3da18-115">String collection</span><span class="sxs-lookup"><span data-stu-id="3da18-115">String collection</span></span>|<span data-ttu-id="3da18-116">アクセスできる追加 Url</span><span class="sxs-lookup"><span data-stu-id="3da18-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="3da18-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="3da18-117">blockedUrls</span></span>|<span data-ttu-id="3da18-118">String collection</span><span class="sxs-lookup"><span data-stu-id="3da18-118">String collection</span></span>|<span data-ttu-id="3da18-119">アクセスのためにブロックされる追加 Url</span><span class="sxs-lookup"><span data-stu-id="3da18-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="3da18-120">関係</span><span class="sxs-lookup"><span data-stu-id="3da18-120">Relationships</span></span>
<span data-ttu-id="3da18-121">なし</span><span class="sxs-lookup"><span data-stu-id="3da18-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3da18-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3da18-122">JSON Representation</span></span>
<span data-ttu-id="3da18-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3da18-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




