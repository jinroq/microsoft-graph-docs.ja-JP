---
title: iosWebContentFilterAutoFilter リソースの種類
description: '[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74e281a4cbc08467730680b556e6e8026535ff3a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155665"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="18e15-104">iosWebContentFilterAutoFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18e15-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="18e15-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18e15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18e15-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18e15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18e15-107">[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。</span><span class="sxs-lookup"><span data-stu-id="18e15-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="18e15-108">プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。</span><span class="sxs-lookup"><span data-stu-id="18e15-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="18e15-109">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="18e15-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18e15-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18e15-110">Properties</span></span>
|<span data-ttu-id="18e15-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18e15-111">Property</span></span>|<span data-ttu-id="18e15-112">型</span><span class="sxs-lookup"><span data-stu-id="18e15-112">Type</span></span>|<span data-ttu-id="18e15-113">説明</span><span class="sxs-lookup"><span data-stu-id="18e15-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e15-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="18e15-114">allowedUrls</span></span>|<span data-ttu-id="18e15-115">String collection</span><span class="sxs-lookup"><span data-stu-id="18e15-115">String collection</span></span>|<span data-ttu-id="18e15-116">アクセスできる追加 url</span><span class="sxs-lookup"><span data-stu-id="18e15-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="18e15-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="18e15-117">blockedUrls</span></span>|<span data-ttu-id="18e15-118">String collection</span><span class="sxs-lookup"><span data-stu-id="18e15-118">String collection</span></span>|<span data-ttu-id="18e15-119">アクセスのためにブロックされる追加 url</span><span class="sxs-lookup"><span data-stu-id="18e15-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="18e15-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18e15-120">Relationships</span></span>
<span data-ttu-id="18e15-121">なし</span><span class="sxs-lookup"><span data-stu-id="18e15-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18e15-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18e15-122">JSON Representation</span></span>
<span data-ttu-id="18e15-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18e15-123">Here is a JSON representation of the resource.</span></span>
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




