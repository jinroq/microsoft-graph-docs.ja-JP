---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98b58759fbac16ad7fad78dc2a9ef0c449c42659
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793624"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="0464c-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0464c-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="0464c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0464c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0464c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0464c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0464c-106">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="0464c-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="0464c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0464c-107">Properties</span></span>
|<span data-ttu-id="0464c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0464c-108">Property</span></span>|<span data-ttu-id="0464c-109">型</span><span class="sxs-lookup"><span data-stu-id="0464c-109">Type</span></span>|<span data-ttu-id="0464c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0464c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0464c-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="0464c-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="0464c-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0464c-112">String</span></span>|<span data-ttu-id="0464c-113">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="0464c-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="0464c-114">プロキシ</span><span class="sxs-lookup"><span data-stu-id="0464c-114">proxy</span></span>|<span data-ttu-id="0464c-115">文字列</span><span class="sxs-lookup"><span data-stu-id="0464c-115">String</span></span>|<span data-ttu-id="0464c-116">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="0464c-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="0464c-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0464c-117">Relationships</span></span>
<span data-ttu-id="0464c-118">なし</span><span class="sxs-lookup"><span data-stu-id="0464c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0464c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0464c-119">JSON Representation</span></span>
<span data-ttu-id="0464c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0464c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```





