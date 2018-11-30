---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
ms.openlocfilehash: 310ccb1420ed450c9e7c53d534181720f9051ff4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067511"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="eea72-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eea72-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="eea72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eea72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eea72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eea72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eea72-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eea72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eea72-107">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="eea72-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="eea72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eea72-108">Properties</span></span>
|<span data-ttu-id="eea72-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eea72-109">Property</span></span>|<span data-ttu-id="eea72-110">型</span><span class="sxs-lookup"><span data-stu-id="eea72-110">Type</span></span>|<span data-ttu-id="eea72-111">説明</span><span class="sxs-lookup"><span data-stu-id="eea72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea72-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="eea72-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="eea72-113">文字列</span><span class="sxs-lookup"><span data-stu-id="eea72-113">String</span></span>|<span data-ttu-id="eea72-114">IP アドレスまたは完全修飾ドメイン名 (FQDN) です。</span><span class="sxs-lookup"><span data-stu-id="eea72-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="eea72-115">プロキシ</span><span class="sxs-lookup"><span data-stu-id="eea72-115">proxy</span></span>|<span data-ttu-id="eea72-116">文字列</span><span class="sxs-lookup"><span data-stu-id="eea72-116">String</span></span>|<span data-ttu-id="eea72-117">プロキシの IP アドレスまたは FQDN です。</span><span class="sxs-lookup"><span data-stu-id="eea72-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eea72-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eea72-118">Relationships</span></span>
<span data-ttu-id="eea72-119">なし</span><span class="sxs-lookup"><span data-stu-id="eea72-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea72-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eea72-120">JSON Representation</span></span>
<span data-ttu-id="eea72-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eea72-121">Here is a JSON representation of the resource.</span></span>
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



