---
title: iosWebContentFilterAutoFilter リソースの種類
description: '[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。 プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91efedb47fff71a66d12e0d2c976d61fab2fa76c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460416"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="4ffbe-104">iosWebContentFilterAutoFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ffbe-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="4ffbe-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ffbe-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ffbe-107">[ios Web コンテンツフィルターの設定] の種類を表します。これにより、ios 自動フィルター機能が有効になり、追加の URL アクセス制御が許可されます。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="4ffbe-108">プロパティ値を指定しないで構築された場合、iOS デバイスはに関係なく自動フィルターを有効にします。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="4ffbe-109">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ffbe-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ffbe-110">Properties</span></span>
|<span data-ttu-id="4ffbe-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ffbe-111">Property</span></span>|<span data-ttu-id="4ffbe-112">型</span><span class="sxs-lookup"><span data-stu-id="4ffbe-112">Type</span></span>|<span data-ttu-id="4ffbe-113">説明</span><span class="sxs-lookup"><span data-stu-id="4ffbe-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ffbe-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="4ffbe-114">allowedUrls</span></span>|<span data-ttu-id="4ffbe-115">String collection</span><span class="sxs-lookup"><span data-stu-id="4ffbe-115">String collection</span></span>|<span data-ttu-id="4ffbe-116">アクセスできる追加 url</span><span class="sxs-lookup"><span data-stu-id="4ffbe-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="4ffbe-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="4ffbe-117">blockedUrls</span></span>|<span data-ttu-id="4ffbe-118">String collection</span><span class="sxs-lookup"><span data-stu-id="4ffbe-118">String collection</span></span>|<span data-ttu-id="4ffbe-119">アクセスのためにブロックされる追加 url</span><span class="sxs-lookup"><span data-stu-id="4ffbe-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ffbe-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ffbe-120">Relationships</span></span>
<span data-ttu-id="4ffbe-121">なし</span><span class="sxs-lookup"><span data-stu-id="4ffbe-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ffbe-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ffbe-122">JSON Representation</span></span>
<span data-ttu-id="4ffbe-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ffbe-123">Here is a JSON representation of the resource.</span></span>
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





