---
title: proxiedDomain リソースの種類
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API の proxiedDomain リソースについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b13e880508c80a009eacb520452c66e7b733ad86
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421845"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="b693a-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b693a-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="b693a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b693a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b693a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b693a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b693a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b693a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b693a-107">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="b693a-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="b693a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b693a-108">Properties</span></span>
|<span data-ttu-id="b693a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b693a-109">Property</span></span>|<span data-ttu-id="b693a-110">型</span><span class="sxs-lookup"><span data-stu-id="b693a-110">Type</span></span>|<span data-ttu-id="b693a-111">説明</span><span class="sxs-lookup"><span data-stu-id="b693a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b693a-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="b693a-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="b693a-113">文字列</span><span class="sxs-lookup"><span data-stu-id="b693a-113">String</span></span>|<span data-ttu-id="b693a-114">IP アドレスまたは完全修飾ドメイン名 (FQDN) です。</span><span class="sxs-lookup"><span data-stu-id="b693a-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="b693a-115">プロキシ</span><span class="sxs-lookup"><span data-stu-id="b693a-115">proxy</span></span>|<span data-ttu-id="b693a-116">文字列</span><span class="sxs-lookup"><span data-stu-id="b693a-116">String</span></span>|<span data-ttu-id="b693a-117">プロキシの IP アドレスまたは FQDN です。</span><span class="sxs-lookup"><span data-stu-id="b693a-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b693a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b693a-118">Relationships</span></span>
<span data-ttu-id="b693a-119">なし</span><span class="sxs-lookup"><span data-stu-id="b693a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b693a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b693a-120">JSON Representation</span></span>
<span data-ttu-id="b693a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b693a-121">Here is a JSON representation of the resource.</span></span>
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



