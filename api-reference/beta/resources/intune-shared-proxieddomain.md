---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4668a58e09b21c2689e10c27e773128f886b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971551"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="20bce-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20bce-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="20bce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20bce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20bce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20bce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20bce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20bce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20bce-107">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="20bce-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="20bce-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20bce-108">Properties</span></span>
|<span data-ttu-id="20bce-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20bce-109">Property</span></span>|<span data-ttu-id="20bce-110">種類</span><span class="sxs-lookup"><span data-stu-id="20bce-110">Type</span></span>|<span data-ttu-id="20bce-111">説明</span><span class="sxs-lookup"><span data-stu-id="20bce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20bce-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="20bce-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="20bce-113">文字列</span><span class="sxs-lookup"><span data-stu-id="20bce-113">String</span></span>|<span data-ttu-id="20bce-114">IP アドレスまたは完全修飾ドメイン名 (FQDN) です。</span><span class="sxs-lookup"><span data-stu-id="20bce-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="20bce-115">プロキシ</span><span class="sxs-lookup"><span data-stu-id="20bce-115">proxy</span></span>|<span data-ttu-id="20bce-116">文字列</span><span class="sxs-lookup"><span data-stu-id="20bce-116">String</span></span>|<span data-ttu-id="20bce-117">プロキシの IP アドレスまたは FQDN です。</span><span class="sxs-lookup"><span data-stu-id="20bce-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20bce-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20bce-118">Relationships</span></span>
<span data-ttu-id="20bce-119">なし</span><span class="sxs-lookup"><span data-stu-id="20bce-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20bce-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20bce-120">JSON Representation</span></span>
<span data-ttu-id="20bce-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20bce-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



