---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465280"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="0ddcf-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ddcf-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="0ddcf-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ddcf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ddcf-105">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="0ddcf-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="0ddcf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ddcf-106">Properties</span></span>
|<span data-ttu-id="0ddcf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ddcf-107">Property</span></span>|<span data-ttu-id="0ddcf-108">型</span><span class="sxs-lookup"><span data-stu-id="0ddcf-108">Type</span></span>|<span data-ttu-id="0ddcf-109">説明</span><span class="sxs-lookup"><span data-stu-id="0ddcf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ddcf-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="0ddcf-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="0ddcf-111">文字列</span><span class="sxs-lookup"><span data-stu-id="0ddcf-111">String</span></span>|<span data-ttu-id="0ddcf-112">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="0ddcf-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="0ddcf-113">プロキシ</span><span class="sxs-lookup"><span data-stu-id="0ddcf-113">proxy</span></span>|<span data-ttu-id="0ddcf-114">文字列</span><span class="sxs-lookup"><span data-stu-id="0ddcf-114">String</span></span>|<span data-ttu-id="0ddcf-115">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="0ddcf-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ddcf-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ddcf-116">Relationships</span></span>
<span data-ttu-id="0ddcf-117">なし</span><span class="sxs-lookup"><span data-stu-id="0ddcf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ddcf-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ddcf-118">JSON Representation</span></span>
<span data-ttu-id="0ddcf-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ddcf-119">Here is a JSON representation of the resource.</span></span>
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



